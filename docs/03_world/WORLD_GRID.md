# 3D World Grid

## POC dimensions

`64 × 64 × 32` cells, divided into reusable chunks.

## Cell state

```text
terrainId
materialId
solid/air
fluidId + amount
temperature
light
occupantEntityId
structureId
flags
```

## Terrain rules

Every cell exposes traversability, hardness, support, opacity, and interaction tags.

## Chunking

Use chunk-local arrays and dirty flags. Terrain edits mark the affected chunk plus neighboring mesh/pathfinding regions. Rendering caches are rebuilt asynchronously from immutable snapshots where practical.

## Vertical play

Z-levels are first-class. Stairs, ramps, shafts, caverns, bridges and vertical visibility are required by design.