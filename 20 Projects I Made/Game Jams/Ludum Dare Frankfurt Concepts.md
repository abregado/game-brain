---
title: "Ludum Dare Frankfurt Concepts"
source: "Game Stuff/Ludum Dare Frankfurt Concepts"
modified: 2017-04-11
type: brainstorm
area: jam
status: "idea"
projects: ["[[Game Jams]]", "[[Shooters & FPS]]"]
concepts: ["Ludum Dare", "Pacman Growing Maze Runner", "Massive Enemy", "Binary States Maze", "Growing Shooter", "Starfox Clone"]
words: 783
summary: "Shared planning doc for a Frankfurt Ludum Dare 34 team: theme brainstorms (Growing, Two Button Control), team member skills, and high-level game concepts like a growing Pacman, a shared massive enemy and a binary-states maze."
tags: ["area/jam", "project/game-jams", "project/shooters-fps", "type/brainstorm"]
---

[*https://docs.google.com/document/d/1IABBoPCsqA7rTICM78ooaRmqKdaNwxJkj41fB5n6y3k/edit?usp=sharing*](https://docs.google.com/document/d/1IABBoPCsqA7rTICM78ooaRmqKdaNwxJkj41fB5n6y3k/edit?usp=sharing)

Inception style link to itself, send to others who want to be involved.

First Section is for themes

Second Section is about us

Third section will be about actual complete ideas as high level concepts

You can comment on anything using the Google comment system, we will have a voice chat in Skype soon to start discussing.

# 

#  

# Themes:

## Growing Ideas

- Plants

- Size change +/-

- Drugs

- Farming

- Osmos/Pacman size change (see [*HLC Section 3*](#high-level-concepts))

- Katamari - collecting things

- Enemies grow as they take damage, becoming slow and easier to avoid, but harder hitting.

- Powerups grow slowly on the level. Wait longer to make the powerups better

- Health packs grow on players backs

- Stockmarket, growing

- Groot (Plant character)

## Two Button Control

- Only two buttons

- Two activatable objects in the level/game

- Two buttons on a shirt control the king/lord/dude of power

- James Bond suit, has two buttons with different abilities

- Mouse shooter, but you can only move back and forth along a line (left and right arrow)

- Jump and Run

- wheel, hold and release to activate abilities

- Flipper

- Pinball (yuk)

- Moral Choice games

- Binary states!

- Program the avatar with 1’s and 0’s and then press play

- Example for a simple two-button game (Klabutong): [*https://www.youtube.com/watch?v=JM-0WrRCXVc*](https://www.youtube.com/watch?v=JM-0WrRCXVc)

- QWOP: buttons to walk or performs an action (complete complex task)

- Quicktime event construction

- Two button-like characters that you control

- combinations of opposites (buy/sell, red/green)

- mouse + left/right

- Starfox flying mechanics

- two virtual rotating buttons (like on a stove) with 6 states each

## Combined Ideas

- you gain more buttons to press as you progress

- buy/sell buttons, prices are growing or shrinking

- Racing game: being in first place makes you bigger so limiting your paths on the map

# Involved Parties

What you want to do, who you are, skills etcetera.

Ben (Abregado): Mechanic Design, 2d Non-Unity stuff, Lua code, Love2d as Framework. Happy to work alone or as sole programmer on a project.

[*http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=20783*](http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=20783)

Fabio: programming low poly pixel art, has own engine which is preferred

Alden: 2d/3d art, textures, ui design, digital art

Alex (Gladers) Programming (backend/frontend), AI, 3d, 2d networking

[*http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=40397*](http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=40397)

Evegeny: programming 2d procedural

Anton: graphics environment procedural network code

Richard (CWolf): programming unity help only engine asset

Herbert (Kriesh) 3d lowpoly art, Unity

Alden: 2d/3d art, textures, ui design, digital art

Marcus(The Arrival): unity programming music sound raw sounds

[*http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=47053*](http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=47053)

Lucas: unity level design player direction

[*http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=64444*](http://ludumdare.com/compo/ludum-dare-34/?action=preview&uid=64444)

Peter: consultant native unity frontend backend netcode engine. No time to participate but might be able to answer some implementation questions

# High Level Concepts

Pacman Growing Maze Runner

- eating food pellets makes you larger

- when big you can shoot

- when small you can jump over walls

- passages are different sizes

- handmade map

- walking, shooting and jumping makes you smaller

- balance between being big enough to eat enemies, but small enough to navigate

- FLAW: Passage that gets wider is single direction

Massive Enemy

- simple shooter

- when a player kills an enemy, the server is told and the massive enemy is reduced

- all players are effecting the same enemy

- when enough damage has been done by all players the boss changes to a different attack pattern.

- The massive enemy grows when a player dies

- only send the kill count when a player dies.

- Send a timestamp so we can determine a maximum rate of change

- Massive Enemy damage calculated server side, and modified based on how often deaths are sent from the same IP, to limit griefing.

- 

Binary States Maze

- Player can see a maze with an exit and an avatar

- limited time to input a “code” to move the player through the maze

- code is made of only left or right

- player has simple rules as to how they move, if one choice, take it, if two then left/right selects, if three options then the middle option is not available

- loads of places to die

Growing Shooter

- Health is decreasing as you shoot enemies

- Shooting them also inflates them

- fat enemies are slow or stationary but shoot slowly and with a lot of damage

- damage enemies slowly over time to kill them

- killing enemies too fast makes them level up or split

- powerup growing idea?

Starfox Clone

- Fly with mouse, Shoot and Barrel Roll

- Good team project, everyone can work separately

- Polish flight mechanics, shooting and graphics separately

-
