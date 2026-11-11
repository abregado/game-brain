---
title: "Conundrum - When to evolve"
source: "Game Stuff/Game Ideas/Big Five/Living World PvE/Conundrum - When to evolve"
modified: 2021-06-15
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Living World PvE]]"]
concepts: ["Living World PvE", "Design: Evolving AI Opponents"]
words: 519
summary: "Design problem and four options for when CPU players mutate in Living World PvE, based on player actions, respawn, ratings and sorties."
tags: ["area/game-idea", "project/living-world-pve", "type/design-doc"]
---

The CPU players have their settings mutate at various points during the game. But when?

Aim:

- The players can “tend to the garden” of CPU types to cultivate particular ones in an area.

- The game state reaches a stable equilibrium of difficulty.

- The difficulty returns to an easy state if the players are pushed back.

Requirements

- **PLAYER ACTION MUST DETERMINE WHEN A CPU MUTATES**

- Mutation does not necessarily mean the CPU becomes better.

When to Mutate?

The big question.

What does To Mutate mean?

Mutation of a CPU does not mean that it will be automatically better. Mutation only occurs slowly, so forcing a CPU to mutate will result in a new version that is similar to the old.

Gameplay background

CPU base locations are fixed in the world. They can be destroyed, and then players can build a new base on top. If players do not utilize the base location, then the CPU respawns at some point. The time it takes to respawn needs to be balanced so that it is an interesting choice to destroy a CPU simply to have a period of relative safety in the area around the build location.

CPU location become active in two ways:

- The players build a base on a base location “adjacent” to this CPU.

- The players are actively harvesting resources in the area protected by the CPU.

If players deconstruct all adjacent bases, and stop harvesting near to a CPU, it will return to a dormant state.

Option 1: The CPUs mutate when they respawn, but never “clone”

If a CPU only mutates when it respawns, then players can cultivate easy CPUs by simply not destroying them very often. If players find a very tough CPU, they will want to destroy it a lot until it mutates into a less effective CPU.

Option 2: The CPUs mutate over time, and get reset to the best current CPU on destruction.

If a CPU is active, then it mutates on a timer. This will result in CPUs eventually becoming different. Each CPU is ranked in some way. When a CPU is destroyed, then its parameters are overwritten by the most effective CPU template that is still in use. This promotes players only destroying CPUs that have mutated to become more powerful, as destroying easy CPUs will just result in them becoming more difficult.

Option 3: As Option 2 but the CPUs are graded and stored on Destruction.

When respawning, a CPU gains the traits of the most highly rated CPU that was previously destroyed. This promotes players to never destroy the most dangerous CPUs, as they would be added to the resurrection pool.

Option 4: CPU Sorties

CPUs move from the Pool, to an active CPU location for a period of time. During their time, they are rated based on their performance against the players. High rated sorties allow the CPUs to mutate. Very poor rated sorties result in deletion. This promotes players to destroy CPUs when they become troublesome, so that their scores are lower, resulting in less chance of mutation and reproduction.
