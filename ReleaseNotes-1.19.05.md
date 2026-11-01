# MIE 1.19.05 — scrolling tips and Store release candidate

Prepared for owner testing. Microsoft Store upload and submission remain on hold.

- Scrolling a worksheet with the wheel, keyboard or scrollbars immediately dismisses its information and action tips. Tips remain suppressed beneath a stationary pointer after the table stops. Deliberate pointer movement after a 300 ms quiet interval permits a fresh hover using the existing display delay. Recycled cells and layout changes cannot rearm tips by themselves.
- The policy is shared by all DataGrid worksheets and does no cell enumeration or recurring timer work. Scrolling inside an actionable tip remains independent of worksheet scrolling, preserving its persistent hover, checkbox, details and action controls.
- Retains 1.19.04's common popup owner-focus policy, actionable inspection prerequisites, retained evidence and failed-form retry. See [1.19.04 review notes](ReleaseNotes-1.19.04.md).
- Current guides, tutorials and all 20 language catalogs remain available in the immutable [approved language and learning release](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v43). No new interface strings or translation changes are needed for this behavior-only patch. Existing signed 3D/game packs remain compatible and verified.
- The Store candidate includes the matching Theme Studio companion, verified against the digest embedded in MIE, alongside the approved bundled module catalog. Store executable content remains local; only approved language/learning data downloads on demand.

Verification covers tip dismissal on actual offset changes and wheel input, stationary-pointer suppression, deliberate hover recovery, action-tip controls and scrolling, smooth-scrolling behavior, 20-language guide rendering and translated tutorial playback. Store candidate preparation includes offline module checks and MakeAppx validation. The validated candidate is held privately pending owner testing and authorization.

Portable executable: `build/MIE Portable.exe`. Store application version: 1.19.05; numeric MSIX version: 1.19.5.0.
