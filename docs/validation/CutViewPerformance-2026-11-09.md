# Cut-view performance fix — separate development branch

Branch: `fix/cut-view-performance`. The 1.19.27 release and its packages remain unchanged. An isolated, unpublished 1.19.28 development host pins the patched viewer for owner testing.

## Measured bottleneck

The saved assembly has 15 components, 14 representative dimension levels, 63 selectable measurement levels and 35,526 contour edges. After the section completes, the scene contains 458 meshes, 1,628,511 triangles and 4,885,533 vertices.

`WellDimensionsFrame` clips contour edges against the section plane. Each call through `ClipDimensionToCut` previously recalculated `WellTerrain.FrameBounds`, traversing the full assembly repeatedly. A single bounds query took approximately 0.14 ms, but repetition made measurement calculation dominate camera movement. The line/text drawing, water overlay and visibility checks were not the primary cost.

The fix caches the exact framing extent only for frozen scene graphs, keyed weakly by model identity. Rebuilt, reposed or newly cut scenes get independent entries; editable graphs continue calculating live bounds. The value contains only the computed rectangle, so it does not retain the scene. No measurement contours, materials, cap geometry, meshes or source models are changed.

## Same-scene CPU profile

Twenty-five warm samples per operation, same host, completed cut, viewport and source assembly:

| Operation | Before median | After median |
|---|---:|---:|
| Cut-view camera update | 247.072 ms | 1.361 ms |
| Measurement-frame calculation | 247.952 ms | 0.470 ms |
| DATUM and measurement update | 249.400 ms | 0.494 ms |
| Water overlay | 0.002 ms | 0.004 ms |

These are UI-thread CPU timings, not a GPU FPS guarantee. The camera-update path improves by approximately 181 times on the measured scene. Both runs use identical mesh, triangle and vertex counts.

Completed-cut captures at the same fixed camera position are byte-identical before and after: SHA-256 `69d1135feef70f8e2e870618a6a7762dcfe3ef6a2b7164d8a34cfc0f825b7c31`.

## Validation

137 targeted assertions pass: 10 new frame-bounds checks, 17 section-plane checks, 12 terrain checks, 50 cut-dimension/camera checks, 26 measurement-selection checks, 4 saved-well checks, 7 print-capture checks and 11 render-performance checks. Coverage includes transformed/frozen geometry, concurrent reads, mutable transforms and meshes, independent rebuilt poses, all cut axes/sides, retained contour anchors while orbiting, saved real-well measurements, nonoverlapping horizontal dimension text, high-resolution printing and original-file preservation.

The reproducible real-project probe is `tools/Checks/WellCutPerformanceProbe.cs`; it reads a project without recovery or saving and uses its saved constructor plan. Development logs and captures stay in the ignored `.audit/CutPerformance20261109` directory. No customer project or license is included in Git.

No controls or workflows changed, so the existing user-guide, tutorial and translation instructions remain applicable. Public release publication and Store submission have not been performed.
