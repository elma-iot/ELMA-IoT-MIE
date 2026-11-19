# MIE 1.19.20 — consistent cell editing and automatic edit sizing

Prepared for owner testing. Microsoft Store submission remains held.

- Normal and grouped equipment editors use the worksheet cell's display colors instead of mixing dark window inputs with light cell backgrounds. PN/SN labels, input text, carets and selectors remain readable in light and dark themes.
- Fixed the window theme pass repainting input-template backgrounds after their field colors were resolved. Dropdown arrows now follow the field text color.
- Shared table editors retain display formatting across Inventory, Quarantine, In-Order, minimum-stock, outstanding and editable planning worksheets. Master choice editors use the same cell colors. Section-title carets follow their text.
- Native worksheet colors remain intact. Theme Studio worksheet color and typography overrides apply to open equipment editors.
- Editing temporarily grows the row for every field and wrapped line. Adding or removing serial fields adjusts the height immediately. Ending or cancelling an edit restores the saved row height. Narrow columns wrap PN/SN count controls instead of clipping them.
- No project schema or equipment data changes. Existing role controls, background working recovery and incremental saves are retained.
- User guide, tutorials and all 20 languages updated. Existing approved viewer modules reused.
