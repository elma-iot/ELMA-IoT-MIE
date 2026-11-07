# MIE 1.19.19 candidate validation

Prepared for owner testing; Microsoft Store submission is held.

553 targeted assertions passed across 20 suites.

- WorkingPersistenceChecks: 16 assertions
- ResponsiveSnapshotChecks: 2 assertions
- IncrementalLocalSaveChecks: 11 assertions
- LifecycleChecks: 16 assertions
- LifecycleAdvancedChecks: 11 assertions
- LifecycleTransferChecks: 5 assertions
- LifecycleSyncChecks: 7 assertions
- AnnotationLifecycleChecks: 9 assertions
- SaveAsChecks: 11 assertions
- SaveTutorialChecks: 53 assertions
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

Working-persistence tests verify no per-edit project/journal write, no generic resize progress bar, unchanged lifecycle data during sizing, PC-input idle deferral, named and unnamed recovery, retained pending history, edits during checkpoint generation, incremental temporary overlays and quiet ten-minute idle saving. Incremental-save tests cover compressed resource reuse, backups and encryption. Lifecycle tests cover disposal protections, inspection, return, evidence, sync reconciliation and annotation retention. Save tutorial checks cover all 20 supported languages.

Sizing tests verify MIE pack persistence, native/project and extracted Excel dimensions, offscreen fit measurement, compact cleared cells, light/dark editor styling and Undo. The drag tests include a 35-pixel parent offset, an image-level check for the blank-strip regression, zoom, pointer movement above/below the headers, both endpoints, acceleration and braking. Equipment checks cover six-item limits, PN assignment, per-SN lifecycle/Quarantine/return, duplicate details, Save/Load, complete Delete/Undo, grouped Cut/Copy/Paste and text replacement. The actual occupied-cell dialog is checked for Append and Cancel and the six-item limit.

The Store candidate passes offline pack verification and damaged-module rejection. SDK MakeAppx packaging and archive/manifest checks pass. Role backend and dynamic UI checks pass. Owner testing of the live pointer interaction and working project remains pending.

The historical StockMovementChecks harness was stopped at an unhandled nested receipt dialog; it has not been counted as a pass. The current confirmation-dialog and backend movement suites pass.

Portable SHA256: `a5a8fd52b78c0de07563f2a91f07383e792e2aeb01195a4f55643a76e52ac2f2`

MSIX SHA256: `044adbef7a5138f4060da237aded25bc206e205b08b3f66796cc2b853527fb27`
