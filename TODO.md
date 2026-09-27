# The Mutable Deep — TODO

This file is the project execution source of truth. Keep it synchronized with the phase specifications.

## Status legend

- `[ ]` Not started
- `[-]` In progress
- `[x]` Complete
- `[!]` Blocked / decision required

## Phase 0 — Foundation

- [ ] Create Unity 6000.6.3f1 project using URP.
- [ ] Establish `Game/Simulation` assembly boundary.
- [ ] Establish runtime data conventions and IDs.
- [ ] Establish deterministic simulation clock.
- [ ] Add basic test harness.
- [ ] Add debug logging/telemetry for simulation ticks.
- [ ] Add first save/load schema.

## Phase 1 — World POC

- [ ] 64×64×32 3D grid.
- [ ] Block materials and terrain states.
- [ ] Chunk storage and dirty tracking.
- [ ] Procedural starter world.
- [ ] 3D voxel rendering.
- [ ] Orthographic/isometric camera.
- [ ] Digging designation.
- [ ] Basic pathfinding.

## Phase 2 — Fortress Simulation

- [ ] 8–12 dwarves.
- [ ] Entity database.
- [ ] Job system.
- [ ] Mining.
- [ ] Hauling.
- [ ] Construction.
- [ ] Inventory.
- [ ] Stockpiles.
- [ ] Beds/rooms/workshop.
- [ ] Hunger/sleep/safety/social needs.

## Phase 3 — D&D Character Core

- [ ] Attribute model.
- [ ] d20 resolution service.
- [ ] Class progression.
- [ ] Skills/proficiencies.
- [ ] Conditions.
- [ ] Equipment.
- [ ] Party system.
- [ ] Character inspection UI.

## Phase 4 — Adventure + CRPG Layer

- [ ] Adventure camera/control mode.
- [ ] Real-time-with-pause party controls.
- [ ] Melee/ranged combat.
- [ ] Basic spells.
- [ ] Dialogue graph.
- [ ] Quest state machine.
- [ ] Dungeon POI system.
- [ ] Loot/rewards.
- [ ] One authored quest.

## Phase 5 — Mutable Systems

- [ ] Body-part damage.
- [ ] Injuries and capability loss.
- [ ] Status effects.
- [ ] Mutations.
- [ ] Composable effect system.
- [ ] Fire/water/web/acid interactions.
- [ ] Material reactions.
- [ ] Faction reputation.
- [ ] Relationships and memories.

## Phase 6 — Integrated Vertical Slice

- [ ] Shared world between fortress and party modes.
- [ ] Procedural cavern.
- [ ] 4 factions.
- [ ] 10 creature types.
- [ ] 10 spells/abilities.
- [ ] 8 mutations.
- [ ] Ancient structure encounter.
- [ ] Emergent raid event.
- [ ] World history entry generated from consequences.
- [ ] Deterministic save/load verification.

## Phase 7 — Scale Gate (future)

- [ ] Benchmark 1,000 simulated agents.
- [ ] Benchmark 10,000 entities with distant simulation.
- [ ] Region streaming.
- [ ] Background simulation LOD.
- [ ] Larger world generation.
- [ ] Civilization simulation.

## Decisions to record

Use `docs/02_architecture/DECISIONS.md` for architecture decisions. Do not bury important decisions in issue threads only.
