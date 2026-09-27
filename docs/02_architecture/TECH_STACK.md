# Technology Stack

## Engine

Unity 6000.6.3f1 is the prototype target. Keep an upgrade path toward the current supported LTS line if production hardening becomes preferable.

## Rendering

URP; stylized low-poly 3D characters; chunked voxel terrain; orthographic/isometric camera with optional orbit.

## UI

UI Toolkit for inspectors, fortress dashboards, party sheets, quest logs, and debugging tools.

## Input

Unity Input System with context-sensitive bindings for fortress, adventure, and inspection modes.

## Tests

Unity Test Framework; deterministic simulation tests should execute without requiring scene rendering.

## Data

ScriptableObjects for authored definitions; runtime state in serializable simulation records. No gameplay truth should live only in ScriptableObjects.