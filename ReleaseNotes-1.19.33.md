# MIE 1.19.33 — master-driven 3D construction and direct cell editing

- Construct wells directly from Master Equip. list data without uploading a 2D schematic. Cancel the import picker, select 3D Beta and configure the existing attached PN models. Saved 3D-only configurations reopen directly in 3D.
- Make 2D schematics saves the complete portrait 3D print view and equipment table as a project drawing. Leaving a configured 3D-only well asks Yes/No; No retains its editable 3D configuration. Saving the 2D snapshot immediately links and underlines the master well name.
- Generated drawings retain the editable 3D settings, work in normal schematic viewing/export, and support Undo/Redo. 3D-only drafts are excluded from XLSX schematic exports.
- Double-click an editable Master Equip. list data cell to enable edit mode and edit that cell. Clicking another data cell commits the current value and opens the next editor.
- NA and N/A in serial fields mean not available, show a translated hover explanation, and are excluded from duplicate serial checks. Entered text survives save/reopen. Real repeated serials retain their warnings.
- A scoped .NET Framework 4.8 accessibility workaround removes only orphaned editing-column trackers before commit/cancel, avoiding the null-element popup during focus changes and editing-mode changes. Normal accessibility remains enabled.
- Unavailable serials in multi-item cells retain separate positional identities.
- Includes the reviewed well cut-view scanner, water-mask consistency and seabed projection fixes.
- Updated user guide and editing/tutorial guidance in all 20 languages.

Prepared for owner testing. Store submission remains pending owner validation. Original project files and GLB geometry are preserved. Terrain/contact deformation remain illustrative previews.
