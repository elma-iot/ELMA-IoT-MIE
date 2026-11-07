# MIE 1.19.23

Prepared for owner testing. Microsoft Store submission remains on hold.

- Model uploads now refresh the availability index on reused Master equipment columns in the background. Duplicate warnings remain visible alongside the 3D model badge; refreshing the indicator does not resolve or hide a data conflict.
- A grouped cell with one PN now has a top-level **View item** command. With several serials, it opens the shared PN model with **All serials** selected. A grouped cell containing only one actual item opens that individual item directly.
- The shared view lists only shared PN models. Serial documents, inspection, history and attachment editing require an individual serial selection. Painting and deformation are disabled, with no serial damage read/write callbacks attached to the shared viewer.
- Select one SN in the item selector to load its own documents and damage, with editing subject to the existing license role and project protection. Selecting All serials restores the shared original view. Large 3D views inherit the same restrictions.
- Shared PN material and connection settings remain available to roles that can edit them. Each serial keeps its independent evidence and damage records.
- The common item view, image/PDF/document previews, model loading, grouped editing, permissions and original-model sharing retain their regression checks. The new wording and guide guidance are included in all 20 language catalogs.

The application reuses the approved 1.19.22 3D viewer. Language and learning packs are versioned 1.19.23; earlier published packs and the 1.19.22 application remain unchanged. The local portable candidate includes one offline Content folder and a compatible license when available.
