# Movement audit for 1.19.21

The Inventory routing dialog and the new Master card call `InstallInventoryPlaced`, which applies stale source/destination checks, Replace/Append semantics and the six-item limit, then delegates to `InstallInventoryChecked` / `InstallInventory`. The duplicate-location action uses the same checked installation backend, retaining its PN correction and drawing-reference behavior.

The Master catalog reuses `StockWarnings.Category` and `EquipmentRouting.Suggested`, retaining native category identities while following visible header order. A category may include multiple matching Inventory sections, such as first/second-position wear bushings; choices show their source section. It does not guess unrelated categories from fuzzy names.

The older `TransferStockDated` Master branch previously wrote stock directly. It now retains its exact source validation and calls `TransferStockPlaced` into the same backend. Ordinary empty single-item cells keep their existing identity representation; grouped cells retain member identities. Occupied legacy destinations require an explicit Replace/Append choice.

Return-from-removal calls existing `ReturnEquipmentChecked` or `ReturnEquipmentMember`. It retains original Inventory grouping where recorded, assessment/quarantine visibility, unavailable status, original identity, custom fields, damage-clearing history and movement events. Multiple SN returns collapse into one undoable user operation. No independent installation or lifecycle state machine was added.

Menu Delete and keyboard Delete share the same confirmation. Deleting a linked Inventory member affects only that member. Cell clearing still uses the existing audited clear/edit backend. Row deletion retains its own existing confirmation; it does not imply a physical return. Cut/Copy/Paste retains existing edit semantics and sheet restrictions, independent of physical Inventory transfer. Receiving and Quarantine keep their existing checked receipt/lifecycle paths.

A grouped return is rolled back in full if a later member conflicts. The shared PN/serial conflict check also scans newly entered Master items that have not yet received a lifecycle identity; these were previously absent from the slot-based check. Clearing the last Master identifiers retires that placement in history and removes the hidden cell identity, so another item can be installed there.

Role permissions and protected-project write checks remain in the backends. New UI actions add corresponding checks and reuse the application's role menu policy. The beta well assembly is a licensed, read-only derived preview, not a stock movement or an item-damage editor.
