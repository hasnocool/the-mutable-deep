# Fluids, Fire and Physical Reactions

## POC model

Use cellular/region flow approximation rather than a full physics solver.

### Water

Moves into adjacent lower cells, fills bounded spaces, extinguishes simple fire, and changes traversal.

### Fire

Tracks heat, fuel, spread probability and lifetime. Flammable materials become fuel; nonflammable materials can conduct heat without burning.

### Other reactions

`Web + Fire → burn`

`Oil + Fire → high heat`

`Water + Hot Surface → steam placeholder`

`Acid + Armor → durability loss`

The purpose is systemic consequence, not physical simulation fidelity.