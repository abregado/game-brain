---
title: "Spacetrauma Design Doc"
source: "Game Stuff/Spacetrauma Design Doc"
modified: 2024-11-28
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Spacetrauma]]"]
concepts: ["Spacetrauma", "Design: Ship Building", "Design: Limited Visibility"]
words: 930
summary: "Design doc for Spacetrauma as a Barotrauma-inspired 3D space game: inspirations, customer expectations, changes from Barotrauma, and experiments P1-P6."
tags: ["area/game-idea", "project/spacetrauma", "type/design-doc"]
---

# Design

## Other Inspirational games

Heavenly Bodies

Lovers in a Dangerous Spacetime

Outer Wilds

## Games with zero-g movement

Hardspace Shipbreaker

Breathedge

Heavenly Bodies

Space Engineers

Kerbal Space Program

Prey (2017)

Outer Wilds

Boundary

## Games to try for research

Clouds Ahoy

Void Crew ← meh. I hated the “you lose everything on a customizable ship after a mission”.

We need to go Deeper

## What do our customers expect in the game?

Round based missions ← somehow feels like a better experience than a continuous world

Being inside a spaceship

Being outside a spaceship

The spaceship is customizable

Keep the outside out and the inside in

Periods of calm when docked

SS13 players expect a chaos simulator

Among Us players expect social deduction (Traitor) gameplay

Space players expect floaty space movement with momentum ← Dunno. Not many people actually like this. Momentum-based controls are always hard by default.

Vehicle sim players expect it to be “not straightforward” to fly the ship

Horror game players expect to be scared

## Barotrauma conflicts

I don't want to go outside but I must go outside

I want to go fast but I also want to go carefully

I want to see where I'm going but I don't want to be detected

## Things that work well in Barotrauma

Limited view range ← An “no” outside view range for everyone except the captain.

Longer than sight radar range (Something is there but what?)

## Things that we want to add on top of Barotrauma

In-game ship editor when at certain bases.

Crew and ship upgrades are communal, anyone can buy them for any character

The players invest in their ship over a long time

3D?

Multiple sensors? Radar (active, can be picked up by enemies), ELINT, IR Detector, Magnetic Detector, Geiger Counter for different kinds of threads or assets.

More interesting gameplay during missions for engineers / mechanics instead of “repair this” and “maintain that”.

Basic systems are always online in some basic capacity

Basic Maintenance tasks add buffs, instead of just shutting down systems if not completed.

Maintenance tasks are more complex, multistep processes

Special modes or machine activations only stay online/available for a limited time after “maintained”. So their default state is non-functional.

Inventory management is only done inside bases.

At the start of the round, all items are returned to their allocated starting positions.

At the end of the round, items on players and in the ship are tallied. If something ot lost then it is removed from the ship.

Nothing stays in a character's inventory between rounds.

## Things we want to change from Barotrauma

Crafting in a station is easy, simple and instant.

Crafting when underway is hard, complex and slow.

Semi complete information about the next area so you can plan… a bit.

Base levels are not walkable and never have combat instead they are just UI based game state (Ben wants)

Neutonian movement, with a Stabiliser button, when outside the ship. ← Stabiliser could be on by default. Movement can actually feel the same as in Baro, since it worked pretty well. No heavenly bodies experience here, since nobody “liked” it, it was a challenge and does not work at all when under pressure.

Precise, sticky movement when inside the ship.

## Things we want to remove from Barotrauma

Inventory management hell

Physics based character movement

Traitor mode, it should be PVE only ← depends on how well the traitor mode is made, especially the missions. “Kill the crew” is no fun for anyone and easy to do. “Get Keycard from X” is way more challenging and none-harmfull to others.

# Experimentations

## P1: Ship and Player Movement

Movable ship + Movable Character

Should ship and player movement be the same?

How do characters transition between inside and outside the ship?

## P2: Prototype multi layer map and movement

Overview map scene with nodes

Mission scene with side view. Very simple movement (WASD)

Exits based on Overview map

Some nodes trigger a Base scene.

Between each maze there is a different kind of scene (becomes docking scene eventually) ← Docking only if it is super crisp, like in Highfleet.

Select a new node from the Base Scene.

Repeat.

## P3: Visibility prototype 2D

Simple 2D side view movement.

How far can the player move the camera from the character?

How does the radar look and function?

How tight can corridors be?

Do we need LoS blackouts (blurring/blocking behind objects) like in Project Zomboid

What is the excuse for not being able to see far in space?

## P4: Visibility prototype 3D

How to make limited visibility interesting from a first person perspective?

Limited camera angles?

Fog (ala Dark Bramble, Outer Wilds)

Sensor Ping (ala Subnautica)

Darkness

What is the excuse for not being able to see far in space?

## P5: Interaction

When interacting with something inside the ship, are the characters still affected by physics?

## P6: Ship Building

How can we make building volumes more intuitive?

Tile grid based?

Vertex/Edge based?

Free form continuous or fixed units?

What are the reasons to build bigger?

What are the reasons to build smaller?

Where is the conflict between the two?

How do we limit the number of stations/usable objects on a ship? Volume? Tetris placement? Weight?

Do we have windows?

Conflict between areas where you can move fast and areas where you can do a lot of stuff.

Using existing editors and formats for ships to begin with.

Blender + gITF + custom properties for a vertex based approach

LDtk for a tile based approach.
