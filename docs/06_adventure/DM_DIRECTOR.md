# Dungeon Master Director

The DM Director is a future orchestration layer that creates situations rather than rigidly scripting outcomes.

## Inputs

World state, player power, unresolved threats, recent history, faction tensions, known locations, resource scarcity, and pacing goals.

## Outputs

Quest seeds, encounter seeds, rumors, NPC goals, complications, rewards, and escalation events.

## Guardrails

The Director proposes events. The simulation validates legal effects. It must never teleport state or bypass rules merely to force a story beat.

## Example

```text
Threat = Goblin pressure
Fortress = short on guards
Player = returning from cavern
Director proposes = night raid
Simulation resolves = raid path, defenders, casualties, theft, retreat
History records = Battle of the Lower Gate
```

## Long-term

Support authored modules, procedural campaigns, replayable scenarios and human-authored DM content without requiring one monolithic quest script.