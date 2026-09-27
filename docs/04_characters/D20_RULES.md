# D20-Compatible Rules Layer

The prototype uses a familiar d20-style rules service while keeping the overall simulation original and implementation-independent.

## Core resolution

```text
D20 + modifier + proficiency
        vs
Difficulty Class
```

Attack resolution compares an attack roll with the target's defense.

Damage then passes through armor, resistance/vulnerability, hit location and conditions.

## Roll modes

`Normal`, `Advantage`, `Disadvantage` are first-class resolution modes.

## Classes

POC classes: Fighter, Rogue, Wizard, Cleric. They are progression data packages rather than large inheritance hierarchies.

## Rules boundary

Use the applicable current System Reference Document for any implementation deliberately using published D&D mechanics. Do not include proprietary setting text, adventures, characters, artwork or non-SRD prose.