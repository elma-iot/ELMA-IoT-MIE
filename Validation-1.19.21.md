# MIE 1.19.21 candidate validation

Prepared for owner testing; Microsoft Store submission is held.

633 targeted assertions passed across 23 suites.

- WellInventoryChecks: 27 assertions
- WorkspaceActionChecks: 17 assertions
- GridTipScrollChecks: 9 assertions
- ActionableTipChecks: 14 assertions
- EquipmentEditorLayoutChecks: 62 assertions
- EquipmentCellDeleteChecks: 28 assertions
- EquipmentMembersChecks: 19 assertions
- EquipmentRoutingChecks: 34 assertions
- LifecycleTransferChecks: 5 assertions
- LifecycleSyncChecks: 7 assertions
- ContextClipboardChecks: 15 assertions
- RoleAccessChecks: 219 assertions
- WorkingPersistenceChecks: 16 assertions
- IncrementalLocalSaveChecks: 11 assertions
- CellEditorThemeChecks: 31 assertions
- ModelViewerChecks: 10 assertions
- RoleModelViewerChecks: 11 assertions
- RoleUiChecks: 30 assertions
- SchematicDeletionChecks: 6 assertions
- SchematicReferenceChecks: 11 assertions
- SchematicPnCorrectionChecks: 20 assertions
- EquipmentRoutingDuplicateChecks: 6 assertions
- StoreBundleOfflineChecks: 25 assertions

New feature checks cover empty informational tips, explicit metric depth parsing, seabed/stick-up datum derivation, missing/ambiguous values, header-ordered Inventory sections, retained and permanent installs, stale selections, grouped append, complete grouped returns, unavailable assessment stock, one Undo for the group, rollback on a later-member conflict, and vacating a cleared Master identity while preserving history.

The actual WPF action card is opened through the empty-cell context menu, its virtualized item button installs hardware, and removal choices are clicked through the owned modal dialog. All removal buttons remain visible while details scroll. Save preparation is visible before a deliberately pending checkpoint completes and closes after saving. A synthetic schematic resolves its shared PN model and renders a 3D Beta assembly through the exact-hash approved optional pack. Frozen geometry reuse, axes, model scale, top/bottom anchors, seabed soil placement, invalid inputs and read-only damage behavior are checked. The rendered synthetic scene was inspected visually.

Existing checked movement, duplicate consolidation, lifecycle transfer and sync, drawing references/corrections, clipboard, deletion, role backend/UI, model permissions, incremental saves, background recovery and light/dark editor tests pass. See [movement audit](Movement-Audit-1.19.21.md) for the common paths and fixes.

SDK MakeAppx packaging, archive integrity, correct manifest/version, excluded licenses/customer fixtures and the actual EXE embedded in the Store package are verified. All six offline Store pack descriptors load; the viewer renders offline and damaged executable content is rejected. Guides and all 20 languages are updated. Model geometry and assembly controls stay in the optional pack.

Owner testing against the working well drawings is pending. The beta requires review of extracted depths, common datum, model units/orientation, anchors and lateral offsets. It omits components lacking a model or confirmed depth. PDF-only drawings require manual depths; unlabelled distances are not assigned to components. Preview settings do not change project equipment data or shared original models. Microsoft Store submission remains held.

Portable SHA256: `5613b532aec98540e541c00a9cdd7d42ea1badded6fe96fe07719eb11f0f847d`

MSIX SHA256: `1b82c13c339d76fd4eee58a65aa32262579e383919d9c283014ffb7a1fe26205`
