# Architecture Decisions

## ADR-001 Simulation is authoritative
All persistent game state belongs to the simulation, not the renderer.

## ADR-002 One shared world
Fortress mode and adventure mode never use separate copies of the world.

## ADR-003 Composable effects
Spells, mutations, weapons, materials and hazards use shared effect primitives.

## ADR-004 Real-time with pause
The world is continuous; players may pause and issue tactical commands.

## ADR-005 Profile before escalation
Start with conventional C# data structures. Introduce Jobs/Burst/ECS or custom native containers where profiling demonstrates a real bottleneck.

## ADR-006 Content IDs
Every authored definition has a stable ID so saves can survive asset reorganization.