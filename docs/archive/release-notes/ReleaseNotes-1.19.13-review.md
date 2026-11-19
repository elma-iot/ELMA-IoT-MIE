# MIE 1.19.13 review — attachment Replace and Rename

Item View attachment context menus now include Replace and Rename alongside Save as and Delete. F2 opens Rename. Both actions use confirmation, Enter/Escape, background transactions, stale-selection checks and Undo/Redo.

Rename changes the displayed filename for the selected equipment, preserving its extension and rejecting invalid or duplicate names. Save as uses the displayed name. Original source files and immutable historical evidence keep their original names. Filename intents have causal reconciliation and explicit concurrent conflict review; Undo/Redo writes compensating audit events.

Replace selects one file and hides the previous upload for this equipment after confirmation. Original evidence remains in history and other equipment retains shared PN originals. Replacing with identical bytes is rejected; use Rename instead. Different model geometry keeps its own model-hash annotation history, so old damage is not copied to unrelated geometry. Replacement does not delete source files or compact retained historical data.

Older projects remain readable. Renamed attachment projects require MIE 1.19.13 or newer; removal/replacement visibility requires 1.19.12. Native/incremental saves, selected-record packets and project synchronization preserve the new records. Existing optional executable modules remain unchanged. The public v51 language and learning packs include the new controls and help in all twenty languages.

Validation: release build passes; attachment edit data checks cover rename scope, shared siblings, project exchange, native save/reopen, reader guard, concurrent rename review, Undo/Redo, invalid paths and replacement deduplication. Removal and incremental-save regressions pass. WPF UI checks exercise the actual Rename context menu, confirmation and refreshed filename, plus existing Delete actions. Lifecycle sync and selected-record transfer regressions pass.

This is a portable review release, not a Microsoft Store submission. No operational project, license, credentials or private key is included in either repository or release.
