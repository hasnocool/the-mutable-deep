# Runtime Data Model

## Identity

Every persistent entity receives a stable `EntityId`.

Suggested representation:

```text
EntityId: uint64
WorldId: uint64
ContentId: string
```

## Component categories

### Physical
- Position
- Facing
- Movement
- Containment
- Occupancy

### Character
- Attributes
- Skills
- ClassProgression
- Body
- Health
- Needs
- Traits
- Memories
- Relationships
- FactionMembership

### Object
- ItemDefinition
- MaterialInstance
- Durability
- EquipmentSlot
- Ownership

### Simulation
- JobAssignment
- AIState
- CurrentAction
- Cooldowns
- StatusEffects

## Immutable definition vs mutable instance

```text
Definition
  → static authored data

Instance
  → runtime mutable state
```

## Persistence rule

Serialize stable IDs and authoritative runtime records. Do not serialize Unity object references, mesh instances, path caches, or other rebuildable presentation state.
