---
title: "Dungeonizing OPR Quest"
source: "Game Stuff/Dungeonizing OPR Quest"
modified: 2024-09-14
type: design-doc
area: wargame
status: "designed"
projects: ["[[Other Wargames]]"]
concepts: ["Dungeonizing OPR Quest", "Design: Dynamic Enemy Spawning"]
words: 1534
summary: "Rules for randomised dungeon-style play with One Page Rules Quest using the Warhammer Cursed City tiles: tile exploration, exit counters, awareness and spawning, objectives, monster waves, neighbourhood setup."
tags: ["area/wargame", "project/other-wargames", "type/design-doc"]
---

# My Goal with this

Simulate the feeling of airship based guerrilla warfare on a town controlled by vampire overlords.

Create a complete campaign (3 chapters with 2 missions each and a Finale) that utilises all of the models in the Cursed City box.

Supply list agnostic rules for randomised dungeon adventures with OPR: Quest

Balance for Difficulty 2 play only

#  

# Component Descriptions

Cursed City Exploration Cards

Exit Counter = numbered exit token

Exit Door Marker = red door token

Door Marker = open/closed door token

Search Token = silver triangle token

Objective marker = gold triangle token

# Using Tiles

Tile = 1 board depicting a room

Square = 1 grid position on a tile

Two models with 25mm bases can be in the same square.

Halve all distances from OPR.

Models can move diagonally, except around corners.

All squares that touch a Door Marker are considered adjacent.

When Charging, the player decides which adjacent hexes they are engaging. They may engage all of them if they wish.

Line of sight extends from adjacent squares until Door Markers. Squares adjacent to Door Markers can also be seen, unless the door is closed.

# Setup for Dungeon Style play

Draw 2 Exploration cards to form the starting dungeon. The first room only gets one door, no token and the heroes are placed here. Also place the Exit Door Marker with the first Exit Counter on it. Place the one unit of the sentries in the other room, and otherwise set it up the same as below, skipping the Scouting step. Additional sentry units are set up as per the Awareness section.

# Exploring a new room

End of Round, if a hero is next to a door and wants to open it:

1.  Scouting

2.  Room Tile

3.  Exit Door Marker

4.  Other Doors

5.  The Red Dot

6.  Sentries

## Scouting

Take a Skill Test to search without detection.

## Room Tile

Draw an Exploration card and place it. Roll a D6 to determine which side of the shown Tile to use.

**Room Tile Placement:** Join it to the previous Door Marker via one of the points shown on the card. Use common sense and fit the Tile to your table space. If possible, place the Tile so the Exit Door Marker will be as far from any existing Exit Door Marker as possible.

## Exit Door Marker

Decide if an Exit Door Marker is here.

- There is an exit portal down on the card

- There is an exit portal number on the door that just opened

- The position is 18 tiles away from any other exit

If so, then place an Exit Door Marker in the shown place and one of the Exit Counters on top of it.

## Other Doors

If there are no Exit Counters to distribute, skip this step.

Roll D6’s for each Door Marker on the card.

For each 4+, place a Door Marker.

If any Exit Counters then minimum Door Markers you can place is 1.

**Door marker placement:** Place Door Markers in positions shown on the card. Always try to place one Door Marker at the farthest option from the entrance.

Split any Exit Counters between the new Door Markers, starting with the furthest from any Exit Door Marker.

## The Red Dot

If there are no Red Dots on the exploration card, then skip this step.

Start with the furthest red dot on the card. Stop as soon as one condition is filled

If there is an Exit Door Marker then it must be a Search Token, if any are left.

If 9 tiles away from all Exit Door Markers then it is an Objective Marker .

If there is already an Objective Marker in this room, it is a Search Token.

If there are no Door Markers, then roll. 4+ it's a Search Token, otherwise it is an Objective marker

If none of the above, place a Search Token.

## Sentries

Remove one token from the Patrolling unit with the least counters whose counters match an Exit Counter in this room. If this leaves them with no counters, they are placed into the room.

# Awareness and Spawning

## What do I want to achieve with this section?

There should always be something to fight.

The tension should increase as time goes on

The players must be able to see the tension grow

If you have a new enemy model you want to use, it should be guaranteed to spawn

## Notes

PHC = percent hero cost

End of turn process

1.  Awareness

2.  Spawn Wave

## Alerted State

Once an enemy unit has line of sight to an enemy, it gains an Alerted Token. Units with an Alerted token have an AI Goal of the nearest hero.

## Awareness

Roll Awareness. If the total is 6\*D then a wave spawns. If you have a boss wave prepared, spawn this first.

## Spawn Wave

Create a Reinforcement Wave using your preferred method.

Roll for each unit. 1-4 to determine which Exit Counter. 5-6 you pick.

If the Exit Counter is on top of an Exit Door Marker, the unit spawns there.

If the unit has Ambush, then it spawns immediately at the Door Marker that has the Exit Counter.

Leave the unit off the board and add D3 Exit Counters to them, of the same number as their rolled Exit Counter. If this unit is worth 100 PHC or more, then roll 2D3.

If 0 is rolled, then the unit spawns from the Door Marker with that Exit Counter immediately.

**Alternate ways**

Place tokens on the Exit Counters. When Awareness is reached, remove one and spawn a random group. This way you dont know what is coming, only that something is coming from that direction.

# Dungeon Style Objectives

## Area Search

A hero can choose to start the mission at the end of the turn while adjacent to any Objective Marker. Add three Door Markers to this tile. When exploring these Door Markers, place a Primary Objective Token instead of completing the Red Dot step. Heroes may use a skill action whilst adjacent to one of these markers, and if they pass a Wil test, replace the marker with a Secondary Objective marker and roll

one die. On a 5+, or if it was the last marker, the objective is completed.

## Investigation

A hero can use a skill action and pass a Dex test when adjacent to an Objective Marker. If passed, this marker is changed into a Secondary Objective marker. Once two markers have been converted, the objective is completed.

## Retrieval

At the start of the mission randomly determine one Exit Counter (2,3 or 4). When that Exit is placed, add a Primary Objective token to the tile as well. A hero standing on the token can pick it up by using a Skill action and passing a Dex test, and drop it in an adjacent tile if they are shaken. The objective is completed when the hero carrying the token ends its activation on the square in front of the first Exit Counter.

## Target Defense

Replace the first Objective Marker you discover with a Primary Objective token. Heroes may use a skill action (none) whilst adjacent to activate the Objective. At the end of each round in which it is activated, if a hero is on the same tile and no enemies are, then it’s seized, and it gets one token. The objective is completed once the marker has 4\*X tokens (where X is the chosen difficulty). At the end each round where the token is activated, roll two Awareness dice instead of 1.

## Clean Sweep

Explore the entire Dungeon to achieve the Primary Goal

# Monster Waves

Zombies - 35pts - 15 units

Skeletons - 55 pts - 3 unit

Vampire Knight - 90pts - 1 unit + 6x Zombie

Butcher - 135pts - 1 unit

Werewolf - 230pts - 1 unit, skip next Spawn

Rat or Bat swarm - 60pts - 2 units

# Neighbourhood Setup

Set all tiles with outdoor sides into three piles. Roll 7d6. Take one tile for each dice based on which number was rolled (1-2 Pile 1, 3-4 Pile 2, 5-6 Pile 3). Place these 7 tiles into a ring without Door Markers between them.

Place an Exit Door Marker on one tile, and a Door Marker on each of the others.

Set all spare tiles to their inside sides and roll 6d6, once again selecting from piles based on what was rolled. Set these aside and place a dice on each. Each tile should have a number placed on it from 1 to 6. One three tiles place an Objective Token, and on the other three a Search Token.

A skill action (Wil) has to be taken while adjacent to these Objective Markers to collect them. If a hero carrying them is shaken, they are dropped. If at the end of a round, all three heroes are on a single outdoor tile while all tokens are being carried, the Mission is successful.

Notes on feeling

Time pressure shown by difficulty increasing “slowly”

Awareness increases
