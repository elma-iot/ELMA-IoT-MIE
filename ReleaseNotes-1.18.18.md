# MIE 1.18.18

- Vertical scrollbar dragging uses WPF's native offset command without a competing replay of the previous position. Repeated drags advance the table and releasing the thumb preserves its final position.
- Master Installed reserves a measured header band across all visible columns, including columns outside the viewport. Refreshed workbook rows and header sizing are updated before transfer navigation. Heading text follows the current theme.
- Excel reports open at the beginning with an explicit selection in the scrolling pane and no conflicting worksheet-level opening offset. This prevents Excel from initially painting row 1 twice despite reporting the correct pane position. The affected workbook reproduced the issue; a copy with the conflicting offset removed was confirmed to open with one header. Frozen rows/columns remain fixed; stale imported split-window state is removed. Fresh Inventory, Master Installed and Revision History exports were checked in Microsoft Excel before and after scrolling.
- Moving Inventory equipment to Quarantine removes the vacated row when removal is selected. Retention preserves the linked row at its original position. Undo/redo, movement logs and save/reopen preserve the selected behavior. Vacated Quarantine slots are suppressed when items return.

Regression checks cover light/dark Master headings at 70% zoom, reordered destination columns, transfer focus/highlighting, virtualized scrolling, retained/removed Quarantine rows, partial quantities, lifecycle evidence and audit logs. Tests on the supplied MIE project use a disposable copy; the original remains byte-identical. No interface wording changed, so the existing translated guides and tutorials remain applicable.

The corrected 1.18.18 build replaces the earlier portable review. Its Store package is prepared for submission; confirmed Store status is recorded in ApplicationNotes.md. Existing signed content packages are reused without changing their published bytes.
