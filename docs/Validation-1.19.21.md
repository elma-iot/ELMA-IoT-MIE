# MIE 1.19.21 candidate validation

Prepared for owner testing; Microsoft Store submission is held.

967 targeted assertions passed across 38 suites.

- OperationProgressChecks: 21 assertions
- WellModelResolutionChecks: 7 assertions
- TransferProgressDialogChecks: 6 assertions
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
- InventoryTransferUiChecks: 55 assertions
- ContextClipboardUiChecks: 17 assertions
- InspectionSubmissionChecks: 10 assertions
- SyncFeedbackChecks: 25 assertions
- ResponsiveSnapshotChecks: 2 assertions
- PartModelLibraryChecks: 19 assertions
- ExportWorkflowChecks: 21 assertions
- ItemViewUiChecks: 77 assertions
- WorksheetPrintChecks: 17 assertions
- PopupPlacementChecks: 12 assertions
- ExportFocusChecks: 12 assertions
- DialogFocusChecks: 33 assertions
- StoreBundleOfflineChecks: 25 assertions

New feature checks cover empty informational tips, explicit metric depth parsing, seabed/stick-up datum derivation, missing/ambiguous values, header-ordered Inventory sections, retained and permanent installs, stale selections, grouped append, complete grouped returns, unavailable assessment stock, one Undo for the group, rollback on a later-member conflict, and vacating a cleared Master identity while preserving history.

The actual WPF action card is opened through the empty-cell context menu, its virtualized item button installs hardware, and removal choices are clicked through the owned modal dialog. All removal buttons remain visible while details scroll. Save preparation is visible before a deliberately pending checkpoint completes and closes after saving. A synthetic schematic resolves its shared PN model and renders a 3D Beta assembly through the exact-hash approved optional pack. Frozen geometry reuse, axes, model scale, top/bottom anchors, seabed soil placement, invalid inputs and read-only damage behavior are checked. The rendered synthetic scene was inspected visually.

Existing checked movement, duplicate consolidation, lifecycle transfer and sync, drawing references/corrections, clipboard, deletion, role backend/UI, model permissions, incremental saves, background recovery and light/dark editor tests pass. See [movement audit](Movement-Audit-1.19.21.md) for the common paths and fixes.

SDK MakeAppx packaging, archive integrity, correct manifest/version, excluded licenses/customer fixtures and the actual EXE embedded in the Store package are verified. All six offline Store pack descriptors load; the viewer renders offline and damaged executable content is rejected. Guides and all 20 languages are updated. Model geometry and assembly controls stay in the optional pack.

Owner testing against the working well drawings is pending. The beta requires review of extracted depths, common datum, model units/orientation, anchors and lateral offsets. It omits components lacking a model or confirmed depth. PDF-only drawings require manual depths; unlabelled distances are not assigned to components. Preview settings do not change project equipment data or shared original models. Microsoft Store submission remains held.

Shared-progress refinements: all common workbook actions now use the themed footer with real completed-stage counts; unmeasured work animates and byte/work-based saves and exports keep measured percentages. Foreground activity preserves concurrent save/sync measurements. Legacy stock-selection and receipt dialogs execute on the worker. New snapshot preparation measured about 4 ms on the synthetic regression fixture.

Popup placement is shared by WPF dialogs and real native Windows Save As dialogs. Tests cover nested ownership, undocked workspace routing from a main-window fallback, session-only manual moves, fresh-process reset and close/foreground behavior. Native initialization resizing is handled; the installed monitor work area is respected. Dock/undock placement remains unchanged. A physical mixed-DPI multi-monitor check is conditional on monitor availability.

Original model filename candidates are offered in 3D Beta for review when precise registered PN models are absent; no PN alias is created and Include stays off pending confirmation. The owner project was inspected read-only and remained byte-identical. Exact PN matching and independent serial damage storage retain their regression checks. New labels have all 20 catalog translations and matching core fallbacks. See Progress-and-model-lookup-1.19.21.md for the refinement audit.

Portable SHA256: `2df67de61e10cd3608ebad391eb56da3d827a5b46d24217e165d0cd8220945bb`

MSIX SHA256: `ca91bda14d4aa1861d3920a3b126bf081a5f0541b62e9ee257a9b4a91141eab0`
