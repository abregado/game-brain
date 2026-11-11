---
title: "Progen and Tilemaps"
source: "Game Stuff/Game Ideas/Progen and Tilemaps"
modified: 2012-11-06
type: design-doc
area: design-theory
status: "idea"
projects: []
concepts: ["Design: Turtle Procgen Maps"]
words: 158
summary: "Algorithm notes for procedural tile map generation using spawning turtles with inherited decaying parameters, boundary exits, pruning, and nested 2D arrays of chunks with tunnelers."
tags: ["area/design-theory", "type/design-doc"]
---

Procgen map

Create 2d array

button to draw it to screen(bitmapdata, one tile is one pixel)

int for states, start with 0 and 1

turtle class

higher change to turn

low chance to go forward

high chance to spawn new turtle

low chance to die

each new generation inherits chance from parent

each new generation gets less chance to turn and higher to go forward

also lower to spawn new turtle

higher chance to die

turtles that collide with boundary are killed

at these points, exits are created if neighbour is a valid location, otherwise create caps to seal ends.

tiles next to 2 other tiles are removed 50% of the time

tiles next to only 1 other tile are removed

tiles next to no other tiles are removed

Create 2d array of 2d arrays.

run generation as in first case

place known entrances from neighbours exits

Place tunnelers that will path/dig from exits to nearest empty space.
