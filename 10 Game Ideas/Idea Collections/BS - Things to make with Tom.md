---
title: "BS - Things to make with Tom"
source: "Game Stuff/Game Ideas/BS_ Things to make with Tom"
modified: 2024-07-21
type: planning
area: game-idea
status: "prototyped"
projects: ["[[Pipe Game - Piperspace|Pipe Game / Piperspace]]", "[[Space Station 13-14|Space Station 13/14]]", "[[Playdate & Small Games]]", "[[Coop Station]]", "[[Kobold]]", "[[Emerge]]", "[[RTS Ideas]]", "[[Shooters & FPS]]", "[[Couch Co-op & Party Games]]", "[[Game Jams]]"]
concepts: ["Things to Make with Tom", "Pipe Game / Piperspace", "Coldsleep Crew", "Games to Clone in One Year", "Barostation 2D Prototype", "Kobold", "Emerge", "RTS Prototypes", "Asymmetric Lane RTS", "Pitchable FPS Environments and Movement", "Co-op Game Ideas List", "Galcon-like Infrastructure Game", "Offline Games", "Quirky Tech Games", "Hacknophobia-like Action Game", "Ludum Dare"]
words: 1744
summary: "Dated log (Feb-Jul 2024) of project planning with Tom: constraints, lists of coop/offline/quirky ideas, games to clone, RTS prototype list, pipe/node game dev notes, 2D Baro station prototype, pizza cat jam proto, pitchable FPS ideas."
tags: ["area/game-idea", "project/coop-station", "project/couch-co-op-party-games", "project/emerge", "project/game-jams", "project/kobold", "project/pipe-game-/-piperspace", "project/playdate-small-games", "project/rts-ideas", "project/shooters-fps", "project/space-station-13/14", "type/planning"]
---

# 10.07.24

Next jam proto

“PIZZA CAT” is at the start.

Doors leaving area “non-airlock style”

Next areas activate a timer on event On entered sector

Each sector has

- Life support input

- Multiple exit airlocks to other sectors

Some sectors have a machine for the Pizza Cat

Some sectors have multiple life support outputs

Some sectors have only outputs which can be used in a machine to make life support

- RNG sectors

# 09.07.24

Things that need to be constantly on:

- Doors (Opening up new areas)

  - The doors have theme to show the “biome”

- Powering up machine slots

- Tools (pipe vision, only in radar range)

  - Multipipe pipe tool

- Fast travel options (teleporter/futurama pipes)

- Quest required areas

- Life support for a new area (remove or lengthen timers)

- Mini-map/Map/Compass (per area, radars?)

- Upgrades for the map

  - Compass

  - Player locator

  - Road signs

  - Waypoint marking

  - Show machines

Resource sinks

- Powering up view modes and tools in certain areas

# 22.06.24

What does it need?

Progression. Currently everything is there at the start. It is overwhelming. Players need to do a small thing first and get rewarded with a bigger thing.

Visual and Audio feedback. Attaching pipes sound and animation. Machines should do something when they are working. The sound scape should grow. What is the constant sound you hear to reinforce that things are working?

TODO ideas

\- toolbar or supertool?

\- networking

\- environment design (interior / exterior)

\- pipe colours

\- full tower extend

\- colliding pipes can't be placed

\- door or bridge that activates on some condition

\- proper bucket model

# 21.06.24

Pipey Nodey System game

**Tom**

Bucket

Connect pipes to simulation

**Ben**

Merge

Pipeends delete themselves when not connected

Move object tool

Fix pipe end hologram issue

Machine Ideas

“Bucket”

- While connected, a float goes up

- When the float is above 0 it outputs something

- input/output/buffer

- Fill it up, take it someplace else

“Underground pipes”

Machine socket “PlacementTargetProvider”

Pipe rail (offsets need to not be shit)

Tower for middle of room

Interaction concepts

# 07.06.24

Tycoon

“City Builder”

# 04.06.24

2d Barostation Prototype

Unity

Tilemap with colliders for station. Rigidbody attached.

Player moves inside the station without physics, based on screen direction. Relative position to ship is fixed when letting go of the controls.

Asteroids fly at the station to give it momentum

Station tries to right itself (use Kobold stabiliser code)

Unity rigidbody for netcode n players (no lobby)

# 04.06.24

Games we think we could CLONE in one person year

- ByteLynx

- Drilbert

- **Among Us**

- **Drawful 2**

- Galcon

- *Heave Ho*

- *Heavenly Bodies*

- Islanders

- *Lethal Company -*

- MewnBase

- Muck

- Plague Inc

- Quest for Glory 1

- Renegade Ops

- Steamworld Dig

- Tinker Racers / Micromachines

- **Tricky Towers**

- Unexplored

- Untitled Goose Game

- A significant vertical slice of Vampire Survivors

- **Worbital**

- Shenzhen IO

- Overcooked

- Papers Please

- Railbound / Train Valley

- House of the Dead

- **Rampart**

- Minit

- Lovely Planet

- Ricochet

&nbsp;

- Infinifactory

- Phaoroh

# 04.05.24

Actual pitchables

FPS Walking simulator exploration

Wizard combat game

Walking Simulator

System driven

First person coop together we did ENVIRONMENTS

- Generic northern europe (ICARUS)

- Demonic invasion germany post war (Vermintide)

- Post apoc desert clean sci-fi city (Roboquest)

- Zombie parkour Dubai/Istanbul (Dying Light 1+2)

- Desert River/Forgotten undead city/Volcano (Conan)

- Sci-fi demon infested mars (Doom 2016)

- Cute stylized quiet village (Goose Game)

- Woodland scandinavian towns (Generation Zero)

- Abandoned moon base / spaceship (Alien swarm / Lethal company)

- Volcanic Island of Giant mushrooms (Morrowind)

Didnt do together ENVIRONMENTS

- Usually empty (Shadow of Colossus)

- Underground industrial city (Necromunda / Metro / Portal)

- Underwater alien reef (Subnautica)

- Level is alive Factory or Biotech (Half life)

Movement modes

- Skiing (Tribes)

- Fast movement (most walking simulators are slow)

- Charge jump (Roboquest)

- Grappling hook (Doom)

- Climb anywhere (BotW)

- Parkour (Mirrors Edge)

- Blink (Roboquest)

- Jetpack

- Gliding (Spyro)

- Flying mounts (Palworld)

Moments and Feelings

- Escape into the overworld (Oblivion)

- 

Workflow test game idea

Interior

- Idea 1

- Dungeon explore

- Maintenance ship tech. Juggle keeping the crew alive in their stasis pods while you keep the skip running. Overcooked First Person multiplayer on a ship.

  - Reenter your pod after each calamity, then time goes 100+ years forward

  - Sacrifice some crew each calamity, but how many

  - 2 million respawns…

  - Space existential horror

  - Roguelike but the world does not reset

  - Immediate goal + spend excess time optimising for future runs

Exterior

- Idea 1

# 09.03.24

Galcon game but slower and with infrastructure building

MANY MANY ENTITIES

# 18.02.24

Constraints

- 2p coop split screen but support single player.

- Could work for a “1 month game”

Things we want to try in godot

- 3d with 2d pixel texture workflow

- UI in godot

# Things to make with Tom

If I make a thing with Tom, it should be:

1.  … something we would play together.

2.  … a quirky tech thing.

3.  … deliberately offline.

Other constraints

- 12 month project

- Fits team skills

- 80k budget

## Section Zero: Mini Mini Mini one month ideas

One jam for concept

Work for a month after hours

Second jam, then its a finished but not polished game

~~Hacknophobia but:~~

- ~~Real time~~

- ~~Shoot only while moving~~

- ~~Special only while stuck~~

- ~~Action game not puzzle game~~

~~Invincible for a time when stuck~~

~~Click and hold to choose a launch destination~~

~~Use parabolic arcs~~

~~Single screen per level~~

~~Item grabbing “whip”~~

~~Shooting while moving along path~~

~~Active shield while moving but then you can’t move/grab~~

~~Turrets~~

~~Moving back and forth enemies~~

~~Hearts~~

~~Recoil~~

~~Mines~~

~~Deployables~~

~~Splash damage~~

~~Phase 1:~~

~~PVP~~

~~Movement~~

~~Shoot~~

~~Level geometry~~

~~Player objects~~

~~Bullet objects~~

~~Controls (mouse + controllers)~~

## Section 1: Something we would play together

Coop

MP - Local or Online P2P

Building

Story

Multi-session playthrough

Open to community content

[*Weekly Episodic Encounters*](https://docs.google.com/document/u/0/d/11PwZ_X1FlBuhIC-RoN4izv8K-wR8aqlSPdar2KI5vD4/edit)

Asteroids cutting coop game

deterministic Pokemon game (1,2)

~~Flocking spaceship/mech game (1,2)~~

Multiplayer “playable” lobby ala Mad Adventures, then agile it from there

~~[*Kobold Subterranean Program*](https://docs.google.com/document/u/0/d/1046_y-3WE_4KNCCZEOFEJF2OT8fTdmYg6kOwwp5y97s/edit). A physics based “build something to drop down a hole” game. KSP but simpler. No atmospherics. Coop MP.~~

Coop climbing game. Go up together. Each player climbs one tower. Players throw items to one another to progress.

Coop minigame collection. Easy to downscope. Each level has variations. 1-4 players.

Infrastructure building game. Connect locations to generate resources and more building pieces. Like Train valley.

Infrastructure building game. Build the locations so they attract transports. Logistical links build up over time automatically. Train valley but you build the locations.

Escort side scrolling shooter. Buy cargo, pick a route and cargo ship to escort, then complete the mission together to arrive at your location. Race other cargo squads to get the best price.

Turn based Tactical shooter, but super basic and coop. You can't see what your ally can see. Friendly fire is a thing. Hitting a target from multiple sides on the same turn gives big combo damage.

Cog towers. Like the climbing game above but you build a machine by stacking mechanical units on top of each other. Power only goes up. Mechanical units have a sweet spot where they generate the most. Keep the plates spinning.

Elevator loading game using emerge movement. You are stationed in a level with an elevator on each side. There is limited storage space in the level itself. Elevators come and go at regular intervals and you must unload them, and reload them with the correct items. Some items need to be recharged by placing them on special tiles. Tell the story of what is happening above and below just by the objects that are coming through.

##  

## Section 2: Quirky tech things

Use fringe hardware

Physical/digital hybrid things

Idea 1: Make Cranquest anyway, Playdate

Idea 2: Multi-screen, multi-input R-Pi setup with games to suit

Tom ideas

- My little keyboard **programming is magic**

- Coop / single player focused RTS PVE

  - CPU Player Asymmetry

  - 

##  

## Section 3: Deliberately offline

Multiplayer but offline

Idea 1: Scavenger hunt kit

Idea 2: Other GPS game

Idea 3: In person trading sticker thing

Async turned based combat engine / vtt thing. Play by email or synchronous online.

# Section 4: RTS

**Prototype 1**

Spring rts mod

Custom factory with units

3 lane map

Boss unit/boss turret thingos

Enemy wave attack generation

Killing a boss unlocks a new unit type

Units have high time to kill

Player Units

- Heavy defender, slow, tough heavy hitter

- Fast interceptor, not good for front line

- Attacking unit. Limited ammo. Shields.

- Deployable ammo refueller. To be defended.

Enemy units

- Attacker

- Defense Turret

- Big Defence node

**Prototype 2**

Give players different units that counter different enemies

**Prototype 3**

Information restriction RTS / Blind mode

Camera is fixed to base or hero unit

**Prototype 4**

Open world RTS

Nomad base loop hero RTS mode

Hero unit that respawns at main base

Bases build units up to a cap

You travel between them to build up your own forces.

Coop Players want to attack together, but to refuel they need to spilt up for a while and communicate which bases they have emptied

**Prototype 5**

RTS in a ruined city. Start in the middle.

Not zombies!

Enemy spawners are everywhere but only react to trespass or attack.

Once active, a spawner will begin scouting and if it finds your base it will begin attacking.

Destroying a spawner awakens nearby spawners.

Strategic use of choke points and strategic expansion strategy is key.

Player Base levels are unlocked based on how many enemy bases are adjacent.

**Prototype 6**

Controller friendly RTS

Left stick just moves your hero unit.

Nearby linked units follow your hero.

While in a base, you can press X while next to a unit to link/unlink it.

In combat you can target enemies with the right stick and press a button to change their priority up or down. This changes which enemies your units target.

Spawn Version

Steam API

Joint app save location

Small rts with the UX of a big rts
