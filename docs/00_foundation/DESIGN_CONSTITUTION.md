# Design Constitution

## 1. The world is the source of truth

Actors, items, structures, terrain, factions, quests, and history exist in simulation state. Rendering presents that state; it does not define it.

## 2. Consequences persist

Important actions must be capable of producing persistent consequences: injuries, deaths, destroyed buildings, faction changes, discovered locations, altered terrain, and historical records.

## 3. Systems should compose

Prefer reusable primitives:

```text
Effect
Condition
MaterialProperty
Ability
Action
Reaction
Event
```

The goal is for new content to combine existing primitives rather than requiring custom code for every interaction.

## 4. Authored and emergent content coexist

An authored quest can operate on the same world state as emergent events. Procedural generation should not invalidate authored content.

## 5. Simulation detail is scalable

Near the player, simulation is detailed. Far away, it may use lower-resolution simulation. The conceptual world should remain continuous even when implementation detail changes by distance.

## 6. Failure creates stories

A failed job, injury, flood, mutation, betrayal, or destroyed workshop should be a valid outcome, not necessarily a bug state.

## 7. Player agency over scripted correctness

The player should be able to solve problems using unexpected combinations of movement, terrain, equipment, social actions, magic, and physical systems.

## 8. Original IP

The project uses inspiration from established games and tabletop concepts but must create original setting, characters, art, dialogue, lore, and implementations.
