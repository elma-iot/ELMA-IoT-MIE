# MIE 1.19.21 — Master Inventory actions and schematic 3D Beta

Prepared for owner testing. Microsoft Store submission remains held.

- Empty informational tooltips are suppressed. Empty Master equipment cells instead offer a deliberate Inventory action card when appropriate stock exists. Right-click Add equipment opens the same card. Sections follow visible Master header order; item lists are virtualized and load in the background.
- Install from the card using the existing checked transfer path. Retain a linked Inventory record or choose permanent removal. Occupied destinations retain Replace/Append/Cancel and the six-item limit. Roles, eligibility, stale-data checks, PN correction, schematic references, stock counts, history and sync are reused.
- Delete on occupied equipment asks Return to Inventory, Delete or Cancel. Grouped returns move every SN to its recorded/matching section as unavailable assessment stock and support one Undo. Linked Inventory member rows affect only their selected serial. Keyboard Delete uses the same choice.
- Schematics adds licensed 3D Beta beside Delete. Review labelled metric depths, seabed, model choices, units, up axes, anchors and lateral offsets. Seabed/stick-up references can derive a wellhead datum. Missing or ambiguous values remain unselected. PDF-only sources require manual depths.
- Assemble original shared PN models with soil at seabed zero. The existing viewer pack supplies scene rendering, camera/cut controls and repeated-geometry reuse. Serial damage is excluded; the preview does not modify equipment records or original model resources.
- Save shows Preparing save immediately, including pending checkpoint waits. Saving no longer computes a full canonical project fingerprint on the UI thread. Snapshot change detection uses the working revision and native workbook stamp. Automatic checkpoints/sync defer during application modal confirmations.
- Grouped returns roll back completely on a conflict. The common conflict check includes newly entered Master equipment that has no lifecycle identity yet. Clearing the last Master PN/SN retires its cell identity, preserving history and allowing the next installation.
- Legacy Master stock installation now delegates to the common checked path while retaining ordinary single-item identities. Movement, return, deletion, clipboard and lifecycle regression checks cover the affected paths.
- Guide/tutorial references and all 20 language catalogs updated. The exact-hash approved viewer pack is updated; other existing modules are reused.

Testing build refinements:
- The existing themed bottom bar now also reports common transfers and background workbook actions across tabs, with completed stage counts and preparation/apply/history/recovery/refresh labels. Measured saves and exports retain actual percentages; unmeasured work uses an activity indicator. Foreground progress cannot be overwritten by concurrent save or sync updates. The sync details window retains its own measurements.
- Inventory movement, legacy stock selection and receipt dialogs use the shared background edit path. Structural edits use the lightweight dispatcher snapshot; workbook reconstruction happens on the worker. Document/model preview, 3D Beta and print preview also report activity in the footer.
- 3D Beta offers exact-filename original-model candidates if no model is registered for the precise PN. The dropdown and source label request compatibility review, and Include stays unticked. This does not alias different PN revisions or modify project data.
- Connection-point authoring is deferred pending owner testing and specification.
- Same-version rebuilds update the single release-assets/1.19.21 folder, preserving its runtime data and license.
- Popup placement is shared across application dialogs and native Windows Save As/Open/Folder dialogs. Popups center on their related main or undocked workspace, preserve manual positions only during this session, and reset on restart. Monitor/DPI changes and native file-picker initialization are handled without re-centering a dialog after the user drags it. Dock/undock placement and close/focus ownership are retained.
