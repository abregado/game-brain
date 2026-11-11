---
title: "Concept - Team Shooter"
source: "Game Stuff/Game Ideas/Concept - Team Shooter_"
modified: 2013-11-25
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Shooters & FPS]]"]
concepts: ["Team Deathmatch Shooter", "Design: Server Event and Sound System"]
words: 1256
summary: "Design and task list for a 2D top-down team deathmatch shooter prototype with limited respawns, five unique weapons assigned randomly on death, scanner abilities, capture points, event system and level design notes."
tags: ["area/game-idea", "project/shooters-fps", "type/design-doc"]
---

Team Deathmatch Shooter Design

Prototype 1 Gameplay Description

In this simple team deathmatch combat game, each team has a limited number of respawns before losing. Players must be careful as dying is of much higher consequence than scoring a kill.

Each time a player dies he is given one of the 5 available weapons randomly. Each team can only have one instance of each weapon, creating an interesting mix of strategy that changes after every kill. These weapons are all unique, physics based designs. Each requires different tactics to use effectivly.

Tasks and Systems

Gameplay UI system

- ammo, weapon, charge and shotgun spread UI

- ~~team score tickers~~

- ~~hold tab to see scores and n~~ames over characters

- ~~pips for directional scanner: phase 1 only for friendlies~~

Respawn system

- ~~respawn at the closest location to all your teammates~~

- ~~weapon selection at spawn - randomised (one of each per team)~~

Sound

- event samples

Debreif screen

- Display player frags from both teams

- display winning team

- display remaining lives/respawns

- display round time

Events

- ~~addition of other event types~~

- ~~sending events that a client can “see”~~

- server tells client when victory/defeat conditions are met

Weapons and abilities

- add plasma gun, bounce gun and shotgun

- grenades must fall into pits

- link abilities to weapons

- ~~grenades only fire on press not depress~~

- ~~grenades explode faster~~

- ~~bullets spawn NEXT TO player ------ priority~~

- ~~bullets can collide with players again~~

Capture Points

- proximity detection

- countdown timer UI and mechanics

- ticker score countdown

Replenishment

- ammo points that recharge players

- healing points in player bases/spawns

Login screen

- team selection

- observer mode if a player forces a team but cannot join due to too many players

Level creation

- One map based on bens plan

- Requires all points and other level based stuff to be working first

Geometry and line of sight

- “low walls” that block everything but not line of sight

- ~~client side LOS~~

5 Weapons We Chose

### Plasma Gun

- burst fire 3 rounds at medium accuracy

- medium cooldown

- fast projectile speed for accurate target prediction

- 1 damage per round

- 15 round clip

### Bounce Gun

- projectile is medium speed

- fixed ROF at medium speed

- can bounce three times

- 2 damage per round

- 5 round clip

### Grenade Gun

- explosive AoE damage

- timed grenade detonation

- slows down fast after one bounce

- 1 damage to all targets in range

- slow ROF

- 5 round clip

### Charge Gun

- long charge time

- semi-auto at low charge

- slower ROF than Plasma Gun

- 1,3 or 5 damage per round

- very fast projectile

- variable ammo usage per shot

- 3 round clip at max charge

### Scatter Gun

- hold trigger to narrow the fire cone

- fires several projectiles

- good ROF

- 1 damage per pellet

- best close range weapon

- projectiles do not travel very far

- 10 round clip

## 5(3) Abilities we chose

### Medscanner

- Can see enemy health status

### Vibroscanner

- Can detect players behind walls

### Lifescanner

- Adds direction pips to the players hud (friend and foe)

Sound and event system

- The server tracks events and adds them to a list

- events have a range of affect and are either based on line of sight or not

- events can have sound or visual effects on the client side

- all clients within range of an event are sent the events

- events are deleted at end of frame after being sent

Event Types

- gunshots (sound effect and visual effect for sound sensor)

- impact on wall (sound and particle effect)

- impact on player (sound and particle effect)

- explosions at given location

- player movement (for sound sensor)

- capture event (juice effect)

- respawn (for spawn animation)

- ammo spawn (visual)

- ammo collection (juice effect)

- teammate/personal reload (sound and visual)

- door opening/geometry changing (trigger for map change)

Current Issues

Bullets are created just outside the area of the players hit box which allows them to be created INSIDE geometry (chainshapes and rectangles tested)

Solution 1: the player hitbox which determines wall collision is separate from the one that determines bullet collision. The wall hitbox is larger than the area in which bullets spawn.

Level Design consideration

- many loops to keep combat moving

- capture points must be fairly open and non-defensable

- if there is a third capture point it should be less valuable than the other 2

- feature rooms are designed in tiled and then fitted together

- procedurally generated connections between important locations?

- several ammo recharge stations per level 3-5? so that they do not become more important than capture points. Limited health and ammo in each

- respawn from edge of map and move inwards? secondary cost of death?

- should be a lot of places where locations can be fired apon but not moved to (using pits)

- avoid protected corridors within sight of capture locations

- minimum 3 exits from each area

Stats

- player count: 8

Philosophy

squad combinations

which ability is lacking the the enemy squad?

which ability do we lack in our squad?

weapon acquisition/selection?

respawn on half ammo/health?

respawn on low health/ammo and then recharge slowly in the spawn. Player selectable “soft respawn” times?

one of each weapon available per team

first in

5 weapons available

each player holds only one weapon

each respawn you get a random weapon (between unselected weapons)

ammunition

limited on player reloads

can recharge ammo from strategic locations on map

global cooldown per point

~2 points per map

keep ammo max low

option 2: ammo rechrages slowly

ammo stations only spawn ammo/health when players are waiting nearby and spawn per player waiting. This means that health and ammo are not items of opportunity as players cant collect them on a cycle to keep them from the enemy.

weapon stats

no reloading

fire rates

aoe/explosions

do 1 or 2 damage

one weapon can see enemy health

one weapon has direction pips

stationaryish weapon which has accuracty based on recent movement

grenade launchers, shotgun, rifle, bounce gun, plasma gun

penetrator, knock around gun, stun gun

non-lethal temp damage

wind up/fire delay/cooloff

charge up - with semi auto lower tiers. fires when it is full

overheat - plasma gun - shoot too much and effectivness is lowered

bounce gun - no speed drop - three bounces

grenade launcher - speed drop over time, speed drop after bounce - explode on timer - falls in pits - double barrel

shotgun - boo - hold button to narrow spread

burst fire

one special ability might be to have your view more zoomed out (scout maybe)

life and victory

limited respawns per team

victory when one side has no respawns

hit points, low discrete (3-5 hps)

capture points lower other team tickers

respawn in team respawn area

can always see friendly health

terrain

red and blue forcefields

walls

pits

respawn points

tasks

implement click and release inputs sent to server

timeout for player connections

victory state and effect

weapon state icon - ammo state ui

health display ui

GUI needed for action component

ammo - on ui bar

weapon - on ui bar

charge - on cursor

health - on player model

team lives - on top ui bar
