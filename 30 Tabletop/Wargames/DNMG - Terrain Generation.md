---
title: "DNMG - Terrain Generation"
source: "Game Stuff/Game Ideas/DNMG - Terrain Generation"
modified: 2014-10-09
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Necromunda Homebrew]]", "[[Other Wargames]]"]
concepts: ["Necromunda homebrew", "Design: Procedural Terrain Generation", "DNMG"]
words: 274
summary: "Pros/cons of three terrain generation approaches (procedural, pre-made tiles, hybrid) plus requirements for Necromunda-style vertical terrain."
tags: ["area/game-idea", "project/necromunda-homebrew", "project/other-wargames", "type/design-doc"]
---

# Types of Generation that suit

## Complete Procedural

- Shapes and Forms are procedural

- Randomise every asset variable

- place items randomly

CONS:

- Some terrain will be unusable

- requires each piece to have “solvability” calculated

PROS:

- Much more variety of designs

- May give more of a broken down, desolate look

## Random placement of pre-made tiles

- Hand designed tiles which fit together randomly

- groups of tiles are randomly joined

- joined constructs are placed on map randomly

CONS:

- A lot of work to create content tiles

- many variations may look “samey”

- takes a lot of tiles before decent variation

- game data becomes much larger (more meshes)

PROS:

- easier to balance terrain (tweak one tile, updates across all situations)

- much easier to code

- easier to follow a visual style

- easier to hire an artist

## Mix of both systems

- Tiles are generated randomly from smaller parts

- Available combinations of tile types randomly generated

- “terrain library” generated per map from seed

- terrain randomly placed on map

CONS:

- Even more coding work

- each tile component needs to be thoroughly tested and built to spec

- substantially more chance for dodgy polygon joins and artifacts

- needs a lot of balancing

PROS:

- massive variation

- better style fit

## Other Considerations

Necromunda terrain needs to be very vertical.

Space that is “consumed” should be kept to a minimum.

Line of sight needs to be heavily blocked.

Falling is a thing

Terrain types need to include: walkable/not transparent (walls you can crouch under), transparent/impassable(sludgepits, wireweed,chasms)

Ladders
