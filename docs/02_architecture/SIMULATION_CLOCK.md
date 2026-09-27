# Simulation Clock

## Authoritative time

The world advances through fixed deterministic ticks. Rendering may run at any frame rate.

## Tick pipeline

```text
Commands → Jobs → AI Decisions → Movement → Actions → Combat → Needs → Environment → Ecology → Events → History
```

## Speed

`Paused`, `1x`, `2x`, and `4x` are presentation controls over the same tick function. Fast-forward must not change rules or RNG sequence.

## Determinism

World generation and gameplay RNG use explicit seeded streams. A `(worldSeed, rulesVersion, commandLog)` combination should reproduce a critical-state hash.

## Parallelism

Systems may later partition independent work, but ordering of stateful events must be explicit and deterministic.