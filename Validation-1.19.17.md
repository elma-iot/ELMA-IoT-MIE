# MIE 1.19.17 candidate validation

Prepared for owner testing; Microsoft Store submission is held.

445 targeted assertions passed across 10 suites.

- EquipmentMembersChecks: 19 assertions
- ColumnPlacementChecks: 20 assertions
- InlineColumnChecks: 26 assertions
- MasterColumnChecks: 15 assertions
- ColumnDragScrollChecks: 15 assertions
- StockSectionChecks: 61 assertions
- ContextClipboardChecks: 15 assertions
- RoleAccessChecks: 219 assertions
- RoleUiChecks: 30 assertions
- StoreBundleOfflineChecks: 25 assertions

The drag tests include a 35-pixel parent offset, an image-level check for the blank-strip regression, zoom, pointer movement above/below the headers, both endpoints, acceleration and braking. Equipment checks cover six-item limits, PN assignment, per-SN lifecycle/Quarantine/return, duplicate details, Save/Load, complete Delete/Undo, grouped Cut/Copy/Paste and text replacement. The actual occupied-cell dialog is checked for Append and Cancel and the six-item limit.

The Store candidate passes offline pack verification and damaged-module rejection. SDK MakeAppx packaging and archive/manifest checks pass. Role backend and dynamic UI checks pass. Owner testing of the live pointer interaction and working project remains pending.

The historical StockMovementChecks harness was stopped at an unhandled nested receipt dialog; it has not been counted as a pass. The current confirmation-dialog and backend movement suites pass.

Portable SHA256: `67c58a16287d4be788b64c4964077dcf22c1983687b0c79bfa99380da060b37e`

MSIX SHA256: `f6fec5303b54d131adcaf2eb880eaf3d68244a56488dddfb2d5e89dee21b9035`
