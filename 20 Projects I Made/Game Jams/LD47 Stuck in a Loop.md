---
title: "LD47 Stuck in a Loop"
source: "Game Stuff/LD47 Stuck in a Loop"
modified: 2020-10-05
type: design-doc
area: jam
status: "prototyped"
projects: ["[[Game Jams]]", "[[Shooters & FPS]]"]
concepts: ["Ludum Dare", "Agent Robot Loop Game", "Marble Run", "Rope Untangling Game", "Rail Shooter Loop"]
words: 444
summary: "Ludum Dare 47 (Stuck in a Loop) notes: last-day todo, Agent Game design where robots record movement commands, many alternate loop ideas and theme word association."
tags: ["area/jam", "project/game-jams", "project/shooters-fps", "type/design-doc"]
---

**Last day TODO**

**Urgent:**

- ~~Buttons fix (there is a bug in the end, it just seems to work sometimes)~~

- ~~Get the colored eyes / matching buttons in~~

**Nice to have:**

- ~~Flavour text (final screen, victory overlay, etc)~~

- SFX (die, pick up orb, deliver orb, spawn)

Agent Game

- Tile based

- Discrete movements (up down left right)

- Send robots to collect “fruit” and bring it back to the start

**Systems**

Each robot records its movement as up, down, left, right commands

Non-destructive, deterministic gamestate that can move in each direction.

- Resimulate from start on undo?

Collision detection when moving a tile

**Assets**

Robot (no directionality needed)

Start tile

5 types of “fruit”

Wall tile (can be “pushed” against to add wait steps)

Pit Tile

- no input accepted, cant enter  
  > Or

- Disables robot and simulation if stepped on

**Buttons**

Arrow keys (movement)

Select Robot keys (bumpers/mouse)

Undo button (sets the simulation back one step)

Play simulation (stop simulation button while simulation running)

**Ben Todos:**

- Max program length

- Robots have a spawn location

Agent Game 2

- Continuous Movement

- Each agent type has different movement and a starting point

Marble Run

Player Auto Game

Portal game

- Plan B

&nbsp;

- Rope untangling game

- Shared input characters

- Dying over and over loop

- Escape room with looping machine

- Death gauntlet deactivation

- Sacrifice parts of your body to escape

- Everything moves in a loop and you have to introduce other objects with no crashing

- Add more agents to a system, new agents become the obstacles in the next round.

- Player moves automatically in a predictable way, but you have an interaction which makes them bump into obstacles, changing their overall path.

- Rail shooter but in a loop

- Falling Portal mobile game

- The level loops over and over, as the player runs to the right

- Closed Resource cycle

Stuck

- Sticky

- Want to stay still

- Attached

- Glue

- Wedged between objects

- Jammed

- Traffic

- Writer’s Block

In a

- Within the bounds of the line that makes the loop

- Inside the volume of a donut

- Always moving

- Not yet stuck and want to get stuck

Loop

- Circle

- Repeating

- Holes

- Rope

- Lasso

- Lifetimes (Growing up, aging, dying)

- Dynastic Cycle

- Music

- Rollercoaster

- Earrings

- Hyperloop

- Trains

- Conveyor belts

- Cycle

- Series of transformations

- Evolution

What is in the Loop

- Enemies

- Obstacles

- Player

- Objectives

- Resources

- Player tools/abilities

- Level geometry
