# Save / Load

## Save envelope

```text
formatVersion
rulesVersion
generatorVersion
worldSeed
simulationTick
worldState
entityState
questState
history
```

## Versioning

Every save has a schema version. Loaders should migrate older schemas through explicit migration steps.

## Persist

Terrain changes, entity state, inventories, injuries, mutations, faction relations, quest state, important memories, event history and deterministic RNG state.

## Rebuild

Meshes, pathfinding caches, UI state, spawned GameObjects, VFX and other presentation caches are regenerated.

## Validation

Reject or quarantine saves with unknown critical definitions, duplicate IDs, invalid references, malformed terrain dimensions, or incompatible rules versions.

## Deterministic acceptance

`Generate → simulate 1000 ticks → save → reload → simulate 1000 ticks` should preserve a critical state hash when command/input streams are identical.