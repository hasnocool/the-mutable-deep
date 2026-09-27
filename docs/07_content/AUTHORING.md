# Content Authoring

Use stable IDs and composable data definitions.

```text
characters
creatures
items
materials
abilities
spells
mutations
buildings
rooms
factions
quests
dialogue
encounters
events
```

ScriptableObjects are appropriate for static authored definitions. Runtime state is stored separately.

## ID examples

`creature.cave_beast`
`ability.fire_burst`
`mutation.extra_arm`
`quest.missing_miners`

## Tags

Examples: `flammable`, `metal`, `underground`, `humanoid`, `construct`, `arcane`, `edible`, `poisonous`, `holy`, `hostile`.

## Validation

Editor validation should catch duplicate IDs, missing references, invalid parameters, unreachable dialogue/quest nodes and circular prerequisites.