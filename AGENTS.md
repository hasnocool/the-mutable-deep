# Agent / Contributor Instructions

## Source of truth

`TODO.md` is the active execution list. Phase specifications in `docs/10_phases/` define acceptance criteria.

## Core rules

1. Keep simulation logic independent of rendering where practical.
2. Prefer deterministic systems over frame-dependent behavior.
3. Use stable integer/entity IDs rather than GameObject references in persistent state.
4. Avoid putting business rules in MonoBehaviours.
5. Do not add a feature to the POC unless it demonstrates one of the project's core pillars.
6. Keep content definitions data-driven.
7. Add tests for rules that affect save/load, simulation determinism, or gameplay-critical calculations.
8. Optimize after measurement. Avoid speculative ECS/Burst complexity before a benchmark identifies a bottleneck.

## Required handoff format

When completing a unit of work, update:

- `TODO.md`
- relevant phase acceptance criteria
- relevant architecture decision if a design changed
- tests
- documentation for public/runtime-facing contracts

## Naming

Use PascalCase for C# types, camelCase for local/private fields where Unity/C# conventions permit, and explicit domain names. Avoid generic names such as `Manager`, `Data`, or `System` without a domain qualifier.
