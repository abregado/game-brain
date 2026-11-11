---
title: "Living World PvE Minimum Spec Proto"
source: "Game Stuff/Game Ideas/Big Five/Living World PvE/Living World PvE Minimum Spec Proto"
modified: 2015-04-14
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Living World PvE]]"]
concepts: ["Living World PvE", "Design: Depletable Resource Grid"]
words: 276
summary: "Minimum spec for a prototype: client/server, simple AI, starter vehicles, scanning beacons, movement, depletable resource grid, base."
tags: ["area/game-idea", "project/living-world-pve", "type/design-doc"]
---

Client

- on connect, receives unique ID and server ID. Adds to list

- player controls sent to the server

Server

- Handshake, give unique ID and own ID

- Simulation and client communication

- sends all players all entity locations

AI

- Simple AI

- detection radius

- move toward target list

- shoot at nearest target list

- request formation from a unit

- if nothing in detection radius then move toward a destination

- if shot then set destination to nearest point in radius to the damage dealer

Player Starter Equipment:

All players spawn in a simple combat vehicle. It can move and shoot but cannot carry anything. Players at the spawning base can change into a larger, slower combat unit, a resource collector or a transport.

Scanning Mechanics

- Players in starter bots can move around and drop a scanning beacon

- this starts a countdown and begins an attack

- If the beacon survives until the timer is complete then the surrounding area is updated

Player Movement

- Keyboard 8 way movement

- mouse aim weapons

- less than instant tracking

- acceleration to max speed

- deceleration

Map

- safe spawn area (instapop turret)

- depletable resource grid

- grid regenerates when a field is depleted

- new regen is somewhere away from players

- radius from starter base increases with each depletion

- amount of resources increases with each depletion

- two versions: real and player scanned

- player scanned version has timestamps on when area was scanned last

- players can see roughly when an area was scanned last

Base

- Unlimited Number of each robot type available
