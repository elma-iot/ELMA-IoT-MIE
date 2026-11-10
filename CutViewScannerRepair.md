# Well cut-view scanner failure and seabed alignment

The 1.19.32 viewer reproduced MILERR_SCANNER_FAILED (HRESULT 0x88980004) on the saved 15-component K.Amasra-06 assembly. The stack trace points to PathGeometry.InternalCombine from WellTerrainCavities.ClearFaces. The native Boolean scanner was receiving kilometre-scale terrain with a 0.0000001 m absolute tolerance, including small equipment cavity contours.

Soil mask union and subtraction now run in a bounded local coordinate frame, then return to world coordinates. Existing fill rules and transforms are retained. Original engineering meshes, units, source GLBs and saved well definitions are unchanged.

The water cut mask follows the successfully displayed section's axis, position and side. A pending or failed section retains the matching previous mask instead of switching the backdrop before geometry arrives. Publishing completed cut geometry updates its mask immediately. Seabed and movement viewports share the active perspective/orthographic camera with the equipment viewport.

Validation:

- Reproduced the original failure with the released viewer and opened the project for import/read-only; the source project was not saved or changed.
- The fixed saved-assembly cuts at 50% and 60% succeeded (about 3.9 s first preparation, 1.2 s second position). Actual asynchronous section publication succeeded, followed by a rendered screenshot with sectioned hardware and no floating seabed tile.
- Returning to the normal view restored exactly the original submitted triangle count (3,059,154). CPU frame-update probes remained below 0.1 ms; these are CPU update timings, not GPU frame-rate measurements.
- Cavity checks passed for X/Y/Z and both sides: bore exclusion, soil outside the bore, deep formations and source immutability.
- Section-plane, terrain occlusion/haze, terrain cut and incremental well-assembly regressions passed.
- Seven new cut-view consistency checks passed for pending/failed cuts, published masks, in-flight edits, both projections, motion-overlay camera and disabling the cut.

Evidence is local under `.audit/CutRepair/`. A separate test application uses an exact-hash development viewer override in `.audit/CutRepair/test-app`; published 1.19.32 packages remain immutable. This repair is not yet a new Store release.
