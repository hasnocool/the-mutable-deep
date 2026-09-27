# Quests and Dialogue

## Quest state

A quest is a persistent graph with conditions and effects.

```text
Available → Offered → Active → Completed
                       ↘ Failed / Abandoned
```

Objectives can reference world facts: entity alive/dead, item possessed, location discovered, faction relation, room state, or event occurrence.

## Dialogue

Dialogue nodes support text, speaker, conditions, choices and effects. Conditions can inspect reputation, memories, quest state, knowledge and world facts.

## POC quest

**The Missing Miners**: investigate a vanished mining crew, locate the cavern branch, discover an ancient sealed structure, then resolve the situation by combat, negotiation, exploration or environmental action.

## Branching requirement

At least three materially different outcomes must be possible and the world should reflect them after the quest ends.