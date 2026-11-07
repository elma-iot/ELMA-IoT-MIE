# MIE 1.19.19 — background working recovery candidate

Prepared for owner testing. Microsoft Store submission remains held.

- Edits stay in the working workspace. Routine changes and resizing no longer await disk journaling or show the generic progress bar.
- After two seconds without PC input or new edits, a worker coalesces changes into a temporary recovery checkpoint. Snapshot compression and file generation run in the background. Edits made during that write remain pending for the next checkpoint.
- Named MIE packs save on an explicit Save, on leaving the project when Save is selected, or quietly after ten minutes of system-wide PC inactivity. Manual Sync remains an explicit save action; automatic sync only adopts its local pack after long inactivity.
- New unnamed workspaces receive temporary recovery copies. Startup can offer recovery without assigning the temporary path as the user's save destination.
- Layout-only edits skip equipment lifecycle and stock recalculation while retaining role permissions, change history and Undo/Redo.
- Explicit saving and closing wait for responsive edits and temporary writes already in progress. Disposal safeguards remain durable.
- Guide, tutorials and all 20 language catalogs describe the updated workflow. Existing approved optional viewer modules are reused.
