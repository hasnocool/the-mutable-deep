# Phase 06 — Integrated Vertical Slice

## Objective

Prove that Dwarf Fortress-style settlement simulation, D&D-style character rules, Neverwinter-style party adventure, and Qud-style mutation/systemic interactions are all operating on one persistent world.

## Required content

- 64×64×32 world region
- 8–12 citizens
- four adventurers
- four factions
- ten creature types
- ten spells/abilities
- eight mutations
- one three-to-five-level cavern/dungeon
- one ancient sealed structure
- one authored quest
- one emergent raid event

## Canonical demonstration

```text
Build Fortress
→ Mine
→ Discover Cavern
→ Form Party
→ Enter Cavern
→ Dialogue
→ Combat
→ Injury
→ Mutation / Ability
→ Alter Environment
→ Discover Ancient Structure
→ Return Home
→ Faction Event
→ History Entry
```

## Success criteria

Every link in the chain operates on shared state. Consequences remain after mode switches and survive save/load. At least three different approaches are accepted for the major quest encounter: combat, social/negotiation, and environmental/systemic manipulation.