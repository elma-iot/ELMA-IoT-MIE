# MIE 1.19.03 — inspection defaults and image controls

Portable review in the 1.19 series. Version 2.0 and Microsoft Store submission remain on hold.

- Actual action date and Reason are optional in inspection review and lifecycle forms. A blank date uses cached verified internet time when available, otherwise the PC clock, without waiting for a network request. A blank reason records the reviewer and selected decision. Entered dates and notes are preserved.
- History records whether the reason was generated and which date source was used. Evidence, required tests, named approval and future-date checks remain enforced. Failed reviews leave the project unchanged.
- Attached images initially fit the right preview pane. Use the mouse wheel to zoom around the pointer, drag with the left or middle mouse button to pan, and use Fit, + and − controls. Double-click also restores the complete image. Preview transforms reuse the decoded image; original attachment files remain unchanged.
- The guide, tutorials and interface wording are updated in all 20 application languages. Existing signed viewer components are unchanged.

Verification covered automatic and manual dates/reasons, audit provenance, approval/testing/evidence restrictions, responsive image controls, attachment retention, PDF preview, optional 3D viewing and Item View exports. The actual inspection form was also exercised with a blank date and existing notes.

Portable executable: `build/MIE Portable.exe`. [Guide and language data](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v42).
