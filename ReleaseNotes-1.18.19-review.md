# MIE 1.18.19 — equipment editing review

- Moving an Inventory item to Quarantine also clears its unique matching Master Installed cell, including older records without an equipment identity. Inventory's part number remains authoritative. Both locations, the acting user and the reconciliation reason remain in history; one Undo restores the whole operation. Multiple installed matches require review before the move.
- For an item already in Quarantine with a stale installed duplicate, right-click it and choose **Send to Quarantine…** to confirm the action. Its previous inspection evidence is preserved.
- Combined equipment editors always display PN and SN and expand the active row to fit both inputs. Finishing or cancelling editing restores the compact row height. Separate stock identifier columns remain available in edit mode.
- Enable **Edit**, then right-click an equipment cell and choose **Delete** to clear PN and SN together. Inventory, Quarantine and In-Order provide the same action from either identifier column. Comments and other details are preserved. The action is logged and supports Undo/Redo. Read-only, formula, disposed and linked-location records retain their existing editing restrictions; use the current physical record for linked rows.

Quick check: edit a test equipment cell, delete its identifiers, inspect Full history, then Undo and Redo. Quarantine a duplicated Inventory item and confirm its former well cell clears. Use a copy of operational data for this check.

Verification covers native records in all four equipment views, comment preservation, revision audit entries, stale-command rejection, atomic undo/redo, actual context-menu enablement, PN/SN editor layout in light/dark themes at 70% zoom, legacy and registered duplicate reconciliation, retained/removed Inventory records, save/reopen and ambiguous-match rejection. Existing translated Delete and routing labels are reused; no new interface translation keys were added.

Portable 1.18.19 is prepared for review in the build folder. The existing 1.18.18.0 Store submission is separate; this review has not been submitted to Microsoft Store.
