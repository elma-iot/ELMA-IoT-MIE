# ELMA-IoT MIE 1.18.10

This release includes the Inventory, history, theme and responsiveness improvements reviewed in 1.18.2–1.18.9, with updated user guidance and tutorials in all 20 supported languages.

- Inventory uses recycled cells and static decorations during scrolling. Duplicate tips open on demand and keep working action buttons, scrolling and expandable details.
- Unticked removal retains one linked, orangish Inventory row at its original position. Installed equipment stays unavailable until returned; inspection and release rules still apply. Permanent transfer removes the section placeholder.
- Same-serial transfers use the Inventory PN, record the previous value, and correct linked editable schematics using reviewed source references. Updated drawings offer a choice to retain their PN or use the corrected installed PN. Ambiguous drawings retain an explicit note.
- Undo and Redo remain in the header before Sync, available across tabs. Destination navigation focuses and briefly highlights the actual installed cell.
- Equipment history loads asynchronously, with SN search, location lanes and horizontal time navigation. Right-clicking an event opens and highlights its exact full-log record.
- Excel extraction preserves current visible rows/columns, installed-row styling, exact identifiers, dates, quantities and standard cell Notes. Timeline exports include the graph and selected equipment events.
- Theme Studio includes shared controls, subtabs, timeline/schedule lines, glows, installed-row colors and tooltip styling, with light/dark contrast validation.
- Background save, backup and sync snapshots avoid repeated metadata serialization, retain later edits, and reuse unchanged resources incrementally where applicable. Lifecycle cache reads remain isolated and integrity checked.
- Startup reports real loading stages, uses the chosen theme and runs its logo animation independently. Invalid or wrong-PC portable license files produce a recurring notice; OK keeps the application open with the appropriate free-feature state.
- Updated guide topics and synthetic tutorials cover installations, global Undo/Redo, interactive tips, timeline/log navigation, appearance and background work. Translation checks cover text, placeholders, URLs, Unicode and source hierarchy in all 20 languages; imported project data remains untranslated.

Windows 10/11 x64, .NET Framework 4.8. Excel is needed for editable XLSX schematic import/rendering. Optional language and guide data download on demand and work offline afterward. Store executable modules are included in the MSIX and are not downloaded as code updates.

The Store candidate is prepared for the existing listing. Certification submission and approval are separate states; preparation alone does not publish the Store update. No customer project, license file, signing key or owner utility is included.
