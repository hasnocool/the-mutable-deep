# Phase 00 — Foundation

## Objective
Create the smallest executable simulation shell with deterministic time, IDs, commands, events and tests.

## Deliverables
- Unity project
- Simulation assembly
- Entity registry
- Fixed tick loop
- Seeded RNG
- command/event interfaces
- basic UI showing tick/seed/entity count
- save envelope

## Exit criteria
A headless test can create a world, tick 1000 times, produce the same hash twice, save, reload, and continue deterministically.

## Explicit non-goals
No voxel art, large AI, combat, complex UI or multiplayer.