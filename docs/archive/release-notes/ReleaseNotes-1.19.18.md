# MIE 1.19.18 — worksheet sizing candidate

Prepared for owner testing. Microsoft Store submission remains held.

- Drag a row's bottom border to resize its height. Drag a cell or column header's right border to resize the column. The pointer uses the standard vertical or horizontal sizing cursor.
- Double-click a bottom border to fit the largest content across the row. Double-click a right border to fit the header and all column contents, including items outside the viewport.
- Save the project to retain dimensions across restarts and share them through MIE packs. Size changes use the background change pipeline, respect roles/project protection, record previous and new dimensions, and support Undo/Redo. Read-only projects cannot save changed dimensions.
- Full-project XLSX and active-tab extraction preserve manual row heights and column widths. Inventory dimensions map to the particular item and displayed field, including retained linked records. Export's previous automatic sizing no longer overrides explicit sizes.
- Cleared equipment groups display one PN and one SN line. Unused blank slots no longer enlarge the row. The configured capacity remains available in Edit, so a one-PN/six-SN column still provides six serial inputs when edited.
- Normal and multi-item editor fields use the common theme surface, text and caret colors. Native equipment formatting remains preserved in stored data and Excel exports.
- Guide/tutorial help and all 20 offline language catalogs are updated. Existing approved 3D viewer and other optional modules are reused.
