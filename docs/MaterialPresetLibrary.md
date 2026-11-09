# Material presets and shared model names

The Material editor filters AISI/SAE, ASTM, API, UNS/named alloys and generic materials. Over 130 selectable entries are grouped by alloy family. Selecting one fills the saved material designation, Young's modulus in MPa and Poisson ratio. All three fields remain editable. Reopening an assigned material preserves edited parameters rather than replacing them with catalog defaults.

The values are typical room-temperature visualization starting points. Grade labels identify the selected material; they are not a claim that an actual component meets a specification, nor a complete standards database. Condition, heat treatment, product form and temperature can affect properties. Family-level approximations are used where this preview has no grade-specific elastic data. Generic polymers and solders are explicitly labelled as generic estimates.

Reference sources used to check the catalog:

- [Outokumpu grade properties](https://www.outokumpu.com/-/media/from-sharepoint/documents/product/outokumpu-steel-grades-properties-global-standards.pdf): stainless grade names and typical moduli.
- [Special Metals Alloy 718](https://www.specialmetals.com/documents/technical-bulletins/inconel/inconel-alloy-718.pdf) and [Alloy K-500](https://www.specialmetals.com/documents/technical-bulletins/monel-alloy-k-500.pdf): nickel-alloy elastic properties.
- [Indium Corporation](https://www.indium.com/blog/how-soft-is-pure-indium/), [Goodfellow indium foil](https://www.goodfellow.com/usa/indium-foil-group) and [Goodfellow lead](https://www.goodfellow.com/eu/material/metals/lead): soft-metal values.
- [API 5CT addendum](https://www.api.org/-/media/Files/Certification/Monogram-APIQR/0_API-Monogram-APIQR/Advisories-Updates/Addenda-Errata/API_Spec_5CT_11th_Edition_Addendum_1_20250521.pdf) and [Nippon Steel API grade list](https://www.tubular.nipponsteel.com/octg-material/application-list/api): API grade designations.

## Rename behavior

Names are display metadata attached to the existing P/N and model hash. Mesh aliases use stable mesh ordinals, CAD node aliases use hierarchy paths, and motion-group renames retain their group keys. Renaming does not rewrite CAD bytes, mesh membership, motion limits, physical properties, connection identities or saved motion readings. A renamed mesh also updates an associated single-mesh motion label. Contact selectors, tree leaves and new motion definitions use one shared display-name function. Visible mesh ordinals distinguish equal names.

The existing canonical revision, Undo/Redo, conflict rebase and native merge paths carry the names. Independent aliases rebase by key; competing changes to the same alias require review. Projects containing names or physical materials require reader 1.19.29. Existing connection-only projects retain their prior reader floor.

The model tree occupies a separate pane between attachments and the viewport while mesh selection is active. Its scrollable height follows the available model area. Mesh context menus have a height limit and placement constrained to the owner window. Both contact selectors apply temporary hover emphasis using stable mesh IDs and restore normal appearance on leaving or closing.
