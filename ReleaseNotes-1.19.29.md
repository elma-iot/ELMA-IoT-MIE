# MIE 1.19.29 — model materials, contact preview and mesh-tree editing

Release prepared after owner testing. The owner authorized Microsoft Store submission on 9 November 2026.

- Linear movement previews highlight only the chosen positive or negative arrow half and update immediately when direction changes.
- Defining and previewing linear, rotation or planar movement preserves Cut view. The previous section remains visible until its replacement is ready.
- Physics Deformations previews local elastic contact between two selected meshes. Physical material name, Young’s modulus and Poisson ratio are saved with the P/N model. Explicit editable estimates override only the current simulation.
- Material provides over 130 selectable presets, grouped by alloy family and filtered by AISI/SAE, ASTM, API, UNS/named alloys or generic materials. Includes common oilfield steels, stainless families, nickel/copper alloys, indium and lead. Selection fills editable starting properties.
- Both contact dropdowns highlight hovered meshes in the viewport and restore normal appearance on leaving or closing.
- The model tree sits beside attachments and uses the available model height. Context menus stay within the application window and scroll as needed.
- Rename mesh, CAD node or motion-group labels without changing stable IDs, CAD geometry, material assignments, motion limits, connections or saved readings. Names persist through native save/reopen, history and synchronization review; independent renames rebase by key.
- Updated user guide, tutorial instructions, material categories and interface catalogs in all 20 supported languages.

The deformation feature is an approximate quasi-static surface-contact visualization. It distributes local displacement by relative stiffness, caps displacement at 5% of part size and limits a contact pair to 250000 vertices. It does not calculate stress, forces, plasticity or failure. Coarse/open meshes can miss contact. Material presets are editable room-temperature starting values rather than certified component properties or complete standards requirements.

Projects containing physical materials or renamed model nodes require reader 1.19.29. Existing connection-only projects retain their prior reader floor. Source models are preserved; temporary previews do not accumulate geometry edits.

Portable and Store packages include approved offline optional content and SHA-256 checksums. No customer projects, licenses or authorization files are included in distribution archives.
