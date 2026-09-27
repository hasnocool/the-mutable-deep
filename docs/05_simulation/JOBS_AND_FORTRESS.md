# Jobs and Fortress Simulation

## Job flow

```text
World need/designation → Job created → Candidate scoring → Claim → Path → Work → Output → Event
```

POC jobs: Mine, Haul, Build, Farm, Cook, Craft, Guard, Heal, Sleep, Eat, Socialize.

## Fortress systems

Rooms, workshops, stockpiles, beds, farms, storage and simple defensive positions are represented as simulation structures.

## Stockpiles

A stockpile stores filters and capacity. Haulers choose jobs based on distance, urgency and skill.

## Room detection

Use enclosed-space analysis to identify rooms; furniture and fixtures infer purpose.

## Citizen autonomy

Citizens choose jobs from available work according to skills, needs, traits and proximity. Player priority settings influence scoring rather than directly puppeteering every citizen.