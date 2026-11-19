# MIE 1.18.16

This update combines the reviewed 1.18.11–1.18.16 improvements.

- Transferred Master equipment cells show PN and SN; additional business details go to Comments. Internal application identities stay in the MIE project and are omitted from the interface and Excel reports.
- History fills the available view, supports serial search, wheel navigation, shared minus/plus zoom controls and exact event-to-log navigation. Default connectors are bold blue in dark themes and bold green in light themes.
- Printing and PDF output follow the selected tab/subtab. Graph views print their visible graph. Excel extraction includes an editable native timeline chart and event rows, and a worksheet layout preview. Excel's own font metrics and chart layout can differ from the preview.
- File → Save project as XLSX includes current worksheet and subtab choices and respects their checkboxes, including the separate linked-Schematics folder option. It exports a background snapshot so later edits remain available for the next export. PN and SN use separate lines inside combined equipment cells, with wrapping and row height set across applicable sheets. Existing separate PN/SN columns stay separate.
- Export destinations and view output formats survive restarts. Saving shows completed-work progress, closes its progress popup and closes successful view exporters. Errors leave the exporter open for correction. Export completion returns to the same MIE tab, while intentional switching to other work is respected.
- Visited tabs retain their views. Scrolling recycles viewport content, avoids unnecessary offscreen Master cells, reuses formatting and keeps glows static during scrolling. Large cold jumps through complex wrapped tables can still take longer than a frame.
- Actionable tips retain their travel grace, scroll routing and collapsed details. Their triangle follows the source cell when the card is moved to fit on screen.
- View navigation, search, clipboard targets, library extraction, schematic command availability and synchronization-audit displays match current workspaces.
- Updated guide, safe synthetic tutorial narration/playback and UI language data cover all 20 supported languages. Theme Studio continues to expose common graph, highlight, tooltip and control styling.

Existing project data, licensing terms, privacy choices and Store product identity are retained. Excel reports are presentation exports; use the MIE project to preserve complete application tracking and audit history. No operational projects, owner utilities, settings or private keys are distributed.
