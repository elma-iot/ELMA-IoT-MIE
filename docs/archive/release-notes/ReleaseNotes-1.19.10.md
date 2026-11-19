# MIE 1.19.10 — shared original models

Release candidate for owner testing. Microsoft Store submission is on hold; 1.19.09 remains in certification.

- Upload an original GLB once: it appears in Item View for every item with the same part number, including items added later. Shared originals are labelled in the attachment list.
- Only the original model is shared. Documents, custom textures, damage marks, deformation and scene settings remain specific to the individual item. Existing GLB uploads are recognized automatically.
- Native projects retain one content-addressed original. Incremental saves reuse its compressed entry; incremental sync sends new resources without resending unchanged model bytes. Backups retain the same association.
- Selected-item exports include the shared original without another item's documents or damage. Merge preserves the latest active damage and immutable historical checkpoints.
- Returning an item clears its active damage while preserving its history and scene preferences. Other serials remain unchanged.
- Header search by SN, PN or description runs only on Enter or Search. All matches appear in a scrollable dropdown with the tab name; selecting a result collapses it and focuses the destination row. Searches run in the background with cancellation and safe project-change handling.
- Updated guide, tutorials and all 20 language packs.

Validation: shared-PN lookup, legacy uploads, serial isolation, incremental resource selection, native save/reopen and backups, scoped exports, model checkpoint merge, return/undo/redo, inspection documents and save workflows.
