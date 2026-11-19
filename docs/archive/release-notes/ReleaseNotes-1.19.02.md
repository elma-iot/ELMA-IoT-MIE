# MIE 1.19.02 — Quarantine action tips

Portable review in the 1.19 series. Version 2.0 and Microsoft Store submission remain on hold.

- Quarantine records awaiting action show a concise status and action button instead of the long stock-planning explanation. This covers physical Quarantine records and returned Inventory items projected into its assessment worklist. Inventory retains its existing details and Quarantine navigation tip.
- Licensed users choose **View item** to open the correct equipment in Item View. **Review inspection** handles inspection evidence and the release/scrap decision. **Lifecycle…** provides the controlled inspection, repair, testing, approval and disposal form directly from Item View.
- Users without licensed Item View receive a **Lifecycle…** action in the Quarantine tip. It opens the existing controlled form directly, without requiring Edit mode first. Existing evidence, testing, approval and lifecycle restrictions remain enforced.
- Action tips use the existing persistent hover behavior, pointer alignment and shared theme styling. Hovering only prepares lightweight navigation; it does not load item history or attachments. Opening Item View loads its data in the background. Lifecycle submissions from Item View use the responsive transaction path, retain audit history and preserve the user's current item/tab when they switch while work is running.
- The new explanation and guide text are available in all 20 application languages. Existing signed viewer components are unchanged.

Verification covered concise tip content, correct equipment focus, native and projected Quarantine rows, licensed and free actions, opening the real lifecycle form from Item View, persistent popup behavior, inspection/approval restrictions, evidence retention and lifecycle regression checks. Original project data is unaffected by hover and navigation.

Portable executable: `build/MIE Portable.exe`. [Guide and language data](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v41).
