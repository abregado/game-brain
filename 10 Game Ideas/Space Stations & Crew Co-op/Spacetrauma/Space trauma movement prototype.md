---
title: "Space trauma movement prototype"
source: "Game Stuff/Space trauma movement prototype"
modified: 2024-12-01
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Spacetrauma]]", "[[Kobold]]"]
concepts: ["Spacetrauma", "Kobold"]
words: 301
summary: "Prototype todo and design notes for Spacetrauma: suit resources, hit points and bleed, visibility, player in ship movement, and ship control."
tags: ["area/game-idea", "project/kobold", "project/spacetrauma", "type/design-doc"]
---

Space trauma movement prototype

Next!

- toggles for each sensor ring

- Atmospheric graphics

- Drift mode toggle with check box

- Oxygen in suits

- Prograde marker should be on top

- Grabbing objects

## Visuals

3d models, plain texture

Fog

Background objects protruding into playable area like in kobold

## Player Suit

Prograde marker that shows speed and danger level

### Resources V2

4f hit points

Collision at speed costs 1 and adds 1 bleed

Suit has 1 charge to reduce bleed over 10 seconds

1 bleed causes 1 damage over 10 seconds

Taking no damage for 30 seconds will start Regen of any decimal loss.

Oxygen lasts a long time

Oxygen usage is based on remaining hit point percentage

Thruster fuel is very limited.

Boost costs more fuel when you first press it.

For a new player, thruster fuel will be the limiting factor in an away mission.

Each hit point lost causes a status effect that makes everything harder. These last until the next station.

- View restricted

- Thruster force reduction

- Fuel or oxygen use modifier

- Screen effect

- Interaction range reduction

- Interaction speed reduction

## Player visibility 

Circle cutout.

Right click to zoom out and restrict view to an arc.

Same sensor ring as the ship, but only limited options and resolution.

Sensor ring only in direction looked

## Player in Ship movement

Reparent to ship

Parented rigid body? How does it move.

Fixed movement

How collision with walls?

Rotate camera to keep ship upright

## Player ship

Ship does not rotate?

Button to eject player

If player collides with ship entrance zone then they get in

Set a direction

Set a speed

Ship will try to match (use a PID?)

Reactor builds up heat while ship is changing direction or speed
