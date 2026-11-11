---
title: "BD - Agile EDF Game"
source: "Game Stuff/Game Ideas/BD - Agile EDF Game"
modified: 2022-04-26
type: design-doc
area: game-idea
status: "idea"
projects: []
concepts: ["Agile EDF Game"]
words: 324
summary: "Minspec/bloatspec and core concepts for a minimal Earth Defense Force style multiplayer horde shooter base built with Agile methods."
tags: ["area/game-idea", "type/design-doc"]
---

Goal: To do the minimum work to have a base in which to develop an EDF style game using Agile methodology.

**Minspec:**

- Player controller

- Level architecture

- Damage system

- 1x Enemy

  - Melee attack

  - Shooting attack

  - Hunt Behaviour

- 1x Gun

- Spawning hole

- LOD system for models and animation frames.

- Scenario scripting (enemy spawning)

- Multiplayer / Splitscreen

- Menu

  - Class/weapon selection

  - Respawn position selection

  - Host/Join

  - Controls

- Proto should be able to handle 100-200 active enemies

**Bloatspec aka add later**

- Destructible terrain/buildings

- Player Classes

  - Heavy

  - Flying

  - Support

  - Transformer

  - Melee

- Guns guns guns

- Knockdown/Temp Ragdoll on players and enemies

- Vehicle type (controller, prefab for type)

- Procedural animation for insects and bendy bois

- Unlock system

- Level up system

- Powerups

- More Scenario events

- Friendly Troop AI

**Core Concepts**

Every game is Multiplayer, you just have to open it.

Hot Join wherever you are.

Starting a new game just takes you to an “empty” level that is “already finished”

Change class/weapons during a mission

Respawn during a mission

Select a new mission when you finish a mission

Humanoid Controller

- Move, Strafe, Jump, Dodge

- Dodge should not be faster than walking

- Sprint forward, can’t shoot, unlimited stamina.

Basic Enemy Hunt AI

- Move toward a player

- Track number of enemies hunting each player

- Spread enemies out between players

- Dont come within a minimum distance, create a circle around players.

Basic Enemy Jump AI

- Same as hunt AI, but only updates when it lands

- Picks the next point to jump to

- Fires and then jumps

- Then recalculates the next position.

- “Stay at range” AI

**Systems**

Block of health that cant be healed

Block of Armour that can be repaired

Block of shield that self repairs

Clip ammunition, but unlimited reloads
