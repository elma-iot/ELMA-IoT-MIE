# MIE 1.19.28 — cut-view performance and complete project merge

Release candidate for owner testing. Microsoft Store submission remains on hold until testing is complete.

## Smooth cut-view navigation

Fixed repeated assembly-bounds calculations in the Schematics 3D Beta cut view. On the measured 15-component saved assembly, cut-view CPU camera updates decreased from 247 ms to 1.36 ms, and measurement-frame calculation from 248 ms to 0.47 ms. These are CPU timings, not a GPU FPS guarantee. Geometry, section caps, contour anchors and measurement detail are preserved; completed before/after captures are byte-identical.

## Complete native project merge

- Review conflicting equipment assignments: transfer as-is with warnings, exclude incoming conflicting cells and merge the rest, or cancel.
- Compare populated current/imported values, tab names and cell addresses, with expandable full-cell contents. Review windows remain movable above the application while tab navigation stays available.
- Transfer shared 3D models even when no worksheet cells changed. Include saved seabed-constructor hierarchy, depths, offsets, model selections, connections, motion and dimensions under the matched well drawing.
- Place imported custom equipment columns beside their source neighbours, retain grouped PN/SN membership and remap constructor references to the destination column identities.
- Refresh the live table, stock tabs, Item View and open constructor after merging without Save or restart. One Undo restores the complete reviewed merge.
- Updated guides, tutorial captions and interface/learning catalogs in all 20 languages.

Existing authorization, identity/formula reconciliation, controlled disposal protections and synchronization rules remain in force. Import comparison does not rewrite either input pack.

Portable and Store packages, approved offline optional content and SHA-256 checksums accompany this candidate. The Store package has not been uploaded or submitted.
