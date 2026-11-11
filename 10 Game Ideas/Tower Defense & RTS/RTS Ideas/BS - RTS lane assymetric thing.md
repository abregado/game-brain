---
title: "BS - RTS lane assymetric thing"
source: "Game Stuff/Game Ideas/BS_ RTS lane assymetric thing"
modified: 2023-12-29
type: planning
area: jam
status: "prototyped"
projects: ["[[RTS Ideas]]"]
concepts: ["Asymmetric Lane RTS", "Design: Node-Based RTS Map", "Design: Extractor Placement Loop", "Design: Base Plan Setup and Leave"]
words: 549
summary: "Dated jam prototype notes (Dec 2023) for an asymmetric co-op RTS on a Spring/ZeroK-style engine: lane map, AI patrols, base nodes, extractors, commander recall, more bases than players."
tags: ["area/jam", "project/rts-ideas", "type/planning"]
---

Jam prototype things

## 29.12.23

MVP List

- Spawn units for AI player to attack us with

- AI has no factories

- Force AI to attack specific points

- Map

  - with single lane

  - Metal on the player starting area

- Custom victory condition: Destroy a particular base

- AI units replace interstitial lane bases

Thigns to Rmove

- Units using energy

- Global resources Metal/Energy

- 

## 08.12.23

### Add a unit

Just… add a new unit

### Persistent gameplay?

Can we find a way to save and load a game in progress?

ZeroK has a save load system, but does it work for multiplayer well?

Does it work with script state?

### Commander Recall

You can press a button on the command centre (first building) to bring your commander back there, or spawn a new one if yours is dead.

### Script ai attacks to make the world feel populated

Set up ai patrols in script so they march around in loops

When the patrol is killed or damaged, units are replaced.

### Gaining control of buildings and units near a Commander

Is this doable via script?

Radar coverage only from nearest/last visited base

### Information on battle state is shared amongst players

Players cannot see what each other can see.

They need to explain or direct the others

### Resource extractor placement idea

Place an extractor within range of a base

It stays and builds up internal resources

Rate is based on where you place it

When it is full it waits for you to return

When you return, you send it back to the nearest base.

Creates a loop where you go to a base, then go out to set up all the extractors, then revisit them once they are done.

Extractors can come under attack, are very tough, but stop harvesting when they are under attack.

Proximity to other extractors lowers output, therefore makes it take longer to fill.

“Easier to defend \<-\> more reward in same time” scale

Gameplay to keep one player busy

### Base plan setup and leave

Each base location has a static builder that builds slowly

The player can only place structure holograms inside the base area.

The builder builds things slowly.

When resources are available here, building speeds up

Resource capacity per base is part of the design

Resources generate automatically at a slow rate

Each structure in the base uses some of the resources per time

Base design must balance the number of structures with resource rate, or visit regularly to boost resources manually.

### Manage more bases than players

Make the map large

Each enemy base can become a player base

More players means you can keep more bases running

Good players can handle more bases simultaneously

Players are always moving their commanders between bases.

### Node based map design

Bases are nodes on the map

The paths between each node are important

Enemy AI bases only activate if they are “adjacent” to a player base on the graph.

Surface area of the player base network is important.

Number of player bases supportable is probably based on number of players

Bases in the back that are not adjacent to enemy bases do not receive attacks, so can focus their build quota on economy buildings.
