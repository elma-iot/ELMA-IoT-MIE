# MIE 1.19.22 candidate validation

Prepared for owner testing. Microsoft Store upload and submission remain on hold.

760 assertions passed across 12 suites.

- ConnectionCommitChecks: 15 assertions.
- ConnectionGeometryChecks: 19 assertions.
- ConnectionSurfaceChecks: 27 assertions.
- ConnectionSurfaceUiChecks: 58 assertions.
- ConnectionTutorialChecks: 320 assertions.
- MeshSelectionChecks: 22 assertions.
- ModelAppearanceChecks: 6 assertions.
- ModelLoadChecks: 8 assertions.
- RoleAccessChecks: 219 assertions.
- RoleModelViewerChecks: 11 assertions.
- RoleUiChecks: 30 assertions.
- StoreBundleOfflineChecks: 25 assertions.

The eight new guided examples played in each of the 20 supported languages (160 playbacks), with separate checks for real control visits and original project restoration. The point/surface controls, 3D magnet, mesh selector, Settings, measurements and information pane are targeted on a synthetic model in a temporary workspace. Role-restricted users retain the existing department-specific guidance. No customer projects or actual license files are changed by these tests.

Translation integrity checks cover 321 learning entries and 3,269 interface entries in every supported language, preserving formatting placeholders, links and UTF-8 text. These are automated coverage/integrity checks, not a claim of independent human review of every translation.

Native host regressions include reported point coordinates, shared-model revision checks, independent rebasing, overlapping conflict refusal, pending edit preservation, recovery/discard choices, PN sharing, undo/redo, serial-specific damage isolation, vertical reference dimensions and mesh selection. The role suite covers free/unprotected and protected project permissions and large-view inheritance. An older large-window test was updated to await asynchronous window preparation before asserting permissions.

MakeAppx packaging, package integrity, embedded application/module hashes, unchanged Store identity, and exclusion of customer projects, license/device keys and owner tools were checked. Offline tests load the approved viewer and Theme Studio; tampered executable content is rejected. The portable release includes one Content cache folder and a compatible copied local license.

The model preview remains a beta engineering aid. Review mesh-derived snap candidates, original units, calculated distances and approximate steel weight. Shared connection metadata does not automatically approve or install a well stack-up.

Portable SHA-256: `dcdf6899ec8b6ff78932c5ee8e85f881d7823947ce878ef9d86206ee9f06f5cd`

MSIX SHA-256: `0538014950ff76cac1e7f826fc8fa03be07dd86183919714fa14ddf0593e3642`
