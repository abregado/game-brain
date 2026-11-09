---
title: "Minecraft 1.8 Gamemode Brainstorm"
source: "Game Stuff/Game Ideas/Minecraft 1.8 Gamemode Brainstorm"
modified: 2015-06-24
type: brainstorm
area: game-idea
status: "prototyped"
projects: ["[[Minecraft & Voxel Building]]", "[[Dungeon Crawlers]]"]
concepts: ["Minecraft ideas", "Radzone PvP", "SkyDungeon Generator", "Minecraft Maze Generator"]
words: 396
summary: "Ideas for Minecraft 1.8 gamemodes built with ComputerCraft Command Computers: Radzone PvP, SkyDungeon generator, and a self-constructing chunk maze (noted as actually prototyped)."
tags: ["area/game-idea", "project/dungeon-crawlers", "project/minecraft-voxel-building", "type/brainstorm"]
---

# Ideas to utilize ComputerCraft Command Computers

# 

# Radzone PvP

The entire Overworld is radiated. Players accrue Radiation sickness points while in the wilderness. As these points build up, players are afflicted with various debuffs. Eventually players die from these.

The strength of the Radiation is based on the distance to the nearest ‘safe zone’. These are x,y,z coords stored in a CC Command Computer.

The application of radiation points is done using CC Command Computers.

Biomes are supplied by Biomes o’ Plenty. Only the Wasteland biomes are used.

Acid Rain mod is used to damage players when it rains.

# SkyDungeon Generator

Using CC Command Computers, create a randomly generated dungeon world.

Set up a flatworld with nothing in it.

Place a Command Computer and run the program

The program checks the location of each player, and if the surrounding chunks have not been spawned, then generate that area.

Closed in areas, as well as gantries can be generated.

Since entire world gets generated, supply of resources can be controlled.

Area around the computer gets protected and a safe zone is spawned immediately when the program is run.

Each area can be refreshed when visited if it has not been refreshed for a long time. Keeps resources coming in.

Needs a Trading mod and could work well with Archemedies Ships if the dungeon is floating in sky

Maze Generator - Actually prototyped

Similar to above but instead of generating dungeons it generates a maze. Players are in Adventure Mode and must explore a huge ungenerated maze by forcing the maze to construct itself. The Generator is controlled by a CC Command Computer.

Each cell in the maze is one chunk.

Cells are 16x16 flat platforms floating in a empty superflat world.

The floors of the cells are built using colored clay

Red clay means that the cell has not been explored yet

Green means the cell has been explored

Blue means that 3 players must be present to explore the cell

Yellow means that 10 players must be present to explore the cell

Purple is the winning cell, and all players must move there to reset the game

The size of the maze can be given as a function

Every time the maze is completed, the size goes up.

Needs a chunk loader as the center chunk will end up far from the exit
