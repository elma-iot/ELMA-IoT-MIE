# MIE 1.19.33 — direct cell editing and unavailable serial numbers

- Double-click an editable Master Equip. list data cell to enable edit mode and edit that cell. Clicking another data cell commits the current value and opens the next editor.
- NA and N/A in serial fields mean not available, show a translated hover explanation, and are excluded from duplicate serial checks. Entered text survives save/reopen. Real repeated serials retain their warnings.
- A scoped .NET Framework 4.8 accessibility workaround removes only orphaned editing-column trackers before commit/cancel, avoiding the null-element popup during focus changes and editing-mode changes. Normal accessibility remains enabled.
- Unavailable serials in multi-item cells retain separate positional identities.
- Includes the reviewed well cut-view scanner, water-mask consistency and seabed projection fixes.
- Updated user guide and editing/tutorial guidance in all 20 languages.

Prepared for owner testing. Store submission remains pending owner validation. Original project files and GLB geometry are preserved. Terrain/contact deformation remain illustrative previews.
