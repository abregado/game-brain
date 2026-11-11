---
title: "Concept - Factorio GeoTech Tree"
source: "Game Stuff/Game Ideas/Concept - Factorio GeoTech Tree"
modified: 2016-09-08
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Factorio mods & ideas]]"]
concepts: ["Factorio mods / ideas", "Design: Tech Trees"]
words: 649
summary: "Factorio mod design for 15+ players: tech recipes and upgrades live in Wreckages with databanks, decoded by labs and moved by radars, plus bloat features (deconstruction pacifist victory, satellites, power pole changes, seed scanner tool)."
tags: ["area/game-idea", "project/factorio-mods-ideas", "type/design-doc"]
---

## Constraints and Goals

- Gamemode for 15+ players

- Create much more variation in final endgame state

- Provide more exploration and travel gameplay

- Remove linearity of tech progression

- Add focus to distribution gameplay

- Add Pacifist victory in an interesting way

## Core Mod Components

### Starting Equipment

- Power Armor, Roboport and 10 Constructors

### Evolution Changes

- Time and Pollution based Evolution reduced to zero

### Crafting Changes

- No hand crafting of weapons, electronic circuits or armor

- Recipes available based on being near to a piece of Wreckage

### Wreckage: Available Recipes

- Each wreckage contains a databank with a fixed number of slots

- Each slot may contain either a Recipe or Upgrade

- When in range of a Wreckage, player force changes

- One force per Wreckage

- This means that within range of each Wreckage, the player has different recipes

### Wreckage: Passive Upgrades

- All passive technological upgrades (shooting speed, inventory size) available

- Alien Pheromone Upgrade: Biters are not aggressive to this Wreckage force

- Area Boost: The radius of this Wreckage databank is larger

- Slot Boost: This Wreckage Databank has more slots

### Labs: Decoding Wreckage

- Recipes and Unlocks are not available to begin with, they must be unlocked.

- When Labs receive science bottles they are consumed and count towards unlocking tech nodes in the Wreckages databank.

- Once unlocked, the recipes and upgrades become available for this Wreckage

- Once unlocked, they can be moved using the Radar system.

- Labs only contribute to unlocking techs when within range of a Wreckage

### Radar: Moving Techs and Upgrades

- Unlocked nodes in a databank can be moved by setting up Radars within range of a Wreckage.

- Each time a Radar scans, it generates a Transmission point.

- Unlocked tech or upgrade nodes can be moved to any other Wreckage with an empty slot for a cost

- Transmission cost is exponential, so it is cheaper to transmit several times to close nodes, than to transmit once a long distance.

- This allows the player to modify the level structure over time.

### 

## Bloat Mod Components

### Deconstruction: Passive Victory (bloat feature)

- Wreckage can be deconstruction at cost of Red, Green and Blue Science

- When finished, all technologies and upgrades contained within are removed from the game.

- Alien Artifacts are rewarded per technology and upgrade sacrificed

- A fixed number of Artifacts are rewarded for empty Wreckages as well

### Satellites: Making effects Global (bloat feature)

- Super long term goal for those who want one

- When a Rocket is launched with a Satellite within range of a Wreckage, Orbital points are accumulated in that Wreckage.

- When enough Orbital points are accumulated, a Technology may be moved to the “Orbital Wreckage”.

- Orbital technologies and Upgrades are global, and can be accessed from everywhere on the map.

- Final “win state” is then to have all techs and upgrades moved to orbit.

### Power Changes (bloat feature)

- Power poles have a fixed energy consumption.

- Large poles should have the cheapest consumption per distance travelled

- Substations should have the cheapest consumption per area covered

- Small poles should have cheaper consumption per area than Medium poles, to keep them relevant.

- This should promote efficient power design and simulate inefficiencies of running long power lines between bases.

### The Scanner Tool (bloat feature)

- A simple tool written in Lua to show the formation of fallen Wreckage given a specific level seed.

- Perhaps make this available as a web service so players can share good seeds and so they can share save games to compete on the same seed.

- Of course, playing with random seed will mean you need to explore on the ground, if you like that sort of thing.
