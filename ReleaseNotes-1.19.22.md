# MIE 1.19.22

Prepared for local testing. Microsoft Store submission remains on hold.

- Add named connection surfaces and points to shared PN models, with unique numeric IDs, editable coordinates and spacing, deletion, history and undo/redo. Model units control physical measurements.
- 3D snapping finds mesh edges, vertices, ring/hole centres and other mesh-derived reference candidates. Point markers align with the model surface. Review snapped positions before using them for assembly.
- Point-to-surface dimensions measure perpendicular separation. Top/bottom reference levels show vertical ΔY, excluding the point's sideways offset. Both upper and lower levels appear when available, with outside dimension lines and clear gaps around values.
- Mesh selection highlights actual geometry. Ctrl-select groups meshes; internal selections remain visible through faded surrounding meshes. Existing material, colour, texture and mapping controls apply to selected meshes.
- PN appearance and connection definitions are shared across serials. Serial-specific damage remains separate and retains the existing return-to-service clearing behaviour.
- Model loading uses cached immutable geometry, faster spatial indexing and background preparation with stage progress. GLB uploads support up to 120 MB, subject to existing mesh/resource limits.
- Item View shows description, model dimensions and weight in kg/lb. Inventory weight overrides the steel mesh-volume estimate, which is labelled approximate. Mesh repair for volume estimation does not modify the original model.
- Independent shared-model edits refresh and merge before retrying. Overlapping edits remain protected. A failed Apply no longer blocks Save/Close indefinitely; recovery offers Retry, Continue without saving 3D edits, and Cancel. Already applied project changes are retained.

Connection data requires MIE 1.19.22 or later. Retain backups before opening updated projects with an older application.

The portable candidate includes the approved offline content cache for testing. The Store package bundles its approved executable modules; language and learning packs remain optional. Guide topics, eight guided examples and all 20 language catalogs are updated for this release.

Guide: [Model connections and Item View](ModelConnections-1.19.22.md).
