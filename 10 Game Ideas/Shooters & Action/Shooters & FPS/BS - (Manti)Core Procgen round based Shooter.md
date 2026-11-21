---
title: "BS - (Manti)Core Procgen round based Shooter"
source: "Game Stuff/Game Ideas/BS - (Manti)Core Procgen round based Shooter"
modified: 2021-11-07
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Shooters & FPS]]", "[[Diablo-like Action Shooter]]"]
concepts: ["Manticore Procgen Shooter", "Diablo-like action shooter"]
words: 477
summary: "Design for a round-based extraction shooter in a procedurally generated 11x11 maze with movement items, limited-ammo weapons, enemy types and risk of losing brought resources."
tags: ["area/game-idea", "project/diablo-like-action-shooter", "project/shooters-fps", "type/design-doc"]
---

Procgen round based Shooter

Grid based maze generated.

Players spawn at a safe zone in the centre.

Every 5 minutes a game starts.

Everyone who stands in the Start Zone gets teleported together.

The maze that will be generated has more resources based on number of players.

**Step 1: generate maze**

Generate a 11x11 grid

Place 3 resource locations

Place 3 crafting locations

Place 1 “exit” on the outer edge

Pathfind from each of those 7 locations back to the middle

Add weights from locations along paths

Fill rest of area with dead ends.

**Step2: Fill map with level prefabs**

Add Enemy spawners at intersections

Add easy parkour along long straight corridors

Place resource hard parkours at dead ends.

Players have 10 minutes before they are killed automatically

Players can teleport out of the maze at any time by standing still and holding a button.

Each player chooses their equipment setup before round start.

They pay for their setup when the round starts.

They can also choose to bring resources with them, which they risk losing in the maze.

If a player dies in the maze, they lose all their items.

If a player returns from the maze, they keep only the resources they collected.

**Movement Items**

Blink ray (teleport to where you are looking)

Door keycard (open a single locked door)

Jetpack (high jump)

Multi-jump (long jump)

Mount (fast movement)

All movement items have limited ammunition that recharges slowly.

**Weapons**

Sticky grenade launcher (aoe)

Freeze ray (immobilizes an enemy, no damage)

Acid Gun (causes target to take triple damage)

Railgun (big single target damage)

Lightning Gun (autohits, minor damage)

All weapons have limited ammunition. Player chooses how many reloads to bring into the maze (all are lost regardless of what happens)

**Enemies**

Basic turret guy - moves to a cover spot and just shoots at what it can see.

BarrierTank - tanky guy who makes a force field over one exit, forcing players who want to go that way to engage. Cant be damaged unless affected by Acid.

Telekinetic - pushes Sticky grenades away

Hot guy - makes nearby enemies immune to freezing

Ninja - teleports when hit, unless frozen.

Enemies do not drop anything. All enemies shoot something.

**Locations**

Long Parkour - just some jumping puzzles.

- One for each movement item, which has a shortcut that uses this item.

Spawner locations

- Has cover locations and easy parkour. No shortcuts.

Resource Locations

- While players are inside these locations, they gain resources automatically but are attacked by enemies.

Crafting Locations

- Like resource locations, but resources are consumed to create other resources.

- Players need to stand on a large area with limited cover to keep the crafting going.

Once a location is found by one player, a color tracker is drawn through the maze from that location back to the start.

Flare Gun
