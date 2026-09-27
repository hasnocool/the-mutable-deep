# World Generation

## POC generator

Input: `worldSeed`.

Pipeline:

```text
Seed → Surface Height → Rock Layers → Soil → Caverns → Ore Veins → Water Pockets → Vegetation → Creatures → POIs
```

## Deterministic generation

Generation must be reproducible from seed + generator version.

## Geology

POC rock layers: granite, slate, limestone, sandstone. Ore: copper, iron, coal.

## Caverns

Generate at least one large connected cavern below the starter fortress and several smaller disconnected pockets.

## Future

Region streaming, civilizations, climate, rivers, biomes, ruins, ancient roads, world history and multi-scale simulation.