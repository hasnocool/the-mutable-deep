# The Mutable Deep

**The Mutable Deep** is a 3D systemic fantasy simulation / CRPG sandbox built in Unity.

The project combines four design traditions into one shared simulation:

- **Dwarf Fortress** — persistent world simulation, fortress management, jobs, ecology, materials, history, and emergent stories.
- **Caves of Qud** — systemic mutations, body-part consequences, factions, strange abilities, and combinatorial interactions.
- **Dungeons & Dragons** — character progression, d20-style resolution, classes, abilities, spells, equipment, checks, and party adventuring.
- **Neverwinter Nights** — authored adventures, dialogue, quests, dungeons, encounters, companions, and a future Dungeon-Master/content-authoring layer.

The goal is not to reproduce any of those games. The goal is to build an original game where their strongest design ideas operate over the same simulation.

## Start here

1. [Game Vision](docs/01_vision/GAME_VISION.md)
2. [Design Constitution](docs/00_foundation/DESIGN_CONSTITUTION.md)
3. [Architecture](docs/02_architecture/ARCHITECTURE.md)
4. [POC Acceptance Test](docs/09_testing/POC_ACCEPTANCE_TEST.md)
5. [Phased Roadmap](docs/10_phases/README.md)
6. [TODO](TODO.md)

## Guiding architecture

**Simulation first. Rendering second.**

The world must be able to tick, save, load, test, and replay without requiring every simulated entity to be a Unity GameObject.

## Documentation map

```text
The-Mutable-Deep/
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
