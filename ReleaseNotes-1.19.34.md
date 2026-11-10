# MIE 1.19.34 - model choice consistency and manual 2D replacement

- Owner-test correction: repeated NA, N/A or missing serial numbers no longer share one saved constructor entry. Legacy saves restore repeated rows by occurrence; new saves add distinct row and connection-reference keys. This prevents false occupied-connection errors and an empty well when reopening.
- Metadata-only GLB duplicates that differ solely in exporter identification share one active model choice. The copy with saved connection configuration is preferred; original GLBs and their history remain stored.
- Item View and the well constructor use consistent active choices. Superseded model versions are excluded from current choices, and saved constructor model references follow unambiguous replacement/duplicate aliases.
- Different geometry, conflicting configured profiles and separate damage annotations remain independently selectable. Configured models are listed before unconfigured choices, with recent connection edits preferred.
- Replace 2D schematic from 3D scene appears directly beside Select measurements in the 3D well toolbar. Confirmation is required. The new image preserves the current camera, cut view and visible measurements, excluding interactive controls.
- Replacement retains the drawing ID, master well link and editable 3D configuration. Undo/Redo restore the prior and replacement drawings. Cancel leaves the current drawing intact.
- Includes the prior master-driven 3D construction, numeric connection ordering and sequential point-name improvements. Updated user guide, tutorials and all 20 supported translations.

Prepared for owner testing. Microsoft Store submission remains pending owner validation.
