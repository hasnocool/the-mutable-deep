# Architecture

## High-level layers

```text
Presentation
    ↓ commands/events
Application / Game State
    ↓
Simulation Core
    ├── World
    ├── Entities
    ├── Jobs
    ├── AI
    ├── Combat
    ├── Magic / Effects
    ├── Economy
    ├── Factions
    ├── Quests
    └── History
    ↓
Persistence / Replay / Tests
```

## Unity boundary

Unity owns rendering, scene lifetime, input binding, audio/VFX, UI, asset loading, and presentation animation.

The simulation owns positions and state, terrain state, jobs, actions, health, inventories, relationships, world events, and quest state.

## Command/event split

Player/UI systems issue commands such as `DesignateMine`, `BuildStructure`, `MoveParty`, `UseAbility`, `TalkToNpc`, and `AcceptQuest`.

Simulation systems emit events such as `MiningCompleted`, `CharacterInjured`, `CreatureDied`, `FactionRelationChanged`, `QuestObjectiveCompleted`, and `RoomDiscovered`.

## Entity views

A Unity `GameObject` represents a view of an entity, not the entity itself. Views can be unloaded/rebuilt without losing simulation state.
