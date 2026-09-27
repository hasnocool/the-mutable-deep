# Bodies, Injuries and Mutations

## Body tree

```text
Head
Torso
├── Left Arm
├── Right Arm
├── Left Leg
└── Right Leg
```

Each part tracks health, armor, conditions, capabilities and equipment relationships.

## Injury pipeline

`Damage → Hit Location → Mitigation → Part Damage → Condition → Capability Change`

Example: severe right-arm injury can prevent two-handed weapon use and reduce shield control.

## Mutation model

Mutations are effect bundles that add capabilities or change body/environment rules.

POC: Extra Arm, Night Vision, Regeneration, Stone Skin, Chitin Armor, Acid Spit, Telepathy, Photosynthesis.

Prefer tradeoffs and behavioral consequences over pure statistical upgrades.