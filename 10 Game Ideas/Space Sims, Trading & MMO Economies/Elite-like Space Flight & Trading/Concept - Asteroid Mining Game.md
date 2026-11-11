---
title: "Concept - Asteroid Mining Game"
source: "Game Stuff/Game Ideas/Concept - Asteroid Mining Game"
modified: 2016-05-08
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Elite-like Space Flight & Trading]]"]
concepts: ["Asteroid Mining Game", "Design: Economies"]
words: 594
summary: "Design for an asteroid mining game where a ship anchors to an asteroid, deploys tools, manages cargo holds, ports and prices for arriving merchant ships; includes a full class structure and update loop."
tags: ["area/game-idea", "project/elite-like-space-flight-trading", "type/design-doc"]
---

Asteroid Mining game.

- Your ship is “anchored” to an asteroid and you need to fill your hold with valuable resources. Merchant ships arrive at regular intervals and you sell your cargo to them.

- The players actions are

  - Choosing where to deploy mining implements

  - Choosing what each cargo hold contains

  - From which cargo is each docking port selling

  - What price is each cargo port selling

  - Transferring between cargo areas

  - Choosing how to allocate freighters

- The player's goal is

  - Earn the most money from the asteroid set before moving on (get a new seed)

  - Utilize 80% of the asteroids value the fastest

- Your ship has

  - A maximum number of controllable mining implements

  - A number of small freighters to bring resources back from implements

  - A set of cargo holds

  - A set of docking points

  - A set of filters (to divide mixed ores)

- You can view a list of local prices for each material.

- You allocate different holds to different resources and set a price for each.

- Cargo ships arrive at regular intervals (you can see countdowns for each of them) and will collect/purchase from you whatever is going to make the best profit.

- Each asteroid has a number of faces, each with a list of resources.

- Mining too fast means you get a greater percentage of overburden (worthless)

- You can set a resource to have a negative sale price, so that ships will dispose of the waste OR you can dump it to space, which gives a time based debuff to all future mining on this asteroid.

- Each mining technique has a bunch of stats:

- Each asteroid face has a number of layers

- What is generated at the start of the level (or what is chosen by the level designer)?

  - Player ship

  - Asteroids in area

  - Rate and type of cargo ships arriving

See Below for class structure

Class Structure

Classes

Belt

asteroidlist (array - Asteroid)

distancefromstation (int)

Asteroid

x,y (int)

wastelist (array - Pile)

facelist (array - Face)

Face

deployedtool (Tool)

layerlist (array - Layer)

\*deploy(Tool) = boolean

\*get_mined_by(Tool) = Pile

Layer

resourcelist (array - Pile)

thickness (int)

surface area (int)

density (int)

boredepth (int)

borearea (int)

\*get_mined_by(Tool) = Pile

Pile

quantity (int)

resource (ResourceType)

\*combine_with(Pile) = Pile

ResourceType

resourcename (string)

volumeperunit (int)

Ship

control quantity (int)

toollist (array - Tool)

baylist (array - Bay)

freighterlist (array - Freighter)

portlist (array - Port)

filterlist (array - Filter)

connectionlist (array - Connection)

routelist (array - Routes)

\*connect(Bay/Filter/Port) = Connection

\*create_route(Tool,Freighter) = boolean

\*list_offerings() = Pile

Route

cyclelength (int)

cycletime (int)

volumepercycle (int)

from (Tool)

to (Bay)

\*update_time() = boolean

Connection

from (Bay)

to (Bay)

rate (int)

isplayercontrolled (boolean)

\*transfer()

Bay

volume (int)

transferrate (int)

contents (array - Pile)

\*store(Pile) = Pile

Port

offeredresource (Pile)

saleprice (int)

transferrate (int)

dockedship (Freighter)

\*set_offered(Pile,int)

Filter

processingrate (int)

\*process()

Freighter

isplayercontrolled (boolean)

speed (int)

dockingspeed (int)

transferrate (int)

volume (int)

Station

purchaselist (array - BuyOrder)

merchantlist (array - Freighter)

processingcost (int)

\*calculate_value(Pile) = int

BuyOrder

resourcetype (Resource)

targetquant (int)

currentquant (int)

consumption (int)

minprice (int)

maxprice (int)

Tool

speed (int)

dockingspeed (int)

drillingarea (int)

maxdepth (int)

boringspeed (int)

unitscollected (int)

reclaimationrate (int)

cycletime (int)

controlcost (int)

volume (int)

contents (Pile)

transferrate (int)

\*store_in(Pile)

Update Loop

Tools Drill

Store in Drill

Connections to Filters

Processing in Filters

Connections out of Filters

Bay to Bay Connections in order

Bay to Port Connections in order

Port to Freighter connections

Routes in order

Update Freighters in order
