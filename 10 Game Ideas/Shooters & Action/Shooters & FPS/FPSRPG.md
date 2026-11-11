---
title: "FPSRPG"
source: "Game Stuff/FPSRPG_"
modified: 2022-03-14
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Shooters & FPS]]"]
concepts: ["FPS RPG Prototype", "Design: Enemy Attack Director"]
words: 295
summary: "Minimum element list for a first-person shooter RPG prototype in Unity: HP as spell cost, ScriptableObject abilities, cuboid level, enemy volumes and an enemy attack director."
tags: ["area/game-idea", "project/shooters-fps", "type/design-doc"]
---

**Minimum elements**

HP counter

Action bar UI visuals

Select with numbers and mousewheel or controller bumpers

Player controller

Left click to activate ability

Spacebar to jump

Main Level with Progrids

Rest of level made with cuboids that can be affected by spells.

Level contains volumes where enemies can appear.

Player abilities as ScriptableObjects

- Cost to cast (in HP)

- Prefab of projectile or effect

Enemies that have a random length timer. After the timer is up, they either:

- move to a new spot in their current volume

- stay put

- Move to a new volume

Enemy attack director, which has a timer. Maintains a list of enemies, and which ones can see the player.

Tracks when an enemy has fired at the player. Doesnt allow too many enemies to fire in quick succession.

- Logic

  - Randomly select one enemy which could see the player last frame.

  - Check if it can see the player.

  - If yes, fire, if not, then set the enemy as not seeing the player.

  - If no enemies available that could see the player last frame, shuffle the list of enemies that cant see the player and pick the first one.

  - Can it see the player now?

  - If yes, fire, mark it as seeing the player

  - If no, move on.

  - If no enemies can see the player then just have a random enemy fire toward the player.

- When an enemy fires, a timestamp goes into a stack.

- When the director wants to fire, it checks the queue if too many attacks have been made in recent time.

**Assets to make things faster**

- Elemental materials pack

- Some basic ball shaped meshes for enemies

- Projectile trail particle effects pack
