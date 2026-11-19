# MIE 1.19.20 candidate validation

Prepared for owner testing; Microsoft Store submission is held.

234 targeted assertions passed across 9 suites.

- CellEditorThemeChecks: 31 assertions
- WorksheetSizingChecks: 28 assertions
- EquipmentEditorLayoutChecks: 62 assertions
- EquipmentCellRenderingChecks: 8 assertions
- EquipmentMembersChecks: 19 assertions
- WorkingPersistenceChecks: 16 assertions
- RoleUiChecks: 30 assertions
- ThemeFeatureChecks: 15 assertions
- StoreBundleOfflineChecks: 25 assertions

Editor checks inspect the rendered template background as well as control properties: grouped inputs, labels, caret and selectors must match native white worksheet cells in light and dark themes. Open editors respond to Theme Studio worksheet color overrides. Narrow-column controls remain visible. Images were rendered and visually inspected for the native white cell in dark chrome and the dark worksheet override. Row tests cover single-item and six-item fields, changing SN counts, multiline typing and restoring the original manual height on exit/cancel.

Static audit covers all cell editor factories: Master plain fields and choices, single/grouped equipment fields, shared workbook table text editors, identifier editors and schedule import choices. Shared worksheet panels cover Inventory, Quarantine, In-Order, minimum stock, Outstanding and planning worksheets; read-only tabs do not gain edit actions. Existing template bindings are now retained by the window theme pass.

Equipment rendering, history, grouped edits and background recovery regressions pass. Theme features, Studio digest verification, role UI and offline Store packs pass. The older vector-rendering harness referenced a removed private Lines field; its assertion now checks the current retained formatted text, wrapping flag and alignment.

SDK MakeAppx packaging, archive integrity, correct manifest/version, excluded licenses/customer fixtures and the actual EXE embedded in the Store package are verified. Store submission remains held for owner testing.

Portable SHA256: `93ac5a7cb155a9791deff13299a88cfe573c062dec0a306b25240ea61c0238b7`

MSIX SHA256: `871fdec4efe80aca9579e97486ec1ef9306a42e543cbb8fdf202a77ff6ffc9ab`
