# Spells and Effects

## Common effect primitives

```text
Damage
Heal
Condition
Add/RemoveTag
ModifyAttribute
CreateEntity
DestroyEntity
MoveEntity
ModifyTerrain
ModifyFluid
ModifyTemperature
Ignite
Teleport
Reveal
```

## POC spells

Fire Burst, Create Water, Stone Shape, Heal, Web, Light, Frost Bolt, Shock, Mist Step, Detect Life.

## Spell resolution

A spell validates resources and targets, then emits effects into the simulation. Visual VFX are observers of successful effects, not the source of truth.

## Systemic examples

Fire Burst can ignite wood. Create Water can extinguish fire. Stone Shape changes terrain. Web creates a blocking/slowing material. Detect Life modifies the viewer's knowledge state.

## Extensibility

Every effect should have deterministic parameters, target rules, duration, source entity, tags and reversible/terminal semantics where applicable.