# Microsoft Store release

## MIE 1.19.11 submitted

Submitted to Microsoft Store as **Submission 15**. Partner Center confirms **In certification / Pre-processing**, with automatic publication after certification passes. [Submission record](StoreSubmission-1.19.11.md). The preparation/owner-testing holds below are historical.

## MIE 1.19.11 local candidate — 1 November 2026

Prepared for owner testing; **not uploaded or submitted to Microsoft Store**. Package `1.19.11.0 x64`, 26,204,540 bytes, SHA-256 `aa18faeb36716911f530bdc58eccf0bb70dd206f3ca6943eeaa5c903fa0da238`. No existing Partner Center submission was changed.

Ctrl+F searches the current tab/subtab in a common themed popup with expandable case/whole-word/regex options. Ctrl+H and Replace/Replace All work in View and Edit modes on editable tables, through background transactions with old/new history and Undo. Find scrolls and focuses the matching cell with temporary highlighting, cleared on close; the row stays below even expanded controls. Read-only views remain search-only. [Release notes](ReleaseNotes-1.19.11.md).

Guides, tutorials and 20 translations are updated in [mie-content-v49](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v49). Validation includes all 12 tabs, History and Schedule subtabs, background replacement from both modes, history and Undo, popup clearance, highlight cleanup, regex errors, all 20 search tutorials, header search, Item View and offline module/tamper checks. Evidence: `.audit/finalfind11911.log`, `.audit/tabfind11911.log`, `.audit/searchreplace11911.log`, `.audit/offlinefind11911.log`, `.audit/boundedfind11911.log` and `.audit/Store-1.19.11/candidate.json`.

## MIE 1.19.10 local candidate — 1 November 2026

Prepared for owner testing; **not uploaded or submitted to Microsoft Store**. Package `1.19.10.0 x64`, 26,198,542 bytes, SHA-256 `f711d86c0808954f55fb3f4a9ee2a4075583a7b9e42c13a91e709c467a4b9f9f`. 1.19.09 Submission 14 remains in certification.

Includes one shared original GLB per PN, serial-specific documents and damage, immutable checkpoints and incremental resource reuse. The header search uses an embedded lens, matching header-button height/frame, Enter or click activation and a virtualized scrollable dropdown with direct row navigation. The result frame grows to at most 20 rows and shrinks for fewer matches; overflow uses the common theme scrollbar. Guides/tutorials and 20 language packs are updated. [Release notes](ReleaseNotes-1.19.10.md).

Checks: shared original/model isolation, two-PC model damage merging, return/undo/redo, native incremental saving, selected-item export, global search including 1,200 untruncated results, theme colors, Item View UI, all language bundles, incremental sync, inspection documents, save workflows and offline Store modules/tamper protection. Evidence: `.audit/modelsync11910.log`, `.audit/finalmodel11910.log`, `.audit/sharedchecks11910.log`, `.audit/finalshared11910.log`, `.audit/globalsearch11910.log`, `.audit/candidatechecks11910.log`, `.audit/offlineshared11910.log` and `.audit/Store-1.19.10/candidate.json`.

## MIE 1.19.09 submitted - 1 November 2026

The owner authorized submission. Partner Center confirms **Submission 14: In certification**, currently **Pre-processing**, for package **1.19.9.0 x64**. Publication is automatic as soon as certification passes. The Store description, release notes, Item View feature entry and reviewer instructions are updated. [Submission record](StoreSubmission-1.19.09.md). The preparation records below are historical; the owner-testing hold has been lifted.

## Version 1.19.9.0 - local candidate, held for owner testing, 1 November 2026

Display **1.19.09**; do not upload to Partner Center or submit until owner approval. Package: `dist/store/ELMA-IoT-MIE_1.19.9.0_x64.msix`, **26,178,430 bytes**, SHA-256 `c4a8ffaf0692bd5f1d78f13ed2824020696ebde9b749f3ed17ddff7fcf8ceadf`. Identity, publisher, architecture and permissions remain unchanged.

The optional 3D pack provides independent paint UVs, left/right deformation, deferred asynchronous editing checkpoints and a CAD-style circular floor with separate contact shadow and model reflection. Reflection is a native planar approximation with automatic fallback for software rendering and scenes above 200,000 displayed triangles. Store executable modules are bundled and verified. Portable packs use [mie-content-v47](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v47), with Browse pack fallback.

[Review notes](ReleaseNotes-1.19.09.md), [Store notes](StoreReleaseNotes-1.19.09.txt), [reviewer instructions](StoreReviewerNotes-1.19.09.txt). Evidence: `.audit/sessionchecks11909.log`, `.audit/finalchecks11909.log`, `.audit/languagechecks11909.log`, `.audit/tutorialdiagnostics11909.log`, `.audit/offline11909.log` and `.audit/Store-1.19.09/candidate.json`. Checks cover rendered paint over remapped textures, no idle writes, quiet session commit, failed large-window recovery, damage/history, input, exports, dialogs, all 20 guide/tutorial languages and offline/tamper validation. No Store submission has been changed.

## Version 1.19.8.0 - local candidate, held for owner testing, 1 November 2026

Display **1.19.08**; do not upload to Partner Center or submit until owner approval. This local review replaces the previous candidate. Package: `dist/store/ELMA-IoT-MIE_1.19.8.0_x64.msix`, **26,165,102 bytes**, SHA-256 `17f078afd08698434a902f7b7e2fb549b799b14c584eae8fe9e16d2809f11fd1`. Identity, publisher, architecture and permissions are unchanged.

The separately verified 3D pack puts the filename beside Settings, adds live surface-projected marking/deformation footprints and uses indexed picking, local cached decals and incremental/coalesced background deformation. Previews do not modify equipment or history. Original models and audited damage history remain preserved. Store modules are bundled and verified; portable modules use [mie-content-v46](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v46), with Browse pack fallback.

[Review notes](ReleaseNotes-1.19.08.md), [Store notes](StoreReleaseNotes-1.19.08.txt), [reviewer instructions](StoreReviewerNotes-1.19.08.txt). Evidence: `.audit/previewchecks11908.log`, `.audit/uichecks11908.log`, `.audit/tutorialchecks11908.log`, `.audit/offline11908.log` and `.audit/Store-1.19.08/candidate.json`. Dense synthetic-mesh performance checks cover surface preview, local triangle queries, cached stamps, queued-work retention and UI responsiveness. Guides/tutorials and all 20 languages are updated. No Store submission has been changed.

## Version 1.19.7.0 - local candidate, held for owner testing, 1 November 2026

Display **1.19.07**; do not upload to Partner Center or submit until the owner authorizes it. This local review replaces the previous candidate. Package: `dist/store/ELMA-IoT-MIE_1.19.7.0_x64.msix`, **26,158,443 bytes**, SHA-256 `dc3d7e3257f34b08ca302e13806d28396af901b6b2834ee1528da632637ffa3d`. Existing identity, publisher, architecture and permissions are unchanged.

The separately implemented 3D pack restores textured cut views, removes section patterns, adds a shaded movement arrow and provides perspective/orthographic and brush overlays. Store executable modules are bundled and digest-verified. Portable content uses [mie-content-v45](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v45), with local Browse pack fallback. Updated 20-language guides/tutorials and signed assets accompany this review.

[Release notes](ReleaseNotes-1.19.07.md), [Store notes](StoreReleaseNotes-1.19.07.txt), [reviewer instructions](StoreReviewerNotes-1.19.07.txt). Evidence: `.audit/Store-1.19.07/candidate.json`, `.audit/offline11907.log`, `.audit/finalchecks11907.log`, `.audit/viewertests11907.log` and `.audit/sectionchecks11907.log`. The live Store release has not been modified.

## Version 1.19.6.0 - local candidate, held for owner testing, 1 November 2026

Application display version **1.19.06**. **Do not upload to Partner Center or submit** until the owner explicitly authorizes it. This preparation creates or modifies no Store submission and supersedes the earlier local 1.19.5.0 candidate for review. Historical submission observations below were not reverified.

Candidate: `dist/store/ELMA-IoT-MIE_1.19.6.0_x64.msix`, **26,154,296 bytes**, SHA-256 `853808beb449a047c896d100bd9c48824e055bb85fa58c5a2571f2b90e403b86`. Existing product identity, publisher, x64 targeting and permissions are unchanged. MakeAppx and payload checks verify the executable, matching Theme Studio, signed catalog and four approved executable modules. Customer projects, owner utilities and optional data ZIPs are excluded.

All rendering, texture, marking, deformation and viewer-history tools remain in the optional 3D assembly. Store executable modules are bundled and verified; portable installations obtain the approved pack from [mie-content-v44](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v44), with Browse pack fallback. Languages and guide/tutorial data are pinned by exact hashes and remain usable offline after installation. Viewer, annotation return/undo/save, inspection, PDF/Excel, guide rendering and translated tutorial checks passed. Offline Store checks cover real GLB loading, bundled tools, classic games and tamper rejection. Verification machine: WPF rendering tier 2; no per-vendor hardware benchmark is claimed.

Prepared material: [review notes](ReleaseNotes-1.19.06.md), [Store release notes](StoreReleaseNotes-1.19.06.txt), [reviewer instructions](StoreReviewerNotes-1.19.06.txt). Evidence: `.audit/Store-1.19.06/candidate.json`, `.audit/Store-1.19.06/offline-checks.log`, `.audit/Release-1.19.06/final-validation.log` and `.audit/Release-1.19.06/release-checks.log`. Pricing, licensing, availability and privacy declarations are unchanged. The live Store release is unaffected.


## Version 1.19.5.0 - local candidate, held for owner testing, 1 November 2026

Application display version **1.19.05**. **Do not upload or submit** until the owner explicitly authorizes it after testing. No Partner Center submission was created or modified during this preparation. Older submission entries below are historical observations and were not reverified for this candidate.

Candidate: `dist/store/ELMA-IoT-MIE_1.19.5.0_x64.msix`, **26,076,679 bytes**, SHA-256 `1cb4f51f6cab87ca73c49044ad6d9c30497511b19173609cca981f78df1b84e3`. Existing product identity, publisher, x64 targeting and permissions are retained. MakeAppx validated the unsigned Store-upload package; payload verification confirms the candidate executable, its digest-matched Theme Studio companion, approved catalog/four executable modules and shell assets. Customer projects, owner tools and optional language/learning ZIPs are excluded from the MSIX.

Current approved language/learning data is published at [mie-content-v43](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v43), pinned by exact hashes in the app and available offline after installation. Existing signed viewer/game modules are reused because they remain compatible. Store checks cover on-demand data verification, offline executable loading, classic games, real GLB viewing, launching the paired Theme Studio and rejecting damaged executable content. Portable checks cover scrolling tips, existing action tips, translated guide rendering and tutorial playback. Evidence: `.audit/Store-1.19.05/candidate.json`, `.audit/Store-1.19.05/checks.log`, `.audit/Release-1.19.05/checks.log`.

Prepared material: [review notes](ReleaseNotes-1.19.05.md), [Store release notes](StoreReleaseNotes-1.19.05.txt), [reviewer instructions](StoreReviewerNotes-1.19.05.txt), [English listing](StoreListing-en.txt), [listing fields](StoreListingFields-en.json). Pricing, licensing terms, availability and privacy declarations are unchanged. This preparation does not change the live Store release.



## Version 1.18.20.0 — submitted, 1 November 2026

Partner Center confirmed **Update in certification** for **Submission 13**, ID `1152921505702288513`, with Submission complete and Pre-processing in progress. It explicitly confirms automatic publication as soon as certification passes. Approval and public availability of 1.18.20 remain pending. **Submission 12 (1.18.19.0) is the existing live Store presence.** Pricing, availability, age ratings, permissions and optional licensing terms are unchanged.

Submitted package: `dist/store/ELMA-IoT-MIE_1.18.20.0_x64.msix`, 24,375,676 bytes, SHA-256 `eb0866015ee061965921ee1308eea990459b05d1b5a87b04296b892bebff9f12`. English description, release notes and reviewer testing instructions were updated. MakeAppx validation, offline Store modules, responsive clipboard/deletion checks, cell history, incremental recovery, all 20 translated tutorial playbacks and anonymous public data-download digests passed. Source and documentation are pushed; private v1.18.20 and public mie-content-v37 data releases are published. Existing approved signed executable modules remain unchanged. Evidence: `.audit/Release-1.18.20/store-submission.json`.

Release notes: [1.18.20](ReleaseNotes-1.18.20.md), [Store notes](StoreReleaseNotes-1.18.20.txt), [reviewer instructions](StoreReviewerNotes-1.18.20.txt). Older entries below record their status at submission time.

## Version 1.18.19.0 — submitted, 1 November 2026

Partner Center confirmed **Update in certification** for **Submission 12**, ID `1152921505702288457`, with the Submission step complete and Pre-processing in progress. It explicitly confirms automatic publication after certification. Approval and public availability of 1.18.19 remain pending. Submission 11 (1.18.18.0) is the existing live Store presence. Pricing, availability, age ratings, permissions and optional licensing terms are unchanged.

Submitted package: `dist/store/ELMA-IoT-MIE_1.18.19.0_x64.msix`, 24,348,149 bytes, SHA-256 `f283f8560aa2cf536d06e65d8110cf2a7f628940638b2d174f219603c38ed989`. MakeAppx validation, Store offline bundle checks, equipment identifier deletion and Quarantine reconciliation regression checks passed. Existing approved signed executable modules and data packages are reused. English release notes and reviewer testing instructions were updated. Evidence: `.audit/Release-1.18.19/store-submission.json`.

Release notes: [1.18.19](ReleaseNotes-1.18.19-review.md), [Store notes](StoreReleaseNotes-1.18.19.txt), [reviewer instructions](StoreReviewerNotes-1.18.19.txt).

## Version 1.18.18.0 — submitted, 1 November 2026

Partner Center confirmed **Update in certification** for **Submission 11**, ID `1152921505702288179`, with Submission complete and Pre-processing in progress. Publishing starts automatically as soon as certification passes; approval and public availability of this update remain pending. The validated package, English release notes and reviewer instructions are saved. The overview identifies Submission 10 as the existing Store presence. Pricing, availability, age ratings and optional licensing terms are unchanged.

Submitted package: `dist/store/ELMA-IoT-MIE_1.18.18.0_x64.msix`, 24,343,332 bytes, SHA-256 `e43530cf46b845d2e037c563901c22670dbdfec39b919cc5847f1d5d059fcadd`. This is the corrected replacement for the earlier 1.18.18 portable review. It removes the worksheet-level offset that made Excel initially paint the frozen heading twice. The affected workbook reproduced the problem, and its comparison copy was confirmed to open with one header. Export and Store offline-bundle checks passed. Existing signed v36 optional content is reused without changing published package bytes. Evidence: `.audit/Release-1.18.18/store-submission.json`.

Release notes: [1.18.18](ReleaseNotes-1.18.18.md), [Store notes](StoreReleaseNotes-1.18.18.txt), [reviewer instructions](StoreReviewerNotes-1.18.18.txt). Older entries below record their status at submission time.

## Version 1.18.17.0 — submitted, 31 October 2026

Partner Center confirmed **Update in certification** for **Submission 10**, ID `1152921505702285794`, with Submission complete and Pre-processing in progress. It explicitly confirms that publishing starts as soon as certification passes. Approval and public availability of this update remain pending. The validated package, English listing, feature summaries, release notes and reviewer instructions are saved. The overview identifies Submission 9 as the existing Store presence. Pricing, availability, age ratings and optional licensing terms are unchanged.

Submitted package: `dist/store/ELMA-IoT-MIE_1.18.17.0_x64.msix`, 24,343,114 bytes, SHA-256 `df6090d83e85090baaa1207509918e13e40593287b0105077ff4495865fd0aea`. MakeAppx validation, signed/offline bundle checks and actual public data-pack download verification passed. All 20 language packs preserve custom wording and reject unsafe paths. Product identity and publisher are unchanged. Evidence: `.audit/Release-1.18.17/store-submission.json`.

Release notes: [1.18.17](ReleaseNotes-1.18.17.md), [Store notes](StoreReleaseNotes-1.18.17.txt), [reviewer instructions](StoreReviewerNotes-1.18.17.txt).

## Version 1.18.10.0 — submitted, 31 October 2026

Partner Center confirmed **Update in certification** for **Submission 9**, ID `1152921505702284776`, with Submission complete and Pre-processing in progress. The validated 1.18.10.0 package, English product description, feature summaries, short description, release notes and reviewer instructions are saved. Publication is automatic after certification; approval and public availability of this update remain pending. The existing live version remains Submission 8 (1.15.5.0). Pricing, availability, age ratings and optional licensing terms are unchanged. Evidence: `.audit/Release-1.18.10/store-submission.json`.

Candidate: `dist/store/ELMA-IoT-MIE_1.18.10.0_x64.msix`, 24,317,125 bytes, SHA-256 `d2ae309c72af28ed1d94900b3fa3d8bbafec3a08c66129b775b0bcf21f120bcf`. The assigned product identity and publisher remain unchanged. MakeAppx validation, transparent/light/dark shell-icon checks, signed content verification and offline executable-module checks passed. Updated language and learning data are approved by exact app-compiled hashes; previously installed data works offline. Runtime checks cover all 20 languages, right-to-left guide rendering, corrected generated translations, custom wording preservation and synthetic tutorial restoration.

Release notes: [1.18.10](ReleaseNotes-1.18.10.md), [Store notes](StoreReleaseNotes-1.18.10.txt), [reviewer instructions](StoreReviewerNotes-1.18.10.txt). Current status is recorded above; older entries below are historical.

## Version 1.11.0.0 submitted — 18 October 2026

The owner authorized pushing the appropriate private/public repository content and submitting the current version as an update to the existing Microsoft Store listing. Partner Center was refreshed and confirmed Submission 2 is now live; a new Submission 3 was created with ID `1152921505702162749`.

Candidate: `dist/store/ELMA-IoT-MIE_1.11.0.0_x64.msix`, 3,200,403 bytes, SHA-256 `e2c5a9dfb71fc9020afff1193f9fc969e550e7595b7bf1f25dc76b1b991cde09`. Identity, publisher and x64 Windows.Desktop targeting match the existing product. MakeAppx validated the 13 payload files. No customer project, owner signing/recovery material, settings or game scores are packaged.

Store modules are bundled inside the reviewed MSIX. A separately signed catalog verifies the six included content packages. Store mode uses installation-directory package paths and refuses network replacement of missing/damaged executable content. Languages, guide/tutorials, Theme Studio, games and GLB viewer work offline; the portable edition retains the public on-demand pack behavior. `tools/Build-Store.ps1`, `tools/Build-StoreContent111.py` and `tools/Build-MSIX.ps1` implement the separate build. The Store bundle test passed with networking blocked, including a real Studio launch, classic-game activation, GLB loading and tamper rejection.

Partner Center confirmed **Update in certification**, Submission complete and Pre-processing in progress for Submission 3 (`1152921505702162749`). The package is validated and the listing/release notes and reviewer instructions were updated. Publication is automatic after certification; approval and public availability of version 1.11 remain pending. Free availability and optional owner-issued licensing are unchanged. Existing age ratings remain complete. Evidence: `.audit/Store-1.11-submitted.png`. The older status entries below are historical.


## Update submitted on 18 October 2026

The publisher authorized submission of version **1.7.21.0** as an update to the existing Store application. Partner Center confirmed **Update in certification**, with Submission complete and Pre-processing in progress. Submission ID: `1152921505702156595`. Publication is automatic after certification; approval and public availability of this version are still pending.

Submitted package: `dist/store/ELMA-IoT-MIE_1.7.21.0_x64.msix` (1,587,274 bytes), SHA-256 `64838daee714c1148a44709aa00e16128c25f8c9c712c24a6f6c1e47a4475dff`. The superseded 1.7.5 draft package was removed from the submission. The existing listing remains free and publicly available.

The update includes current feature descriptions, release notes, optional owner-issued license disclosures, external-purchase declaration, privacy text for synchronization/licensing/network services, and reviewer instructions. Updated IARC answers include mild fantasy violence and user interaction/purchase disclosures. The publisher explicitly accepted the fresh IARC declaration. Preview ratings: ESRB Everyone (Mild Fantasy Violence), PEGI/IARC 3+, USK 6+, Russia 12+, Brazil 14. No customer projects, imported drawings, credentials, private owner keygen or license keys are included in the package.

Submission evidence: `.audit/Store-1.7.21-submitted.png`. Historical review holds below are superseded by this explicit submission authorization.

The Store build uses an MSIX package. Microsoft signs accepted Store packages; this does not sign the separately distributed portable EXE.

Build the application without an embedded customer project:

```powershell
dotnet build .\MiePortable.csproj -c Release -o .\build -p:StoreBuild=true
```

Reserve an MSIX application in Partner Center. Copy the exact Package/Identity/Name, Package/Identity/Publisher and publisher display name from its Product identity page, then run:

```powershell
.\tools\Build-MSIX.ps1 -IdentityName '<assigned package name>' -Publisher '<assigned CN>' -PublisherDisplayName '<publisher display name>'
```

The registered application is **ELMA-IoT MIE**, Store ID `9NSZMSQKXH67`. Its assigned identity is:

```powershell
.\tools\Build-MSIX.ps1 -IdentityName 'ElnurMehdiyev.ELMA-IoTMIE' -Publisher 'CN=DFCABF04-063D-4487-9360-53745D23DF0A' -PublisherDisplayName 'Elnur Mehdiyev'
```

The current 1.7.21 output is `dist\store\ELMA-IoT-MIE_1.7.21.0_x64.msix`. This package is prepared locally; the initial Store submission remains version 1.4.0.0 until a newer submission is explicitly made. It contains the executable, runtime configuration and app icons. The script rejects an executable containing an embedded project. Imported projects, backups, logs and local settings are excluded.

For the initial Store draft, distribution is free and publicly discoverable. Screenshots must show an empty workspace and application-owned guide text only. Do not capture imported well names, equipment serials, part numbers, drawings or other operational data. The screenshot capture utility in `.audit` uses isolated settings and does not load a project.

The initial submission was sent for certification on 17 October 2026 (Turkey local time), with explicit publisher approval for automatic free public release after certification. Partner Center confirmed **In certification**, with submission complete and pre-processing in progress. Submission ID: `1152921505702154389`. Submitted package SHA-256: `16A4B6F068B3B8D82283E82FDF1AA3D2DB65777547D4424FC3AE7743BEE2CE3F`. This status does not mean certification has passed or that the app is already available in the Store.

Store installations save working files in the package's per-user `LocalState` folder. Portable installations continue saving beside the executable. Users can import their own projects after installation.

Before publication, complete Store listing assets, privacy disclosures, age ratings, availability and certification notes. Validate the actual production package on Windows and submit it for certification. An unsigned local MSIX is a submission artifact, not a trusted installer for other PCs. Test packages in `.audit` use a placeholder identity and must not be submitted.

Version 1.7.12 presents owner-issued license activation for partner, evaluation or separately agreed commercial use. No price, payment processing or automatic subscription is configured by activation. Existing keys remain compatible; license expiry and feature checks are unchanged. The initial 1.4.0.0 submission was observed live in Partner Center on 17 October 2026. Submission 2 is a draft; a local package build does not publish it.

The 1.7.12 interaction-optimization build is for local owner review. Do not upload or submit this candidate until the owner has tested it and explicitly requests Store submission.

The local 1.7.12 candidate also includes the offline idle runner, faint live frost/blur, translated guide/tutorial and Windows Snap-compatible window sizing. No Store upload or submission is authorized by this build.

Version 1.7.21 is a local review build. Microsoft Store upload and submission remain on hold for owner testing.

## Local review after submission

Version 1.7.22 is a local test build prepared after the 1.7.21.0 Store submission. It adds scrolling, in-window tutorial restoration, tutorial close alignment, sync progress/preferences and randomized idle selection fixes. It has not been uploaded or submitted to Partner Center. The next Store update requires a new publisher instruction after testing.


## Transparent taskbar icon packaging correction — 19 October 2026

The source PNG and ICO already retain transparent rounded corners. The installed Store package used a pale VisualElements background and lacked unplated target-size assets, allowing Windows to add a rectangular backplate. Build-MSIX.ps1 now uses a transparent background and generates the 14 shell target sizes in default, dark unplated and light unplated forms, plus 100/200/400 percent scale assets. The existing illustration is retained.

A local packaging-only validation used a copy of the installed 1.11.0 executable and its existing signed content bundle. MakeAppx validation succeeded and tools/Check-PackageIcons.ps1 verified all 42 target-size variants, exact sizes, fully transparent corners and opaque center artwork. The local test package is not a new application release, has not been installed, and has not been submitted to the Store. The currently installed Store app remains unchanged; the packaging correction takes effect with a subsequent signed Store update.

Reference: https://learn.microsoft.com/en-us/windows/apps/design/iconography/app-icon-construction


## 1.11.2 owner review hold — 19 October 2026

The owner requested local testing of Save/Save as, keyboard/clipboard behavior and translated guides/tutorials before any Microsoft Store submission. This version has not been submitted. The review build embeds the newly prepared guide and translations for testing; normal public content activation still requires the existing publisher signature, whose private key is absent from this PC. No signing keys or security checks were replaced. The taskbar icon packaging correction above remains part of the next reviewed Store package.
