# MIE 1.19.28 candidate validation

Prepared 9 November 2026 for further owner testing. Microsoft Store upload and submission remain on hold.

## Package validation

Portable and Store builds have assembly version 1.19.28.0. The Store package retains the registered x64 identity and publisher. The new 1.19.28 viewer and Theme Studio fallback are pinned by exact digest; each executable has a matching companion Theme Studio. Six offline content packages match the application-approved hashes. The portable ZIP and MSIX pass archive integrity and payload checks and contain no customer projects, licenses or device authorization files. SHA256SUMS.txt covers the application packages and optional data/module assets.

## Functional validation

The five native-import suites pass against the final release executable: ProjectTransferChecks, ProjectTransferAdvancedChecks, ProjectTransferUiChecks, ProjectImportConflictChecks and ProjectMergeDataChecks. Coverage includes field Keep/Overwrite/Cancel, both stock-conflict choices, grouped members, causal-history exclusion, model-only and settings-only imports, schematic/column identity remapping, live custom columns, live stock tabs, constructor restore, Undo/Redo, encryption and original-file preservation.

The 137 performance/geometry assertions pass against the final release viewer: WellFrameBoundsChecks (10), SectionPlaneChecks (17), WellTerrainChecks (12), WellCutDimensionsChecks (50), WellDimensionSelectionChecks (26), WellSavedDimensionsChecks (4), WellPrintCaptureChecks (7) and SceneRenderPerformanceChecks (11). The real saved-well checks preserve the input pack and include the portrait report and horizontal labels.

All 20 language/learning catalogs pass Check-Content11925.py: 347 current learning entries and 3,430 interface strings, with matching placeholders and packed values. There are no new controls or translatable UI strings in the performance patch; the current complete-merge guide and tutorials are included in versioned 1.19.28 data packs.

## Performance evidence

The measured completed 15-component cut scene retains 458 meshes, 1,628,511 triangles and 4,885,533 vertices. Frozen-bounds caching reduces median UI-thread cut-camera update from 247.072 ms to 1.361 ms and measurement-frame calculation from 247.952 ms to 0.470 ms. These are CPU timings, not GPU FPS guarantees. Completed-cut before/after PNGs are byte-identical. See [the performance investigation](CutViewPerformance-2026-11-09.md).

Owner testing is the remaining gate before Microsoft Store submission.
