---
title: "LD34 Binary States GFX Spec"
source: "Game Stuff/LD34 Binary_States GFX Spec"
modified: 2015-12-13
type: design-doc
area: jam
status: "designed"
projects: ["[[Game Jams]]"]
concepts: ["Ludum Dare", "Binary States"]
words: 568
summary: "Graphics specification for a Ludum Dare 34 game, Binary States: procedural HSL palette per level, tile/sprite requirements for environment, avatar, portal and crystal."
tags: ["area/jam", "project/game-jams", "type/design-doc"]
---

## Overall

Each level has its randomseed based on a HSL hue value. The color palette for each level will be based on this value.

The perspective is flat orthogonal, in which the front of all objects can be seen, but not the sides. Level objects will be “standing sprites” which are centred in the middle of a floor tile, with a drop shadow (separate).

Sprites will be scales using a nearest neighbour algorithm if necessary, but hopefully this will not be so necessary. I will endeavour to use powers of 2, sprites will never need to be shrunk.

All sprites may use transparency.

## Environment

The levels are made of walkable and non-walkable tiles. Non-walkable tiles are “walls” so their front and top sides are visible. These will be made of flat colors, selected from the proc-gen color palette, with non-animated “detail sprites” rendered over the top of each tile, based on its static contents.

The detail sprites are:

- Floor, rendered on every walkable tile

- Wall Front, rendered on the camera facing side of every wall. These are HALF TILE HIGH

- Wall Top, rendered on the top of every non-walkable tile.

- Entrance, rendered after (on top of) the Floor detail, it shows where the player starts and should not be highly visible

Your suggestion on the colors is also appreciated:

- Floor: the level base Hue but with very low Saturation, but high brightness

- Wall Front: quite low Brightness and Saturation. Almost colorless grey (to link the levels styles together)

- Wall Top: darker than floor but with more saturation. Not as colorful as the Portal, Player or Crystal

## 

##  

## Avatar

The player should be animated while moving. The player regularly stops and can either have an idle animation, or simply have its animation paused when stationary.

Each walking animation needs three directions: Side, Up and Down. The Side animation is flipped on the horizontal axis to create left and right animations.

Points:

- must stand out due to animation and silhouette as its impossible to contrast with every color in the rainbow!

- if an idle animation is used, it must be different enough to the walking animations, and must also have 4 directional versions.

- character design is up to you, but my first idea was something robotic… because I like robots!

## Portal

The portal is a hole in the ground, similar to those from the game Portal. These are animated and rendered over the top of Floor detail sprites.

- colored based on their DESTINATION level, either with a “color mask” sprite or programmatically (looks bad).

- there will be 1-2 of these on each level

- animation can include shrinking or sparkling, this is up to you.

- it must look as if the character can fall through it

## Crystal

This is a floating crystal which is the main goal of each level. It will be defined by its bright color, selected from the levels palette.

- High saturation should be used

- you could use a black and white base and I can color it programmatically (looks pretty bad)

- you could have a colored version, with a “color mask” secondary sprite

- animation could include: moving up and down, rotating, sparkling, lightning, flashing

- something could be inside the crystal

- if you want to go crazy the crystal can be 32x64
