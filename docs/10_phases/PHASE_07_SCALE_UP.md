# Phase 07 — Scale Up

## Objective

Increase simulation scale without replacing the game's core model.

## Benchmark gates

1. 250 active entities at 4× simulation speed.
2. 1,000 active agents with stable tick times.
3. 10,000 total entities using distance-based simulation detail.
4. Stream multiple world regions without changing entity identity.

## Optimization targets

Profile chunk storage, pathfinding, job assignment, AI frequency, event queues, history indexes, terrain meshing and persistence.

## Simulation LOD

Near entities receive detailed perception and decisions. Mid-distance entities update less frequently. Far entities may run aggregate outcomes while preserving important events, resource changes and history.

## Architecture constraint

Do not introduce a second simulation model for scale. Optimize the same authoritative model or create explicitly compatible aggregation layers.