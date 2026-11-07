# 1.19.21 progress, model lookup and popup refinement audit

This testing rebuild updates the existing numeric version folder. Store submission remains held for owner testing; connection-point authoring is deferred until the owner specifies the controls after testing.

## Shared progress

One themed footer presents operations by ownership and priority. Foreground workbook/transfer work takes precedence over a concurrent measured save or sync; their values remain independent and resume afterwards. The sync details window has its own measurement instead of binding to whichever operation owns the footer. Disposed/replaced operations reject late reports. Measurement dispatch coalesces queued updates without dropping the most recent value between reports.

Transfers and background workbook actions report actual completed stages: snapshot preparation, application, commit/history, recovery and view refresh. Stage fractions are not time estimates. Unmeasurable preparation uses an activity indicator; byte/work-based exporters and saves preserve measured percentages. The UI paints before dispatcher-only work. The generic workbook path now uses the existing lightweight snapshot, reconstructing worksheet projections on the worker. Synthetic snapshot preparation measured about 4 ms. No project save is added by progress reporting.

The shared handlers cover Master installation cards, modern movement/lifecycle forms, clipboard/Undo/Redo, structural operations, legacy matching-stock selection, Inventory movement and order receipt forms. Item View preview, attachment saving, 3D Beta, print preview and exports also use the footer. Native saving/export progress retains its existing popup and close behavior. Atomic workbook mutations prevent new competing cell edits while retaining navigation; save and sync continue to preserve later edits for a subsequent operation.

## Model lookup

Precise shared-PN registration remains authoritative. Original GLB filenames provide preview-only candidates when no exact registration exists. This addresses legacy uploads attached to a revision-qualified PN or a combined PN/SN field. Candidates are labelled for compatibility review and remain excluded until the user ticks Include. Different PN revisions are not aliased, no registration is written, and serial damage is never copied into the well preview. Exact registered PN models retain their normal confirmed-depth inclusion. The owner's project was inspected read-only and its original bytes were unchanged. Regression fixtures use synthetic identifiers and models.

## Popup placement

Ordinary WPF dialogs and native Windows Open/Save As/Folder dialogs share the workspace anchor policy. Active-owner resolution recognizes undocked workspace ReturnTo relationships, while placement follows ownership only, stopping at that undocked window. Nested popups center on the related workspace rather than an offset parent popup. Dock/undock positioning and existing workspace restoration are untouched.

Native screen coordinates and work-area clamping handle maximized windows and monitor scaling. Initial native picker size changes are coalesced until layout settles. User move/resize messages stop automatic centering and retain the resulting position in a weakly keyed session dictionary; no placement settings are written to disk. A new process starts centered again. Windows remain owned; positioning uses no-activate/no-z-order flags, preserving close/focus behavior. Native hooks are confined to the application UI thread, exclude external processes, and are released on app exit, dispatcher shutdown and process/domain teardown. This also fixes a shutdown callback failure found by the Store offline test.

## Verification

967 passing assertions across 38 selected suites cover the changed operations and their regressions. The shared progress tests hold a worker to verify dispatcher responsiveness, save/sync ownership, failure cleanup, overlap rejection and measured-value restoration. Real native Save As, nested WPF dialogs, undocked fallback ownership, retained manual placement and a fresh child process exercise placement. Focus tests cover accept/cancel and completion while another application has deliberately been selected. Physical second-monitor checks are conditional on available hardware; the current environment exercised its available monitor configuration.

Inventory permanent/retained transfer UI, receipt and stock-selection dialogs, inspection retry/evidence, role backend/UI, grouped equipment, clipboard, history/sync, working recovery, incremental saving, shared model/damage lifecycle, schematic correction/references and Excel/print paths pass. All 20 locale catalogs match the core fallback translations for the eight new labels and preserve formatting placeholders. The assembled MSIX's manifest, archive integrity and embedded executable are verified; all six offline content descriptors load, GLB rendering and Theme Studio launch work, and damaged executable content is rejected. The Store runner exits normally after these checks.

The older SyncFeedback test expected edits made after a save snapshot to already exist in that snapshot's file. The prior executable reproduced that failure. The assertion now verifies the captured snapshot, retained dirty live edits, and their persistence in the next save, matching the established nonblocking-save contract. WorkingPersistenceChecks separately covers completed temporary recovery checkpoints. No saving behavior was changed to satisfy that assertion.

The executable and MSIX are staged in release-assets/1.19.21. Existing settings, content, working data, license and authorization key remain beside the executable. No license, customer project or owner key is tracked in Git.
