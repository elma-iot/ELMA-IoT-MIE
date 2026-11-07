# Model connections and Item View — MIE 1.19.22

Open Help > User guide for these topics and their guided examples. Examples use a temporary synthetic workspace and restore the original project. Editing follows the licensed role and project permissions.

## Add and edit a connection surface

Open the item in Item View and select its GLB attachment. Select Add connection surface. Use the adjacent triangle to choose XY (normal Z), XZ (normal Y) or YZ (normal X), and confirm model units. For top and bottom levels on a Y-up model choose XZ. Move over the model: a translucent plane and green inner/outer intersection contours preview the position. Movement clamps to the model bounds. Click to enter a numeric ID and a name, then Apply. IDs must be unique on that model; another model may reuse the ID. Saved contours remain visible. Right-click a mark to edit its position, name or ID, or Delete it. Escape exits placement. These definitions are shared by PN/model; they are not serial-specific damage.

## Add a surface point and its cross marker

Select Add point connection, move over the model and left-click the desired surface. The cross follows the surface orientation; it is a point marker, not an intersection plane. Enter its unique numeric ID and descriptive name, review X/Y/Z in metres and Apply. Use 3D snap before clicking when a hole, ring or edge centre is needed. A snapped hole centre may lie in empty space inside the hole; confirm the intended location. Right-click a saved cross to change its ID, name or coordinates, or Delete it. Point and surface IDs share the same uniqueness rule. Point coordinates and normals stay with this PN/model and appear for other serials sharing that model.

## Use 3D snap for points and surfaces

Click the 3D horseshoe magnet to enable snapping, then choose the point or surface tool. Allow background feature preparation to finish. Move close to an edge, vertex, midpoint, ring/hole centre, aligned-ring centre or mesh centre. The highlighted target and its label preview the candidate before placement. Click only after checking the target, then confirm ID and name. Snap uses mesh geometry rather than CAD topology: irregular or incomplete holes may not produce a centre. Rotate or zoom the view, disable snap for free placement, or edit numeric coordinates for precise placement. Snapping never changes the original GLB. Its setting is remembered with the item view.

## Read and adjust connection distances

Hover over a saved contour or point cross to see its ID, name and reference distances. A point shows the nearest marked surface level above and below on each available reference axis. For top/bottom levels, ΔY is the vertical difference: sideways distance from the model centre is excluded. Horizontal extension lines reach an outside vertical dimension line with a gap around its value. Values use metres to three decimals. Point-to-point Centre distance remains a spatial distance. The details pane lists the same reference measurements. Double-click a dimension to edit its selected mark. Surface editing also offers spacing from another parallel surface; changing that spacing moves the selected surface. Check model units before relying on dimensions.

## Select meshes and change shared appearance

Select the cube-shaped mesh selection tool. Hover highlights actual mesh geometry. Click to keep it selected; Ctrl-click adds or removes another mesh. Alt-click cycles through depth candidates so an internal mesh can be selected. Other meshes become partly transparent to keep the selection visible. Open Settings and change material, colour, texture, UV mapping, wrapping, repeat, offsets or rotation: those controls affect the selected meshes. With none selected they affect all meshes. Choose an original texture or a provided preset, or upload a PNG/JPEG up to 16 MB. Texture presets are generic materials, not bundled proprietary V-Ray assets. Appearance belongs to the PN/model; marks and deformation belong to the individual SN. Undo and Redo support applied changes.

## Model dimensions, entered weight and estimates

Item View shows the equipment description, model X/Y/Z size in metres and weight in kg and lb. Description comes from the equipment section. Dimensions use the original model bounding box and configured model units. Add an actual Weight in Inventory, selecting kg or lb; the actual value takes precedence. Without an entered weight, a valid mesh volume may produce a steel estimate at 7,850 kg/m³, marked ≈. Open planar mesh boundaries may be closed for calculation only; the uploaded original is preserved. Overlapping shells, missing geometry and non-steel materials can make estimates inaccurate. An unavailable volume is shown as unavailable rather than as an actual weight. Enter the verified weight when known.

## Save connection edits and recover from a failed Apply

Apply records the shared PN/model edit in project history; save the project to persist the working changes to its MIE pack. Model preparation and native writes run in the background. Independent concurrent edits refresh and merge; overlapping changes require review. A failed Apply keeps the entered values available and Cancel leaves the current project intact. A handled failed point save no longer traps Save or Close. If pending viewer edits still cannot be applied, choose Retry, Continue without saving 3D edits, or Cancel. Discarding pending 3D edits keeps changes already applied to the project; the normal project Save/Discard/Cancel choice follows. Keep regular project saves; recovery after Task Manager termination cannot guarantee every unsaved change.

## Navigate, cut and inspect a model

Use the mouse wheel to zoom towards the pointer, orbit with the left button in Navigate mode, and pan with middle drag. Home and Reset view fit the model; the view selector offers perspective, orthographic and preset directions. Open large 3D view gives more room. In Settings, select the cut axis even before enabling Cut view. Enable it and drag the double-arrow handle or use the position control to move the plane. Turn Cut view off to restore the full model. Scene lighting, ground, camera and item settings are retained separately from the original asset. Damage brush previews show where a mark will land; deformation raises with the left button and dents with the right. Damage remains tied to the SN and follows the existing return-to-service clearing workflow. Uploads support GLB files up to 120 MB within resource limits.

Shared connection IDs describe model references. The current 3D Beta assembly still requires review of component depths, model units, anchors and offsets; these definitions do not automatically approve or install a stack-up.
