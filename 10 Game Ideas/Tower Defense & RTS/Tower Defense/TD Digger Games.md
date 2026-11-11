---
title: "TD Digger Games"
source: "Game Stuff/Game Ideas/TD Digger Games"
modified: 2014-09-13
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Tower Defense]]"]
concepts: ["Tower Defense", "Digger TD", "Design: Tunnel Pathfinding"]
words: 503
summary: "Design notes for a tower-defence digging game: dig tunnels through a rock grid, pathfinding, collapse/maintenance, reinforcement, resource pipes, command pod dropped from orbit."
tags: ["area/game-idea", "project/tower-defense", "type/design-doc"]
---

- to tunnel, the player needs to dig in stages

- tunnelling the same tile allows faster movement

- congestion is calculated daily or on tile dig

- pathfinding calculated after each tile is dug

- djikstra field pathing

- rooms are multi-tile but must be dug out many times to be useful

- aim is to bring raw material to the mine exit

- item size is limited by tunnel height

- tunnels also need maintenance, and to be checked

- most of play is about tunel maintenance and rubble management

- some tiles not good for tunnels, some not good for rooms

- tunnel collapse part of the mechanics

- deliberate and accidental collapse

- monster holes in map require creative collapse

- 

grid based map

grid is filled with rock tiles

the player places important structures in the grid

tiles between these structures are dug out, using imperfect pathfinding

enemies attack from the top of the screen

if there are no paths to the structures special digging entities attack to make paths

Resource tiles added to level at generation, dig them to take resources. These are also used to move to player suboptimally , to avoid cookie cutting

Reinforcing walls to make the AI take longer to dig through, or so they route differently. Use a more tower defence style mechanic.

Resources are carried back to the centre. Defend the supply chain from enemies.

build and fight rounds OR CONTINUOUS?

Each tile dug gives fixed “Raw” resource

Each map the player has a fixed amount of “Tech” resource to build turrets and facilities. These could be monster glands that can be grown.

Sideview? Your command pod is dropped from orbit and digs deep into the ground

Enemies attack from the surface.

As enemies destroy your facilities and breach your walls you must build deeper and deeper

Time limit to build new structures bewettn each wave of enemies? Keep the pressure on. Simply the player depletes the resources and must dig deeper.

Score resources are collected periodically and then some time afterwards you receive more tech points.

Two resources, one is gained immediatly from digging, the other from collecting and storing special resources.

Rig abandoned areas to explode and use them for mining or for defense. As a structure.

dig under your command pod to drop it deeper into the earth or perhaps it digs itself at a fixed rate.

Player can only dig a limited amount of tiles at one time.

Digging interaction mechanic - drag sqaures over the area you want to dig. Only so many squares can be dug per wave

Reinforcing interaction mcahnic - drag lines over walls you want to reinforce. Only one can be reinforced per square dug

Players need to dig as many tiles as possible to get the most reinforcing resources.

Trade off between corridors and digging resource tiles

Closer resources are more accessable.

Display pipes between resource tiles and the command pod

Enemies that reach a pipe will syphon % of resources
