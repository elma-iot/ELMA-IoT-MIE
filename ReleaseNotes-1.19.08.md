# MIE 1.19.08 - compact model header and responsive brushes

The model filename appears beside Settings on the same row as Reset view, Home and Large View. The separate filename row is collapsed after a GLB loads, giving that space to the model canvas. Long filenames use an ellipsis and retain the full name in a hover tip. The large viewer keeps the filename too.

The filename and its layout are supplied by the optional 3D pack; the main application hosts the toolbar and retains the status/progress row during loading and document previews. Active marking and deformation tools project a live surface footprint before clicking; previews do not alter the model, item or history. Surface BVH picking, local decal projection, cached decals/images and coalesced incremental deformation replace full-model scans and canceled/restarted stroke replays. Heavy refinement and indexing stay on workers; prior completed strokes are reused. Original uploads remain unchanged.

A synthetic 64,800-face benchmark verifies local triangle queries, dense-mesh stamping, latest-work retention and dispatcher responsiveness. Guides/tutorials and all 20 languages describe the updated controls.

Portable review: `build/MIE Portable.exe`. Restart MIE to load the verified 1.19.08 viewer from `mie-content-v46`, or use Browse pack. The Microsoft Store candidate remains held for owner testing; no upload or submission.
