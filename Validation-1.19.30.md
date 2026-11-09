# MIE 1.19.30 validation — 9 November 2026

- Final portable and Store .NET Framework 4.8 builds succeeded, with existing compiler warnings.
- Final attachment UI checks passed for ordinary-document and shared-GLB renaming through the real background save worker, deletion confirmations, original hashes/source files and project reader requirements.
- All 23 well hierarchy checks passed, including the inline model selector, connection/unit refresh and selected-model save/restore.
- Final model-resolution and replacement checks passed, including view-only authorization and native save/reopen.
- Final Store offline checks passed: verified bundled viewer, Theme Studio and games load without executable downloads; translated guides remain available; damaged executable content is rejected.
- The attachment UI fixture initially timed out because its isolated test folder lacked seeded optional content. Seeding the verified fixture fixed the harness; all checks then passed.
- All 20 UI/learning catalogs parse; updated constructor guides and tutorial content are included.
- MSIX identity ElnurMehdiyev.ELMA-IoTMIE, version 1.19.30.0, x64. ZIP/MSIX integrity, exact content sizes and SHA-256 pins passed.
- Distribution archives exclude customer projects, private licenses, authorization keys and owner tools. Local testing authorization is kept outside archives.

Checksums accompany the release assets. Microsoft certification is a separate external process.

- All four public optional assets and eight private release assets match local lengths and SHA-256 digests after upload.
