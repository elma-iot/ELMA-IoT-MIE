# MIE 1.19.14 — role access release candidate

This candidate adds owner-signed licensing roles: Full Control, Manager / Approver, Engineer / Data Editor, Maintenance Technician / Inspector and View Only. Managers and Engineers can be assigned Equipment / Operations, Maintenance and Planning departments.

- Menus, right-click actions, toolbars, shortcuts, paste, replace, Undo/Redo and 3D editing follow the licensed role and project protection. Nested context menus follow the same rules. Copy, history, navigation, printing and exports remain available for viewing.
- Restricted licensed users open free or unprotected databases for viewing only. Full Control reviews a database and chooses **File > Save as protected MIE project…** before other roles can work on it. The original file is preserved. Free users can still edit ordinary free projects; protected projects are read-only in the free edition.
- Protected projects carry signed enrollment and saved content proofs. Save, recovery, incremental sync and reviewed import enforce the protection boundary. Legacy keys keep their ordinary-project behavior but cannot authorize protected edits; older clients reject the new role key format.
- Inspection submission and approval are separate permissions. Maintenance Managers can approve submitted evidence or request reinspection. A person cannot approve their own report, except Full Control. Existing test, repair and physical-return requirements remain enforced.
- Optional 3D editing permissions also apply in the large viewer. Language and game packs remain available to every role. Guides, tutorials and all 20 language catalogs include role guidance.

Licenses authorize the Windows account holding its private device key; they are not an interactive user login or online revocation service. Previously issued valid keys remain valid until expiry. Use separate Windows accounts and portable application folders for different people, retain authorization-key.dat with application data, and protect owner signing keys.

This is a local review candidate. Microsoft Store submission is held until owner testing is complete. Back up production data before adopting project protection; protected copies require MIE 1.19.14 or later.
