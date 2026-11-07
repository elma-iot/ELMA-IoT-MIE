# MIE 1.19.23 candidate validation

Prepared for owner testing. Microsoft Store upload and submission remain on hold.

543 assertions passed across 12 suites.

- ConnectionCommitChecks: 15 assertions.
- ConnectionSurfaceUiChecks: 58 assertions.
- ConnectionTutorialChecks: 48 assertions.
- EquipmentMembersChecks: 19 assertions.
- GroupedItemViewChecks: 14 assertions.
- ItemViewUiChecks: 77 assertions.
- ModelLoadChecks: 8 assertions.
- PartModelLibraryChecks: 19 assertions.
- RoleAccessChecks: 219 assertions.
- RoleModelViewerChecks: 11 assertions.
- RoleUiChecks: 30 assertions.
- StoreBundleOfflineChecks: 25 assertions.

The grouped Item View regressions exercise a live duplicate-highlighted Master cell: uploading its shared model refreshes the cube badge without rebuilding the existing column. Tests cover the top-level View item command, All serials mode, absent serial damage callbacks, disabled damage/inspection/upload controls, and explicit serial selection restoring only that serial’s evidence and damage. Permission refreshes cannot enable damage while All serials is selected. A grouped cell with only one actual item opens the serial directly.

Existing native tests cover item previews, inspection attachments, document save copies, painting/history flush, model sharing, grouped equipment, connection commits, and free/licensed protected-project permissions.

Eight guided examples played in English, Russian and Arabic (24 playbacks), checking both real control visits and restoration of the temporary project. Translation integrity checks cover all 20 supported languages, with 321 learning entries and 3,271 interface entries per language. These are automated integrity checks, not independent human review of every translation.

MakeAppx packaging, archive integrity, embedded application/module hashes, unchanged Store identity and exclusion of customer projects and license/device keys were verified. Offline bundle checks load the approved 1.19.22 viewer and reject altered executable content. Updated language and learning packs are 1.19.23; the previous viewer remains unchanged.

Portable SHA-256: `7b3318fe61ec53d670e89c911d5c20e0045fbfcc6657110cca76fb507af85825`

MSIX SHA-256: `42912bc069a53a0d96fa7ccbf2600f592cbc610545dc5e0fe5fbe3a31cfb3a7f`
