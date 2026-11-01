# MIE 1.19.01 — attachment pane controls

Portable review in the 1.19 series. Version 2.0 remains deferred, and this build has not been submitted to Microsoft Store.

- The button below the attachment list is now **Upload**. Its left and right edges align with the list. The former upper Upload button and lower Save a copy button are removed.
- The attachment area starts at half of the left Item View pane. Drag its divider downward to make it smaller. It cannot expand above the midpoint. The saved proportion is restored when Item View opens again and is preserved when the window is resized. Preference writes run in the background after the divider is released.
- Right-click an attachment and choose **Save as…** to save its original file to the PC. The clicked row becomes the selected file. Saving supports every listed format, runs in the background and writes atomically without changing the project's attachment.
- Guide text and the Upload label are updated in all 20 application languages. The right pane remains primarily for document and 3D viewing.

Verification covered native divider keyboard controls and the midpoint limit, restored position, window resizing, exact button/list alignment, attachment-row and list-owner context menus, byte-exact text/photo/PDF downloads, document/3D preview, sections, inspection review, paid/free access, PDF export and native Excel 3D export. Existing signed viewer version 1.19.00 is reused unchanged; the UI and language/guide data are version 1.19.01.

Portable executable: `build/MIE Portable.exe`. [Updated guide and languages](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v40). [Unchanged optional viewer pack](https://github.com/elma-iot/ELMA-IoT-MIE/releases/tag/mie-content-v39).
