---
title: "BS - Coldsleep Crew"
source: "Game Stuff/Game Ideas/BS_ Coldsleep Crew"
modified: 2024-05-19
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Space Station 13-14|Space Station 13/14]]", "[[Dwarf Fortress mods]]"]
concepts: ["Coldsleep Crew", "Wiring Minigame / Pipe Nodes", "Succession Saves"]
words: 557
summary: "Design notes for Coldsleep Crew, a first-person co-op 'Overcooked on a ship' maintenance game with cryosleeping crew, patch panel wiring minigame, succession save-sharing, and a prototype task split between Tom and Ben."
tags: ["area/game-idea", "project/dwarf-fortress-mods", "project/space-station-13/14", "type/design-doc"]
---

From here  
[*https://docs.google.com/document/d/1Ort81Lb0zpG3sXf2xogDJ37Z1x0lJ4TsB7QxPZbta5E/edit?usp=sharing*](https://docs.google.com/document/d/1Ort81Lb0zpG3sXf2xogDJ37Z1x0lJ4TsB7QxPZbta5E/edit?usp=sharing)

# Intro notes

Maintenance ship tech. Juggle keeping the crew alive in their stasis pods while you keep the skip running. Overcooked First Person multiplayer on a ship.

- Reenter your pod after each calamity, then time goes 100+ years forward

- Sacrifice some crew each calamity, but how many

- 2 million respawns…

- Space existential horror

- Roguelike but the world does not reset

- Immediate goal + spend excess time optimising for future runs

# Player story and actions

Change state of interactables

Move interactables between fixed places

# Loops

Locate, Diagnose, Repair

Complete chapter, get new area, loot area, do the main loop

# Feedback mechanisms

A ticking counter of how many people are still in cryosleep

- Goes down by 1 every time you die

- Goes down more if you fuck up

Room states

Room states that spread through doors or vents

A “light years travelled” number that goes up over time

# Machines and Interactables

Terminals with replaceable chips

Conduits connecting rooms

Each room has a patch panel

- Everything is unlabelled to begin with

Rooms are linked by a conduit with

# Succession games.

When you finish playing, your save game with its unique id gets uploaded.

There is a chance that someone plays a shift on your save before you get back.

Option when you start a new game to allow this.

How to deal with trolls?

Gitblame on your save game

Each Collaborator gets a status tube in the starting room

You can eject them to ban them

# Wiring Minigame Prototype

Each screen has:

- a patch panel

- a set of “machines” that have inputs and outputs

- A number of connections to other rooms (conduits)

- A number of buttons to go to other rooms (not necessary the same rooms as the conduits)

The ability to use the buttons to go to other rooms can be disabled via wiring changes.

Machines have hardwired connections between each other that affect their state.

# Overcooked FPS

Network multiplayer, 2+player, fps, “wack a mole” styles chaos gameplay.

Prototype 1

Tom - Network Controller and Node Class

- On update, kill all pipes, rebuild pipes

- Add node

- Delete node

- Make connection

- Remove connection

Ben -

- UX (pipe connections)

- Read state monobehavior

- Pull in Indicators

- NodeBody

  - Ref 1 node

- ConnectionBody

  - Ref 2 nodes

MachineRules

All inputs == all outputs

Day 2 WOT DA WI NEED

Rebuild all pipes on change

Pipe direction shown

Pipe item shown (sprite)

Item types as Struct

Multi camera setup with arrows to swap between them (Cinemachine)

Input/Output Connector shows sprite of item

Demo scene

**Phase 3 What would we do?**

Connector direction (in/output) needs to be visible

Raycast between connectors to see if the connection is allowed

3d FPS

Machine slots that fixed in the level

Machines can be set to be movable or not.

Player can pick up one machine at a time

Silhouette Mesh for each machine

Text showing name and recipe on a part of the machine.

Highlight connector when you hover it

Placement Preview for wire and machines

Machine locations have a bool if they are powered (so we can make machine storage lockers)

Tell the player when you

Feedback for when a pipe is incorrect
