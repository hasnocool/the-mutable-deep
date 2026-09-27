# Determinism, Correctness and Performance

## Determinism tests

- same seed → same generated terrain hash
- same seed + command stream → same critical world hash
- save/reload → same continuation hash
- different seeds → materially different worlds

## Rule tests

Cover d20 rolls, advantage/disadvantage, damage mitigation, hit locations, conditions, jobs, needs thresholds, mutation effects and quest transitions.

## Property-style tests

Examples: destroyed terrain cannot remain solid; dead entities cannot receive normal AI jobs; item ownership cannot point at missing entities; a completed quest cannot revert without an explicit migration/reset.

## Performance gates

Measure tick duration, allocations, pathfinding latency, mesh rebuild time and memory. POC target: comfortable 4× simulation speed on a development desktop with 100–250 active entities.

Do not optimize by assumption. Record benchmark results before/after performance changes.