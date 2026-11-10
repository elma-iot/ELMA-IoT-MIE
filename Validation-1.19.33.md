# MIE 1.19.33 validation

Prepared for owner testing; Microsoft Store submission is pending owner validation.

Verified the final portable and Store builds, matching 1.19.33 module digests, six offline packages, ZIP/MSIX integrity and exclusion of project/license files from distribution archives.

- MasterCellEditingChecks: 15 checks passed.
- CellEditorThemeChecks: 31 checks passed.
- IdentifierPreservationChecks: 11 checks passed.
- EquipmentMembersChecks: 19 checks passed.
- StoreBundleOfflineChecks: 25 checks passed.

The broader StockMovementChecks harness reaches the legacy In-Order receipt dialog and waits for an unhandled nested form; it was stopped and is not counted as passed. The focused master editing check independently covers actual routed cell handoff, commit, unavailable serial identity, grouped records, save/reopen, real duplicates and accessibility.

The prior cut-view repair remains included. See [Cut-view scanner repair](CutViewScannerRepair.md) for the actual 15-component saved-well reproduction and section/mask regression evidence.

The Framework 4.8 workaround is scoped to detached editing-column accessibility trackers, preserving the normal grid automation peer. The original local error stack points to `CellAutomationValueHolder.TrackValue` during commit. See [WPF issue 11077](https://github.com/dotnet/wpf/issues/11077) and [current WPF DataGrid source](https://source.dot.net/presentationframework/System/Windows/Controls/DataGrid.cs.html).

## Same-version owner-test revision: standalone 3D wells

The revised 1.19.33 package allows master-list-driven 3D construction without an uploaded drawing. The prior local build was preserved under the ignored ReleaseWorkHistory folder before rebuilding.

- StandaloneWellChecks: 23 checks passed.
- WellPortraitPrintChecks: 8 checks passed.
- WellLicenseUiChecks: 8 checks passed.
- WellModelNameChecks: 12 checks passed.
- MasterCellEditingChecks: 15 checks passed.

The 23 standalone-well checks exercise attached-PN model loading without a drawing, optional-import cancellation state, sidebar naming, No retaining the 3D draft, direct reopening, actual portrait capture, source XLSX containing the image, native persistence of drawing and 3D state, immediate master hyperlink/underline, Undo/Redo, actual tab-switch Yes handling, the standard 2D viewer, exclusion of drafts from XLSX schematic export, and generated-state preservation in background/synchronization metadata.

The final Store bundle also passed all offline content checks after the revision. Both ZIP/MSIX archives and exact component hashes were verified again; Store submission remains on hold for owner testing.
