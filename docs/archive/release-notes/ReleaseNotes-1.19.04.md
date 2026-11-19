# MIE 1.19.04 — dialog focus and inspection retry

Portable review in the 1.19 series. Version 2.0 and Microsoft Store submission remain on hold.

- A shared dialog close policy returns Accept, Cancel, Enter, Escape and title-bar closes to the owning MIE window. Nested popups return to their immediate parent. Help, placement previews, exporters and detached workspaces use the same policy. Optional viewer windows receive the rule from the host application without downloading a replacement pack. Startup and noninteractive drag/tutorial overlays keep their existing behavior.
- File pickers use the active application popup rather than a covered main window. Color and folder selectors have explicit owners where missing, including Theme Studio's color picker. Background completion preserves another application that the user deliberately selected. Cancelled closes leave the popup active.
- Inspection review now explains outstanding prerequisites before approval. A photo provides evidence but does not record a passed test. When testing is required, complete the test and explicitly select **Record Test / Certification**. Repair, BER assessment and physical-return restrictions remain enforced.
- Submission keeps the inspection form open while applying changes in the background. A rejected operation shows its error inside the form and retains notes, selected documents and newly attached file paths. Correct the issue or cancel without starting over. A successful operation closes only the form and restores its actual parent window. Failed transactions record no partial inspection or release.
- The guide, tutorials and new wording are updated in all 20 application languages. Existing optional executable packs remain unchanged.

Verification covers native foreground focus, nested and modal dialogs, keyboard and title-bar closes, cancelled Closing events, background completion, exporter progress, responsive failed-form retry and actual inspection submissions with photo evidence. The inspection checks include a stale-record conflict, no partial history on failure, retained evidence and successful approved release with passed tests. Session and Item View regression checks cover detached windows, previews and exports.

Portable executable: `build/MIE Portable.exe`. [Guide and language data](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v43).
