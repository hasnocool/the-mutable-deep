# The Mutable Deep

**The Mutable Deep** is a 3D systemic fantasy simulation / CRPG sandbox built in Unity.

It combines four design traditions into one shared simulation:

- **Dwarf Fortress** — persistent world simulation, fortress management, jobs, materials, ecology and history.
- **Caves of Qud** — mutations, body consequences, strange abilities, factions and combinatorial interactions.
- **Dungeons & Dragons** — d20-style resolution, character progression, classes, skills, equipment, spells and party play.
- **Neverwinter Nights** — authored adventures, dialogue, quests, dungeons, encounters and a future Dungeon-Master/content-authoring layer.

The goal is not to reproduce those games. The goal is to create an original world where their strongest design ideas operate over the same simulation.

## Project thesis

> A player can build a living settlement, personally adventure through the same world, alter it with physical or magical systems, and leave permanent consequences that become part of the world's history.

## Start here

1. [Game Vision](docs/01_vision/GAME_VISION.md)
2. [Design Constitution](docs/00_foundation/DESIGN_CONSTITUTION.md)
3. [Architecture](docs/02_architecture/ARCHITECTURE.md)
4. [World](docs/03_world/README.md)
5. [Characters / D20](docs/04_characters/README.md)
6. [Fortress Simulation](docs/05_simulation/README.md)
7. [Adventure / CRPG](docs/06_adventure/README.md)
8. [Content Authoring](docs/07_content/README.md)
9. [Save / Load](docs/08_persistence/README.md)
10. [POC Acceptance Test](docs/09_testing/POC_ACCEPTANCE_TEST.md)
11. [Phased Roadmap](docs/10_phases/README.md)
12. [IP / Asset Guardrails](docs/11_reference/README.md)
13. [TODO](TODO.md)

## Four systems, one world

```text
                    THE MUTABLE DEEP
                           │
                    SHARED WORLD STATE
                           │
       ┌───────────────────┼───────────────────┐
       │                   │                   │
    FORTRESS            CHARACTER           ADVENTURE
       │                   │                   │
 Dwarf Fortress      D&D-style rules      NWN-style quests
       │                   │                   │
       └───────────────────┼───────────────────┘
                           │
                     MUTABLE SYSTEMS
                           │
                    Qud-style weirdness
```

## POC scope

The first playable slice is intentionally small:

- 64×64×32 editable 3D region
- 8–12 simulated dwarves
- four adventurers
- four factions
- ten creature types
- ten spells/abilities
- eight mutations
- one multi-level cavern/dungeon
- one authored quest
- one ancient structure
- one emergent faction event
- save/load + deterministic verification

## Development principle

**Simulation first. Rendering second.**

The authoritative simulation should be able to tick, test, save, load and replay without requiring every entity to exist as a Unity GameObject.

## Repository map

```text
the-mutable-deep/
├── README.md
├── TODO.md
├── AGENTS.md
├── docs/
│   ├── 00_foundation/
│   ├── 01_vision/
│   ├── 02_architecture/
│   ├── 03_world/
│   ├── 04_characters/
│   ├── 05_simulation/
│   ├── 06_adventure/
│   ├── 07_content/
│   ├── 08_persistence/
│   ├── 09_testing/
│   ├── 10_phases/
│   └── 11_reference/
└── project/
```

## Initial implementation target

Unity 6000.6.3f1 + URP for the prototype, with a simulation/presentation boundary that allows conventional C# first and measured Jobs/Burst/ECS optimization later.
