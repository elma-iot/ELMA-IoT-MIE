# MIE 1.19.12 review — attachment removal

Item View has a compact Delete button beside Upload, a Delete right-click command and the Del keyboard shortcut for the selected attachment. All use one confirmation dialog, including Enter to confirm and Escape to cancel. The action prepares and commits through the responsive background transaction workflow, refreshes the current list, and guards stale selections and pending model edits.

Removal is scoped to one equipment identity and content hash. Same-byte aliases on that item are hidden together. Other equipment keeps shared PN models. Original files on disk and immutable historical evidence remain intact; current inspection selection excludes removed files. Re-upload explicitly restores a removed file. Undo/Redo records compensating lifecycle events.

Visibility is stored separately from equipment condition and stock state, using the existing project resource and lifecycle components. Causal visibility intents survive native saves, incremental saves, sync and project exchanges. Concurrent removal/restoration requires explicit review. Unrelated concurrent uploads and equipment edits cannot silently restore a removed model. Scoped packets include the selected item's visibility records.

Older projects remain readable. A project using attachment visibility requires MIE 1.19.12 or newer, preventing older apps from silently ignoring the removal. Historical evidence is retained, so removing an attachment from the active list does not guarantee a reduction in .miepack size. No source file, equipment quantity, licensing rule, user role or database architecture is changed.

Guide and synthetic tutorial updated in all twenty languages, with public data packs v50. Existing verified optional modules remain compatible and unchanged. This portable review has not been submitted to Microsoft Store. No operational project, license or key is included in Git or release assets.
