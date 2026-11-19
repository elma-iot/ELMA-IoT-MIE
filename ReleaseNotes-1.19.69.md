# ELMA-IoT MIE 1.19.69

This update covers changes since 1.19.56. [Previous release notes](ReleaseNotes-1.19.56.md)

## Equipment lifecycle

- Procurement, warehouse, engineering, and operations teams can follow the same equipment record from receipt and storage through installation, inspection, and final disposal. Serial-based matching and conflict warnings help teams avoid duplicate records.
- Filter Inventory by location and equipment status. The site or drillship selector also helps narrow well and schedule views, while global search can find records across locations.
- The licensed Disposal register keeps the item's history and supporting evidence. Scrap approval moves the item out of active Inventory and Quarantine into Disposal. Completion and documented reversal have separate controls. PDF and Excel evidence reports can include documents, images, and serial-specific 3D views.

## Storage and Inventory

- Import a GLB facility and mark named storage locations. Place equipment on textured pallets, drag or rotate pallets on shelves, and share a pallet when loads fit. The picker shows descriptions, sorts by weight and serial number, and excludes equipment already placed.
- After placement, Inventory shows the item's **3D Map Location**. Click it to open Storage and fly to the exact item from the previous camera position or Home. In Storage, hover over the item to see its part number, serial number, and description. Right-click and choose **See in Inventory** to highlight its row.
- Storage adds facility finishes, HDRI controls, interior reflections, and adjustable animated water. Direct3D 12 adapts its rendering to the scene, and WPF is available for compatibility. The Storage overlay shows FPS, GPU use, VRAM, CPU use, and RAM.

## Technical documents and 3D engineering

- Tech Specs indexes part-number references, opens manuals at matching pages, and supports replacing documents and updating their references. PDF viewing adds continuous scrolling, text search, and clickable contents links.
- Inventory can suggest descriptions and kg/lb weights from indexed manuals. Review the suggestions before applying them to a part number.
- 3D Viewer search opens matching equipment models. Saved notes, marks, and damage follow a serial across Inventory, Quarantine, and Disposal. The viewer adds a damage eraser, separate note colors, and a mesh color command.
- Geological section preparation shows progress and completed geometry as it becomes available. Updates improve cut faces around excavations and thin formation layers. Workspace startup and incremental saves also received performance improvements.

## Getting started

The welcome tour supports language selection and role-based walkthroughs. Help provides access to the tour, and the first-start notice explains how the application handles project data and network activity.

The 1.19.69 x64 package was prepared for Microsoft Store submission. Check the listing for availability. [Microsoft Store listing](https://apps.microsoft.com/detail/9NSZMSQKXH67)
