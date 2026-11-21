---
title: "Game of Life Game"
source: "Game Stuff/Game Ideas/Game of Life Game"
modified: 2013-09-14
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Playdate & Small Games]]"]
concepts: ["Game of Life Puzzle"]
words: 144
summary: "Implementation notes for a puzzle game built on Conway's Game of Life with resources, goals, levels, pause/retry and GUI list."
tags: ["area/game-idea", "project/playdate-small-games", "type/design-doc"]
---

Life Sim game

Simulation

Calculates next state of board - runs every X frames

keeps track of dead cells that will become live

counts for current and next state

alive cells

new alive cells

different cells

Updates old state to new state - runs every X frames IF unpaused

modifies resource table when a cell will come alive

adds resources to wallet

check for victory conditions

check for failure (no success and not enough resources for 3 new cells)

check for pause if there are no live/dynamic cells

if pause, save live cell table for retries

controls

Spacebar - unpauses if the next state contains any live cells

quit

left mouse click to place

right mouse to remove

simulation speed scaling

gui

Start Game - level select

Goal popup and confirmation

hud goal progress bars

resource counter

victory/next level popup

failure/retry from save popup
