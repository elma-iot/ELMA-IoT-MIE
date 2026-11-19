# MIE 1.19.34 validation

Prepared for owner testing. Microsoft Store submission is pending owner validation.

Verified portable/Store version 1.19.34, matching exact viewer and Theme Studio hashes, all six offline content packages, ZIP/MSIX integrity and absence of project/license files from distributable archives.

- ModelDuplicateChoicesChecks: 9 checks passed.
- ModelReplacementChecks: 12 checks passed.
- WellModelNameChecks: 12 checks passed.
- WellModelResolutionChecks: 13 checks passed.
- StandaloneWellChecks: 31 checks passed.
- WellPortraitPrintChecks: 8 checks passed.
- ConnectionSurfaceUiChecks: 70 checks passed.
- MasterCellEditingChecks: 15 checks passed.
- StoreBundleOfflineChecks: 25 checks passed.

The duplicate tests cover identical model content with differing exporter strings, preferring a configured copy, mapping historical selections to its canonical choice, preserving original bytes, making no project changes while browsing, consistent Item View choices, retaining different geometry, separate damage annotations and conflicting connection profiles.

The well tests cover the toolbar placement beside Select measurements, Cancel preserving the existing drawing, confirmed capture of the live camera/cut/measurement view, persistent preview replacement, retaining the drawing ID and master hyperlink, rejecting stale reviews, keeping the editable constructor and Undo/Redo. The current-scene capture was rendered and visually inspected.

A read-only local investigation found separately attached GLBs with identical binary chunks and JSON differing only in asset.generator. Connection editing writes profile JSON revisions rather than new GLBs. Current choices previously included both metadata variants and superseded versions. This release resolves eligible aliases at read time and preserves original resources and audit history. Genuine geometric variants remain separate.

## Owner-test correction: repeated unavailable serials

The previous restore selected the first component/PN/SN match for every repeated identity. Two unavailable-serial valves therefore reopened on the same connection despite distinct entries in the saved configuration. The compatibility reader now consumes each legacy occurrence once, and new captures store distinct row keys plus parent/target row references.

SavedWellRestoreChecks reproduces the pre-fix collision, confirms distinct restored targets, builds the complete saved assembly, verifies unique saved keys and a capture/restore round trip, and verifies the source project hash remains unchanged. The 31 standalone-well checks and existing model-resolution checks also pass.
