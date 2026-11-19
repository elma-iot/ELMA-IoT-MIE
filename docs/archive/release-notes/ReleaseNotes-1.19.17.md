# MIE 1.19.17 — release candidate

Prepared for owner testing. Do not submit this candidate to Microsoft Store until the owner approves it.

- Equipment column creation offers Previous, Next and Last placement, plus independent PN and SN counts (one of each by default; up to six). Right-click Edit changes the counts and PN assignment for each SN in an existing Master equipment cell.
- Inventory installation into an occupied well cell offers Replace, Append and Cancel. Append places the incoming SN under its matching PN, keeping the existing items. The backend refuses a seventh item without changing either location.
- Each SN retains an independent equipment identity, lifecycle, documents, model annotations and history. Its cell submenu provides individual history, Item View, return and Quarantine actions, subject to the licensed role. A retained Inventory row refers to that individual member.
- Delete on the Master equipment cell clears every PN and SN together. Undo restores the complete group. Deleting an individual linked Inventory record affects only its member. Before/after values remain in history. Copy/Paste preserves assignments with new identities; Cut/Paste retains the existing identities.
- The drag preview now captures grid-local content without the toolbar/layout offset. This removes the empty strip above captured headers and aligns the outlined drop target and floating header. Pointer height does not move the target vertically. Holding either edge starts scrolling gently and accelerates, then slows near the limit for precision. Neighboring columns catch up with the preview; both the first movable position and the final position are reachable.
- Column creation and layout commits use the existing background change pipeline. Newly inserted blank well rows discard equipment-group metadata from their formatting template.
- Duplicate checks compare each SN and describe its actual entered identifier, including leading zeroes. Identifiers beginning with PN- or SN- are preserved by the equipment parser.
- Excel reimport accepts gaps explicitly marked as hidden internal columns while continuing to reject invalid visible headers. Internal equipment identities are also removed from grouped-cell export metadata.
- Guide and tutorial help and offline UI catalogs updated in all 20 supported languages. New equipment-group projects declare MIE 1.19.17 as their minimum reader version.

Local release folders retain the flat layout: version-stamped test EXE, Store MSIX, notes and a compatible previous license when available. Owner Tools remains at the project root. Previous releases are preserved.
