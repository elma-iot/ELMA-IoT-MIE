# MIE 1.19.16 prepared update

See [release notes](ReleaseNotes-1.19.16.md), [validation](Validation-1.19.16.md) and the updated [user guide](UserGuide.txt). Includes live 3D model badges, transparent dials, revised viewer/pallet controls, safe minimum-stock policy removal, centered About and Full Control header customization with license fallback. All 20 languages and 80 new guided-example runs are validated. Local packages and download assets are prepared; no 1.19.16 Store submission has been made.

The records below describe previous updates.

## MIE 1.19.11 Store submission

Submitted to Microsoft Store as **Submission 15**. Partner Center confirms **In certification / Pre-processing**, with automatic publication after certification passes. [Submission record](StoreSubmission-1.19.11.md). The preparation/owner-testing holds below are historical.

# MIE 1.19.11 — current-tab search and audited replacement

Release candidate for owner testing. Not submitted to Microsoft Store; the existing submission remains unchanged.

- Ctrl+F opens the search popup for the current tab and selected History or Schedule subtab, including detached windows. The header search retains its cross-tab scope.
- More options expands case, whole-word and regular-expression controls, using the application theme. Enter/Next moves forward; Shift+Enter/Previous moves backward.
- Editable tables support Replace and Replace All in both View and Edit modes. Ctrl+H opens replacement controls. Edits run through the background transaction pipeline and retain old/new values in history with grouped Undo.
- Read-only logs, graphs and calculated/document views remain search-only. Protected application identifiers are preserved during replacement.
- Search scrolls to and focuses the matching row/cell. A temporary theme-controlled highlight clears when search closes. The focused row remains below the popup, including its expanded controls; long options scroll within the popup.
- Guides, tutorials and all 20 language packs updated. Native PN-shared models, serial-specific documents/damage and incremental resource reuse are retained.

Validation: all 12 tabs, every full-history and schedule subtab, search/replace in View and Edit modes, audited old/new values, Undo, expanded-popup row visibility, highlight cleanup, regex validation, existing search tutorials in all 20 languages and header search regression.

# MIE 1.19.10 — shared original models

Release candidate for owner testing. Microsoft Store submission is on hold; 1.19.09 remains in certification.

- Upload an original GLB once: it appears in Item View for every item with the same part number, including items added later. Shared originals are labelled in the attachment list.
- Only the original model is shared. Documents, custom textures, damage marks, deformation and scene settings remain specific to the individual item. Existing GLB uploads are recognized automatically.
- Native projects retain one content-addressed original. Incremental saves reuse its compressed entry; incremental sync sends new resources without resending unchanged model bytes. Backups retain the same association.
- Selected-item exports include the shared original without another item's documents or damage. Merge preserves the latest active damage and immutable historical checkpoints.
- Returning an item clears its active damage while preserving its history and scene preferences. Other serials remain unchanged.
- Header search by SN, PN or description runs only on Enter or Search. All matches appear in a scrollable dropdown with the tab name; selecting a result collapses it and focuses the destination row. Searches run in the background with cancellation and safe project-change handling.
- Search results resize to the number of matches, up to 20 visible rows. Additional matches use the common theme scrollbar. The magnifier is embedded at the right of the field; height and border style match the header buttons.
- Updated guide, tutorials and all 20 language packs.

Validation: shared-PN lookup, legacy uploads, serial isolation, incremental resource selection, native save/reopen and backups, scoped exports, model checkpoint merge, return/undo/redo, inspection documents and save workflows.

# Application notes

Current portable review and local Store candidate: **1.19.09** separates paint UVs from model textures, uses left/right deformation and saves editing sessions asynchronously. A soft circular CAD-style floor adds separate shadow and optional model reflection. Failed checkpoints remain recoverable. [Review notes](ReleaseNotes-1.19.09.md). Guides/tutorials and all 20 languages are updated. Submitted to Microsoft Store as **Submission 14**, in certification/pre-processing with automatic publication after approval. [Submission record](StoreSubmission-1.19.09.md).

Previous portable review and local Store candidate: **1.19.08** places the model filename beside Settings and adds live brush/deformation footprints, indexed surface picking, cached decals and coalesced incremental background deformation. [Review notes](ReleaseNotes-1.19.08.md). Store upload/submission remain held.

Previous portable review and local Store candidate: **1.19.07** fixes textured cut restoration and adds solid section surfaces, shaded double arrows, perspective/orthographic overlays, contextual brush controls and an icon toolbar. All viewer implementation remains in the optional pack. [Review notes](ReleaseNotes-1.19.07.md). Guide/tutorials and 20 languages updated. Store upload/submission remain held.

Previous portable review and local Store candidate: **1.19.06** updates the optional 3D pack with pointer zoom, item-specific settings, texture mapping/wrapping, damage marking and reversible Raise/Lower deformation. Return to Inventory clears active damage and retains its historical checkpoints plus scene settings. [Review notes](ReleaseNotes-1.19.06.md). Guides, tutorials and all 20 languages are updated. Store upload/submission remain held for owner testing.


Previous portable review and local Store candidate: **1.19.05** dismisses/suppresses worksheet tips during scrolling until the pointer deliberately moves again. Current guides, translations and optional content are verified; the Store candidate includes the paired Theme Studio and approved offline modules. [Review notes](ReleaseNotes-1.19.05.md). Upload/submission remain on hold pending owner testing.

Previous portable review: **1.19.04** applies a shared owner-focus rule to dialogs, corrects nested file-picker ownership, explains inspection release prerequisites and retains the form and evidence on failed submission. [Review notes](ReleaseNotes-1.19.04.md). Not submitted to Microsoft Store.

Previous portable review: **1.19.03** adds optional inspection date/reason defaults with audit provenance and fitted image previews with wheel zoom, drag-to-pan and Fit / + / − controls. [Review notes](ReleaseNotes-1.19.03.md). Not submitted to Microsoft Store.

Previous portable review: **1.19.02** adds concise Quarantine action tips and Item View lifecycle controls. [Review notes](ReleaseNotes-1.19.02.md). Inventory retains its detailed tips. Not submitted to Microsoft Store.

Previous portable review: **1.19.01** adds the half-height attachment area, remembered divider, aligned Upload button and per-file Save as menu. [Review notes](ReleaseNotes-1.19.01.md). Not submitted to Microsoft Store; version 2.0 is deferred.

Previous portable review: **1.19.00** adds inspection proof, licensed Item View, on-demand 3D controls and draggable hatched X/Y/Z sections, offline pack import and preserved identifier formatting. [Review notes](ReleaseNotes-1.19.00.md). This version has not been submitted to Microsoft Store.

Previous portable review: **1.18.21** corrects returned Inventory assessment visibility and navigation. See [review notes](ReleaseNotes-1.18.21.md). This patch is not yet submitted to Microsoft Store.

Current release: **1.18.20**. [Clipboard, deletion and cell-history changes](ReleaseNotes-1.18.20.md). Portable and Store package validation, regression checks and all 20 translated tutorial playbacks passed. The portable release is published privately. Microsoft Store **Submission 13** (`1152921505702288513`) is **in certification**, with Submission complete and Pre-processing in progress. Publication is automatic after approval; availability of 1.18.20 remains pending. Confirmed Store status is recorded in STORE-RELEASE.md.

Previous release: **1.18.19**. [Equipment editing guide and changes](ReleaseNotes-1.18.19-review.md). Partner Center confirmed on **1 November 2026** that **Submission 12** (`1152921505702288457`) is live in Microsoft Store.

The corrected **1.18.18** build replaces the earlier portable review and fixes the doubled Excel heading on first open, table headings, scrollbar dragging and Inventory/Quarantine row handling.

The private repository contains source and portable builds. The public project contains documentation, approved optional-content releases and the Microsoft Store link. Operational data, licensing keys and owner utilities are excluded from releases.

Historical submission record: version **1.18.18.0** was submitted on **1 November 2026** as Submission 11 (`1152921505702288179`). Partner Center confirmed **Update in certification**, Submission complete and Pre-processing in progress. The validated package, English release notes and reviewer instructions are updated. Publication is automatic after certification; approval and public availability of this update remain pending. At that observation the overview identified Submission 10 as the existing Store presence. On 1 November, the 1.18.19 submission overview confirmed Submission 11 is live.

Portable **1.18.18** is published in the private GitHub release. Approved signed optional content remains at v36. Save/export focus, workflow, native Excel cell lines, guide/tutorial playback and all 20 language catalogs were checked for the preceding content release; this patch adds no interface text. Actual public language and guide downloads passed their application-approved digest checks and remain usable offline. Store executable modules remain bundled and passed offline verification in 1.18.18.
