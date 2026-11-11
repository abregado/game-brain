---
title: "HLC - Probe Wars (gdd notes)"
source: "Game Stuff/Game Ideas/Concept Docs/HLC - Probe Wars (gdd notes)"
modified: 2019-09-25
type: pitch
area: game-idea
status: "prototyped"
projects: ["[[Elite-like Space Flight & Trading]]"]
concepts: ["Probe Wars", "Design: Imperfect Information Scanning"]
words: 1330
summary: "High level concept and GDD notes for Probe Wars, a submarine-feel space stealth game about deducing enemy positions using imperfect probe data; includes todos, probe stats, levels, weapons, AI and phase 1 feedback."
tags: ["area/game-idea", "project/elite-like-space-flight-trading", "type/pitch"]
---

# 

# 

# 

# 

# 

# 

# 

# Probe Wars

High Level Concept

by Ben Buckton for BinaryGambit

## Introduction

Probe Wars is a drop-in/drop-out multiplayer exploration and combat game for serious space fans. Players must deduce where their opponents are using imperfect information then sneak up and strike using powerful weapons.

## Play Experience

Commander Keen has just arrived in Asteroid Belt 554. The ships sensors are completely blind due to the local dust field, and it is unsafe to engage his main drive. Knowing there are probably other scavengers out there, he deploys several long range but weak probes.

One of the probes pings a rough location of another vessel. Thankfully it seems to be moving away, not having noticed Keens ship. Three more probes are launched towards the vessel, this time much more accurate Combat Probes. The resulting information yields two possible locations for the enemy ship.

Workin on instinct, Keen heats up and fires a torpedo at the signature he feels more likely. The bright light of the anti-matter engine speeding away fills the viewscreen. Everyone in the local area will have spotted it.

A similar bright signature appears from around the other signature, heading right for Keens ship. Oh well, you can't always be right...

## Key Features

- **Drop in, Drop-out Multiplayer:** Players can play over WiFi, joining any open games at any time

- **Detailed Scanning Simulation:** Use triangulation, distance, and vector analysis to select your targets

- **Infinite Play area:** The level scales up as more players join, and shrinks again as they leave or are destroyed

- **Information Warfare:** Players must assess the information they are given from their probes, but are never told exactly where a target is.

- **Stealth Gameplay:** Employ several stealth weapons and keep your engine output low to avoid detection.

## Genre and Theme

Probe wars is a slow paced action/stealth game with strategy elements set in a futuristic world. Realism is not considered important. Thematically it is more a submarine feeling than a space feeling.

## Technology

Which libraries, engines, rendering techniques will be used to create the game?

Are there any preestablished gameplay techniques that will be used (monetization, ect)?

## Platform

Probe Wars will be available for Android devices and all Personal Computer Systems (PC, Mac, Linux). Cross platform multiplayer will be available.

## Market

What other games do the players of this game play?

What is it about this game that those players would like?

## Todos for Single Player

- AI ships can receive a wait order, or a new target

- AI ships have a range attribute, and if they detect a torp launch within that range they fire upon it

- ships move towards a torpedo launch if they detect one

- player can mark the location of fixed entities (new tool)

- overlays when launching probes to show their max/min ranges

- player ship detects all entities in a small range

- victory condition detection (all targets destroyed)

- preset levels for single player tutorial (see below)

## Todos for Multiplayer

- players spawned within a range of other players

- player join Effect (warn other players a new player has joined)

- three hit points per ship

- cluster bomb weapon

- probe to detect the type of 5 closest items, with VERY long range

- visual range around your ship

- derelict ships. player can collect them to repair

- random asteroids and other NPCs added if nothing around the new player

- derelicts respawned if taken after a set time

- limited torpedos

## Tiny/Fun Todos

- Per player grid reference system: origin as warp in point. Player client does not know players offset.

- Camera system, multitouch controls. Recenter camera.

- Asteroid belt generator (random distribution)

- One button UI (Android/Touch compatible)

- Tube display UI

- Probe placement overlays

- Show overlay on press, launch on release

- Weak Gravitational bodies

**Scanning System Ideas**

The player has a range of probe types listed down the side of the screen. Some of these are for scanning, and some for attacking. The player selects a probe type, then clicks to deploy the probe to a location.

Probes must fly to their target before deploying. One there they will update your display with their information.

Probe Stats:

- Ping or Active/Constant type

- Ping repeat Time

- Display refresh time

- Display

- Max Range, Min Range

- Detects closest or Furthest Target

- Total Targets Tracked

- Detects Distance or Direction (cone or disk)

- Accuracy at 0, Accuracy at Optimal, Accuracy at Max

- Accuracy Curve

Probes never say exactly where a target is,

**Levels (Single Player)**

1)  The Player is in a fixed location and must locate stationary objects

2)  The Player can move around and must locate some slowly moving objects, while avoiding randomly moving, non-tracking obstacles

3)  The Player can move and must locate some fast objects, while avoiding some slow objects that will track him.

4)  The Player must engage with hostile forces which will track down and kill the player

**Multiplayer**

This level would be a new take on a Battleship style game. Multiple players must use the probes to track eachother down in realtime, while finding holes in the enemies scanning network.

Later Levels could include a capture the flag style combat, perhaps with more players per team.

When a player is destroyed, his ship leaves wreckage which floats away, and can trigger other probes.

Each player can only have a set number of probes active at once. Information is not shared between players on the same team.

Other Sensor Ideas

A expanding wave that detects targets as it collides with them, but the signals are delayed by the distance from the target. Can detect many targets, but suffers from high latency.

Type identifier probe. Multiple targets, very short range,no min range. Displays type only, not distance or Direction.

Names appear next to probe

Signature size shown at "expected" location, modifed by probe scan radius.

Weapons

Torpedo: accelerates slowly for some time before engaging main thrust. Visible to all once main thrust engaged. Explosion visible to all. Small explosion, one hit kill. Explosion. Code as a MIRV missile, one stealth trop which generates another non stealth torp, which generates an explosion.

Stealth Torpedo: same as above but engages engine much later.

Drone pod. Accelerates slowly but is not visible. Detectable by probes very accuratly. Large explosion but minimal damage.

Decoy. Moves to position then mimics a player ship.

Client server stuff

Client displays 100% accurate results

Server provides inaccurate results

Server gives list of ents and probe results, both are innacurate.

If multiple entities pings are placed very close to eachother, thier position is averaged.

Feedback from Phase 1

Precise Probes should last longer so you can see the target fade if hit

Recharge not based on time, as it makes for player downtime

Split torp and probe recharge

probes launched counter / efficiency rating given at end

Respawn enemies

Explain minimum range - overlay on the first probe landed

Explain arc signals

Single player AI ideas

Enemy ships move toward a random location around the player when he fires a torpedo. If an enemy ship moves very close to the player then a warning will appear that he is being boarded. He will suffer some damage to his ship and then evacuate using FTL to a random point on the map (minimum distance travelled). The exit point will be known to all players and again the enemies will update their target. The player must now move out of the exit zone to try and evade the enemies.

Enemies that are in range of their target will begin a countdown. If reached then the ship will go back to being inactive.

If a new target appears that is closer than the current target, enemies will switch to the new target.

Players have 3-5 hits before they are destroyed.
