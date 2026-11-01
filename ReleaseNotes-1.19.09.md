# MIE 1.19.09 - independent paint, editing sessions and CAD ground

Paint decals now clip geometry to their own fixed 0..1 UV footprint. Source texture seams, repeat, wrapping, offsets and placement cannot stretch the paint or expose the underlying texture through its opaque center. Soft brush edges remain intentionally feathered. Live previews use the same corrected projection.

In deformation mode left click raises a convex area, right click makes a concave dent and middle drag pans. A hint accompanies the controls; Pointer and paint-mode navigation remain available.

Damage edits stay local throughout the editing session, including pauses between strokes. Explicit Save, changing attachments, leaving/closing the viewer or saving/closing the project flush one asynchronous checkpoint. The background commit uses optimistic stale-state checks without the global busy indicator, an exclusive edit flag or a full worksheet refresh. Pending writes are tracked before the first await. Failed saves retain the scene for retry; reopening its item/model recovers it. A failed large-window close transfers pending marks back to the parent. Existing immutable damage checkpoints, actor history, return clearing and Undo/Redo remain intact.

The ground is a circular polished surface with a soft transparent edge, separate contact shadow and optional subtle model reflection. Settings remembers Ground reflection and Ground shadow per item/model; Theme Studio Model Floor controls the color. Reflection shares the existing geometry and is automatically omitted above 200,000 displayed triangles or during software rendering. Camera movement reuses the same ground transforms.

The scene pattern follows [Fusion display effects](https://www.autodesk.com/learn/ondemand/tutorial/adjust-display-settings?contextId=AP-ADJUST-DISPLAY-SETTINGS) and [SOLIDWORKS scene controls](https://help.solidworks.com/2023/English/SolidWorks/sldworks/HIDD_DVE_SCENE_EDITOR_BASIC.htm). Native WPF reflection is a lightweight planar approximation, not a ray-traced renderer.

Validation covers extreme/coarse UVs, rendered paint color over wood and remapped metal, left/right deformation, no idle checkpoint, asynchronous session commit, failed-close recovery, dense-mesh interaction, application busy-state behavior, saved damage/return history, exports, dialogs and translated help. Guides/tutorials and all 20 language catalogs are updated. Viewer rendering/tools remain in the separately verified pack.

Review EXE: `build/MIE Portable.exe`. Restart MIE for the verified 1.19.09 viewer from `mie-content-v47`, or use Browse pack. Microsoft Store update **1.19.9.0** was submitted on **1 November 2026** as **Submission 14**. Partner Center confirms **In certification / Pre-processing**, with automatic publication after certification. [Submission record](StoreSubmission-1.19.09.md).
