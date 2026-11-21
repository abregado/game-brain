---
title: "LD28 Brainstorming"
source: "Game Stuff/Game Ideas/LD28 Brainstorming"
modified: 2013-12-16
type: planning
area: jam
status: "designed"
projects: ["[[Game Jams]]", "[[RTS Ideas]]"]
concepts: ["Ludum Dare", "One-Command-Unit Grid RTS"]
words: 726
summary: "Ludum Dare 28 (You only get One) brainstorm that develops into a design/task breakdown for a one-dimension line-wars grid RTS with seeds and level jumping."
tags: ["area/jam", "project/game-jams", "project/rts-ideas", "type/planning"]
---

Theme: You only get One

Asbstract level design based on each of the 4 words

you only get one meaning

One is a person

your name is Only

try to catch just ONE item

Physical objects: You only get one of a thing

Only one life EVER

Only one opportunity try

You only get one of a selection of things

There is only one objective

You only get one each

You only get one at a time

You only get one ever

You only get one

one game mechanic that changes

victory condition that changes at set intervals

you one get one seed - nobody has the same experience

you only get one tool - dig or fight or fix or whatever

One hit point games

One bullet per gun

Only one per minute

Only one second to act per minute

only one powerup per kill

jump once per kill

dinosaur comics level gen

one new one per victory

RTS one dimention line wars

one command unit

move next to resources to collect

spawn units which are automated

these units fight against AI unts like tower defence

you only get one resource at a time

behaviors

follow your base

move toward enemies

move toward enemy spawn/resource points/

move toward enemy objectives

one screen map

base moves slower than units

enemies spawn in waves

\\ or

“dumb” enemy base units

move to next level at any time, taking your resources with you

cost for finishing the level

limited resources on each map?

fail condition is not being able to progress

balance comes from challenging the player at cost that is a little less than the resources you give them

player wants to complete a level with minimum expendature

spend too much and die of starvation later

spend too little and you will be overwhelmed

maps have limited resources

SHOOTER - one bullet in total

ACTION - side scroller shooter space agame but you must defend a cruise missile or bomber

active defence tool to deflect enemy shots

ADVENTURE you only get one crusade, the last one, no snakes i hate them

TD: one enemy at a time, one tower defense, one wave

PUZZLE: must aleays be carrying one tile, get to a point to victroy

STRAT: only one action out of many

Things we are good at

Tile based

Box2d - out unless completely basic interactions

Things we want to do

Phased Based real time

Side scrolling Platforming - out

title/landing page

seed entry

play now

grid map - single screen

static placement of objects and units

objects array - object management

phasing system - shoot/cleanup/move

player object

keyboard commands for movement

unit object

x,y

grid ref

team variable

speed

range

hitpoints

behavior type

map array

every filled tile gets an object

terraintype = 0,1

movement behaviors

turret - move toward scrap point and then turn into turret

search and destroy - move toward enmy units and attack at close range

seiger - move toward point and hang around it (attack or defense) longer range  
movement sliding animations

obstacles - proc gen

pathfinding dijkstra fields

shooting behavior 1 - closest target

damage system

shooting “animations”

clean up phase

remove destrouyed units and other crap

explode “animation”

MILESTONE 1

unit spawning point (perhaps that moves)

distribute targets/behaviors automatically

resource object

interaction with player when on same tile

> variables anf functions for limited resources
>
> location variables
>
> type variaables

resource storage for player units

deployment system

UI for that (select with number keys)

‘d’ for deploy keyboard command

placement not on top of other units

player unit takes damage

targetting rules for enemy units

victory condition

just go to next level at any point

cost a substatial amount of res to jump level

level change - reroll

deterministic proc gen

levels get “harder”

less resources

more enemies at level start

more enemies for wave

players can post their level and seed on the comments

death condition

you died

retry with same seed

retry with new random seed

display current seed and level

art

colored squares and a tilemap

BLOATY MCBLOATERSON

enemy BASES

behaviors as per steves imagination

Do Later List

cleanup on level geenration so there is no terrain off the map grid

instructions

graphics

color pallette

terrain rounding off

fix the goddam sound eating memory like a glutton

tooltip

instructions

acknoledgements on ending page
