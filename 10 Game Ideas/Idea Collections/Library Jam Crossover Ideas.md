---
title: "Library Jam Crossover Ideas"
source: "Game Stuff/Game Ideas/Library Jam Crossover Ideas"
modified: 2014-11-10
type: brainstorm
area: game-idea
status: "idea"
projects: ["[[Xenosurge]]", "[[Playdate & Small Games]]", "[[EVE-like Player Economy]]"]
concepts: ["Seasonal Plant Harvesting", "Xenosurge", "Corpse Piler", "Reverse Asteroids", "Roguefight", "Minigolf Game", "Tilegrid Builder", "Wormlizard", "Sub Sub Submarine", "Haunted Cleaning Game", "EVE-like player economy", "Design: Love2D Reusable Libraries"]
words: 826
summary: "List of small game concepts for a library/game jam (plant harvest, Xenosurge remake, Corpse Piler, Reverse Asteroids, sub-sub-submarine, Halloween haunted cleaning), tagged with reusable library components."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/playdate-small-games", "project/xenosurge", "type/brainstorm"]
---

### Plants/harvest profession - from Perpetuum ideas, to proto

plants have seasons, this could create boom and bust cycles

Spread in Autumn, hibernate in winter, grow in spring, fruit in summer.

each plant has its own seasonal periods, but they are always in that order.

during the harvest season they would fruit/bloom and can be harvested.

Plants could spread more when players leave some fruit on them

cultivation means defending the area from scavengers, and being picky about which plants to pick/cutdown

Plants die after several cycles so it is important not to over harvest

New plants don't fruit for the first x seasons.

Fruit dies in Autumn and converts to new plants.

Each plant is available at different times so harvesters always have something to do

Searching for and recording plots during the off season becomes a important task

plants cannot be planted by players.

protoplants on grid

player has 8 direction movement

player can click on plants to pick(left) or fell(right)

cargo fills up and player returns to a drop point

resources are slowly converted to points in a number of categories

player must keep all categories full constantly to get 'score'

consumption rates change ove

Minigolf Game. **Box2d Physics entity controller**

Simple minigolf game with a twist. Lord knows what the twist needs to be.

Xenosurge Remake: as current xenosurge. Android game. Tap to launch missiles. Missiles come from fixed towers. surround to capture, not build in existing walls. In repair mode, drag shapes to field. At end of time limit all walls are placed and flood fill performed. 5 shapes at bottom of screen, replaced shortly after used, but not instantly. Different structures to capture, increasing build/combat timer, reload speed. Different turrets fire different missiles.

Tilegrid builder. Click on an upgrade and then wait. When countdown finishes, chose immediately from three random addons. Simple survival mechanics such as Resource balancing and budgeting. Addons cost resources to plan, and each option costs a different amount. Long build times, players must think several minutes ahead. Some resources come in random pulses, others as smooth trickles.

Corpse Piler **line of sight and simple “food clock”**

Survival Shooter with a heat mechanic and line of sight. The player is a survivor of a religious apocalypse, holed up in a well stocked bunker. The only thing missing is fuel for the fire. As long as the player continues to collect and return with firewood, or other burnables, he will survive the nights. Ghouls wander the area, and when killed, their corpes can be shifted around. Eventually they will reanimate. The player can burn the corpses but this uses precious resources. Also, there is a viewcone based on mouse direction.

Roguefight. **dijkstra field ai, grid movement controller**

enemies take multiple turns to attack, hitting them interrupts their attack. The hero has a number of attack choices. Difficulty comes from increasing enemy numbers. Knockback is part of combat

Reverse Asteroids - **inventory manager, box2d entity controller**

player is a spaceship. Scrolling infinite world. different scan modes show different pips on screen edge for navigation. Box2d physics. camera tracks player. Clik/tap to boost in a direction. Button to negate momentum. main obstacle is junk. All junk gives pickups when shot, but pickups must be attached to your ship immediately. No inventory for modules. Each item is like a diablo item, and inventory is like diablo inventory. Ites in a radius can be collected and equipped. Dropped items float in space immediately. Random enemy craft cross your space but are not hostile, but will retaliate. two layers of modules, one adds system slots, the other are the systems. Ship hulls have fixed amounts of module slots. Better items come from better junk and ship wreckage. Items in range get stabilized when inventory is open. Adding to hull gives massive penalties. Create power cycle/wave as players must give up power to increase their power ceiling. Permadeath.

crabs

pit

wormlizard. **-simple ai interactions, procgen world**

moves slower and slower over time, except while near warmth. Also needs food which is not abundant. Some creatures have babies and the player chooses to leave them alone as investment.

jelly fish mask - **box2d entity controller**

sub sub submarine junk collection game

drive a sub deep through a maze of obstacles

when you reach a fixed depth, a smaller sub pops out

repeat this several times

when you collect an item, the subs fly straight back to each other

there is a break between each connection

false teeth

Seasonal games. halloween, easter, christmas

Halloween game. **two frame animation, touch controller**

Haunted Cleaning game

room with objects and flashing scary light

press on items that don't belong in that room

room of items, light stays on a few seconds

light goes out, then when it returns there is one new item

player must pick the new item

ghost come move items around, try to steal. tap to stop them if the item is needed.

Apple collection game
