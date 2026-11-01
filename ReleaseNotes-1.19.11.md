# MIE 1.19.11 — current-tab search and audited replacement

Release candidate for owner testing. Not submitted to Microsoft Store; the existing submission remains unchanged.

- Ctrl+F opens the search popup for the current tab and selected History or Schedule subtab, including detached windows. The header search retains its cross-tab scope.
- More options expands case, whole-word and regular-expression controls, using the application theme. Enter/Next moves forward; Shift+Enter/Previous moves backward.
- Editable tables support Replace and Replace All in both View and Edit modes. Ctrl+H opens replacement controls. Edits run through the background transaction pipeline and retain old/new values in history with grouped Undo.
- Read-only logs, graphs and calculated/document views remain search-only. Protected application identifiers are preserved during replacement.
- Search scrolls to and focuses the matching row/cell. A temporary theme-controlled highlight clears when search closes. The focused row remains below the popup, including its expanded controls; long options scroll within the popup.
- Guides, tutorials and all 20 language packs updated. Native PN-shared models, serial-specific documents/damage and incremental resource reuse are retained.

Validation: all 12 tabs, every full-history and schedule subtab, search/replace in View and Edit modes, audited old/new values, Undo, expanded-popup row visibility, highlight cleanup, regex validation, existing search tutorials in all 20 languages and header search regression.
