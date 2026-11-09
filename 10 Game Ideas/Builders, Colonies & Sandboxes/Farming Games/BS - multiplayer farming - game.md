---
title: "BS - multiplayer farming - game"
source: "Game Stuff/Game Ideas/BS - multiplayer _farming_ game"
modified: 2014-03-19
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Farming Games]]", "[[Player Market Hoardmode]]", "[[Other Wargames]]", "[[EVE-like Player Economy]]"]
concepts: ["Multiplayer Farming Plot Game", "Design: Maintenance System", "Design: Player Market and Trade Contracts", "Design: Procedural Moon Terrain", "EVE-like player economy"]
words: 1718
summary: "Design for a persistent single-server multiplayer plot-based farming/moon colony game with rent eviction, trade contracts, maintenance system, pseudo-procedural moon terrain, resources and proof-of-concept plan."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/farming-games", "project/other-wargames", "project/player-market-hoardmode", "type/design-doc"]
---

### Dot point summary

- top view

- tile based

- persistant world

- singler server

- exclusivity

- no “pausing”

- limited “land”

- players that do not play/pay rent are evicted

- new players can only join when there are plots available

- players are emailed when a plot becomes available and have one day to claim the plot

- everything player generated

- when a plot is evicted, everything gets claimed “by the house” and added to a market for sale

- the eviction market items will be at the cheapest price

- you can only buy and sell from adjacent plots

- sell orders only

- buy orders through ongoing contracts

- one plot is not enough to make everything

- space or farming theme

- activities include

  - clearing land

  - building shelters for equipment and people

  - allocating land to crops

  - allocating land to transport

- every plot has limited space

- every plot has a few of the total number of resources

- other resources must be purchased

- building space could be lagrange points or land area

- each building space will be better/worse at different things based on proximity to resources

- set up trade contracts with neighbours to provide resources/time

- different levels of technology

- higher tech requires more players working together

- travelling to trade hubs means you cant micromanage your land during the travel time.

- “change points” build up over time

- these are spent to change stuff

- changes and plans are made in planning mode so you can see the overall cost, effect and time to construct.

- “tax” is charged to build world wide infrastructure systems

- everything builds from nothing

- more plots become available as the waiting population grows

- players build markets to allow more trades to take place, and to collect tax

- these allow players to advertise their needs over a larger area

- there are associated costs with purchasing trade items in shipping them to your door

- charge players fees for storage

- leave reviews of players for other players to read

### Psuedo-Proc gen

using a bitmapimage of the moon we can create a pseudo random level. Each pixel on the map represents a 1km square area. Using the proc-layer method we could do:

Layer 1: Generates a set of points representing craters from the bitmap data (or manually)

Layer 2: base height is generated from the pixel information

Layer 3: Links to neighbouring 1km^2 tiles are created based on height difference

Layer 4: each tile gains 100,100 tile map random points of hard stone, resources are generated. Each point has a weight and depth, which will determine how available the resource is.

Layer 5: stone links to surrounding tiles are made

### maintenance system

each maintenance task need has a severeity of 1-10. This severity determines how many resources are needed to repair it and also how much labortime it will take. DIstance from the laborshed, to the stockpile where the resources are kept and the travel time to the maintenace site all need to be factored in. Regular low severity maintance tasks build up over time regulary. Larger severity tasks will happen by chance (meterite impacts, motors jamming, ect). Each maintenance task reduced the efficency of the object, and also increases the chances of a more severe task happening.

The time it takes to keep everything maintained could then be effected by efficent site planning, keeping resources you know will be needed close by in a stockpile, and having labor available to jump on the task when it happens. There would be some sort of priority system for this (which tasks get completed first).

This also means that while the player is offline, MOST tasks get completed but there will always be some that are required. The player can re-prioritize these tasks to increase efficiency of the site while he/she is offline. Also not logging in means the site will eventually grind to a standstill.

### Resources type

if the game were based on the moon:

- sulfur concrete

- raw basalt -\> to be sintered into bricks

- fiberglass

- anhydros glass

- silicon mesh

- ferric metals

### So to begin what do we need

player authentication: to begin with each client exe can have a unique identifier. Perhap just use IP addresses?

spectator client: just allows players to load up the game and looka round

the developers would have the only playable versions

It would be important to have new versions not break the old world save.

single server for sure

### proof of concept

anything that would need to be simulated realistically should instead just be simulated randomly, or use a rough approximation

assume all action is taking place in craters

terrain is predominantly flat or gently sloping

use the start of the crater wall as a hard barrier

generate rocks and undulations proceedurally

shadow and day/night cycle in real time - 14.77 hours day/night

two objects: lander and rover

tracking objects with the camera.

rover has a more zoomed in camera view than the lander

satellite view shows no details, only simple topography

rovers will move to a point, and collect samples to bring back to the lander

each sample result will be marked on the map

terrain is proceedurally detailed as these rovers travel, using a layers system

basic heightmap generated from lunar images.

rovers only move during the day

UI options:

track next/previous object

zoom out to satellite view

enable/disable sample overlay

Gameplay

- plot maps - limited spaces

  - to start with could be simple slots or tile system

- overworld map showing how plots are attached

- observer mode

- labor units - work done per tick

- Housing, Stockpiles, Utilities(Power, Water, Food, Air), Garage structures

- 3 different tasks that need to be completed for maintenace

- pathfinding for determining task completion

- 5 different resources that are in demand from the NPC market (h3, metals, rare metals)

- collection buildings for each

- prospecting structure for exploring your plot

- beginning plots have different levels of access to each resource

- NPC market wagon that visits each plot in sequence, long travel time between them

- simple vehicles/items to assign to tasks to have them completed faster

- all items should use the maintenace system explained above

- expansion and construction items need to be purchased from the NPC market to begin with

- NPC buys basic resources that you create

- limited NPC buy orders to fill. Sign up to fill them and if you fail then you will suffer a trade boycott for a set amount of time.

- unfilled trade orders can be filled by others on the route

- the price is better if you complete a trade contract

- players want to take contracts for the better price, but risk losing the option for a time. A player can steal a contract by undercutting.

- prospecting for the available resources should be a main early game task

- the player does not know which resources are on his plot to begin with

- all resources expire, slower if packed correctly, which costs more resources and takes more space.

### Abstracting resources

The aim of having many different resources is to create a more interesting system, and to ensure a need for trade. However the actual gameplay effects should not be discounted. The player motivations for resource collection include

- to increase their power in the game world

- to ensure survival of his base

Internal pressures will be predominantly quality building space. Larger investment in a single process will be far more efficient, but these structures will be both expensive and limited in their placement.

External pressures will be from other players supplying goods at cheaper prices. Thus players will need to work to be better at producing particular resources. Specialization is the key to competition.

The actual difficulty of surviving should not be great. Players should be free to focus on developing their plots of land without struggling to keep their heads above water. The pressure to run a base close to the redline will come from competition.

Abstracting the descriptions of the resources too much will result in a system that is not intuitive. So lets work with intuitive names:

- raw material: goes through several processes before it is ready

- structural components (walls, floor, supports)

- utility components (pipes, power lines)

- living components (to build anything that a human needs to survive)

- maintenance parts (adding more types later)

- organic consumables (maintenance parts for living creatures)

- atmosphere (perhaps could be abstracted)

- export material (something that the player wants to sell but cant use himself)

- enabler resources (something the player cant build himself and wants to buy)

these resources should be available at varying levels for each player. Each plot should end up with an excess of one or two types of resource, and a deficit of at least one. This should encourage trade between players who want to develop faster.

npc finished products should be different from player built ones, in appearance, function and specialization.

storage ideas

all commodities need to be stored in the correct way to avoid spoilage. the player builds storage areas which house a particular surface area of containers. these containers can each hold one or more item types.

vehicles and hand equipment must also be stored indoors to avoid excess durability loss.

ther must be a better way!

inventory management should promote players keeping only what the need. the cost of storing excess items shuld be indirect and hard to calculate. it also needs to be easy to access, or automated.

the number of itrms could be decreased greatly, instead there could be many more types with different sizes.

The placement of structures

i would think two types of terrain will work well. stone for rigid structures, while lightweight contruction could be built on regolith. ciuple this ith surfzce strip mining ans perhap space will be limited enough. the sysems should cause players to self regulate their buulding habots. also second gen manufacturing will use all the space for processing, and not be collecting resourcs for themselves.

abstraction of structures?
