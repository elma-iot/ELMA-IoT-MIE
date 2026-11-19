# MIE 1.19.18 candidate validation

Prepared for owner testing; Microsoft Store submission is held.

412 targeted assertions passed across 10 suites.

- WorksheetSizingChecks: 28 assertions
- EquipmentMembersChecks: 19 assertions
- ColumnPlacementChecks: 20 assertions
- InlineColumnChecks: 26 assertions
- MasterColumnChecks: 15 assertions
- ColumnDragScrollChecks: 15 assertions
- ContextClipboardChecks: 15 assertions
- RoleAccessChecks: 219 assertions
- RoleUiChecks: 30 assertions
- StoreBundleOfflineChecks: 25 assertions

Sizing tests verify MIE pack persistence, native/project and extracted Excel dimensions, offscreen fit measurement, compact cleared cells, light/dark editor styling and Undo. The drag tests include a 35-pixel parent offset, an image-level check for the blank-strip regression, zoom, pointer movement above/below the headers, both endpoints, acceleration and braking. Equipment checks cover six-item limits, PN assignment, per-SN lifecycle/Quarantine/return, duplicate details, Save/Load, complete Delete/Undo, grouped Cut/Copy/Paste and text replacement. The actual occupied-cell dialog is checked for Append and Cancel and the six-item limit.

The Store candidate passes offline pack verification and damaged-module rejection. SDK MakeAppx packaging and archive/manifest checks pass. Role backend and dynamic UI checks pass. Owner testing of the live pointer interaction and working project remains pending.

The historical StockMovementChecks harness was stopped at an unhandled nested receipt dialog; it has not been counted as a pass. The current confirmation-dialog and backend movement suites pass.

Portable SHA256: `8f35ffb51cba468fec08c463d5f4faa472860d144d776bdbf7a74c21a1aa8071`

MSIX SHA256: `82eea367c0a44040b15601f94ac0111b8dfd240651f1f646e348982295c1820f`
