# MIE 1.19.30 — attachment rename and inline well model choice

- Fixed Item View attachment Rename/Replace reading a WPF checkbox from the background save worker. Both ordinary documents and shared GLB attachments now rename and refresh without the thread-ownership error.
- Attachment naming retains newer project minimum-reader requirements, original model hashes, shared references and source files.
- When a P/N has multiple GLBs, the well constructor shows a model dropdown directly below the equipment name in each Hardware cell, with P/N and SN underneath. Select the displayed model per row. Connections, units and motion inputs refresh live; the selected content hash is saved with the constructor and restored when reopened.
- Existing advanced model controls remain available. Single-model rows retain their compact layout.
- Updated the user guide and well-constructor tutorial text in all 20 languages.

Includes the 1.19.29 material presets, contact-deformation preview, stable model names, cut-view preservation and complete project merge improvements. Contact deformation remains approximate visualization rather than stress or failure analysis.

No licensing, permissions, pricing or availability changes. Distribution archives exclude customer projects, private licenses, authorization keys and owner tools.
