# Materials and Environment

Materials are data-driven.

```text
Material
├── density
├── hardness
├── toughness
├── flammability
├── conductivity
├── meltingPoint
├── temperatureRate
├── tags
└── appearance
```

POC materials: stone, dirt, wood, copper, iron, steel, bone, glass, water, web.

Material properties drive tools, armor, damage, construction, fire and environmental reactions. A material should not require bespoke code merely to behave differently.

Environment channels: temperature, light, smoke placeholder, fluid amount, support, contamination. Advanced simulation is deferred until benchmarked.