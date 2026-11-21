---
title: "Sumo Snowman Maker 9000 LD31"
source: "Game Stuff/Game Ideas/Sumo Snowman Maker 9000 LD31_"
modified: 2014-12-08
type: design-doc
area: jam
status: "prototyped"
projects: ["[[Game Jams]]"]
concepts: ["Sumo Snowman Maker 9000", "Ludum Dare"]
words: 191
summary: "Design/TODO notes for a Ludum Dare 31 game: roll a snowball by choosing wind direction, collect snowman parts in stages, roll off a cliff to the goal."
tags: ["area/jam", "project/game-jams", "type/design-doc"]
---

TODO

- snowball rolling

- items going under obstacles

- menu screen

- tutorial

snowman parts

- legs

  - button

- body

  - scarf

  - button

  - arm x2

- head

  - eyes x2

  - hat

  - nose

circular level bounds

box2d physics

only one moving object the player

player ball suffers from drag

all other objects are static

player is a ball with variable radius

control by selecting the wind direction

clicking on the screen makes the wind come from that direction uniformly

a smaller snowball will accelerate faster

Snow Collection

The whole level is covered by a grid

As you roll over grid tiles they are emptied of “rolable snow” and cannot be used again

Obstacles

tree (unsmashable)

stone (large snowballs ignore them)

house (unsmashable)

Collectables

carrot (nose)

coal (buttons and eyes)

sticks (arms)

scarf (neck)

hat (head)

Aim of the Game

Collect the correct parts for your snowman in three stages. Grow your snowball to the correct size then roll it off the cliff into the goal zone. Do this three times to see your snowman.

Classes

Level

> Snowgrid

Player

Collectable

States

Menu

Game

Scoring (Snowman display)
