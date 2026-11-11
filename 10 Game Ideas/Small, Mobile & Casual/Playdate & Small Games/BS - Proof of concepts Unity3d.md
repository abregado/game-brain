---
title: "BS - Proof of concepts Unity3d"
source: "Game Stuff/Game Ideas/BS - Proof of concepts Unity3d"
modified: 2015-12-15
type: planning
area: past-project
status: "idea"
projects: ["[[Playdate & Small Games]]", "[[The Factory]]", "[[Ice Tribe - Ice Nomad|Ice Tribe / Ice Nomad]]"]
concepts: ["Unity3D Proof of Concepts", "The Factory", "Orbital Pathfinding Threat Map", "Ice Tribe / Ice Nomad"]
words: 698
summary: "List of small Unity3D proof-of-concept tasks: morphing polygon, terrain, orbits and pathfinding, threat, The Factory room character, weapons, FPS freeaim, movement modes, modular ships, diving character, asset POCs."
tags: ["area/past-project", "project/ice-tribe-/-ice-nomad", "project/playdate-small-games", "project/the-factory", "type/planning"]
---

Proof of Concepts

make a Polygon shape that the camera is focused on, that you can rotate around. Once face is colored. Click that face and the shape morphs into a new shape with more faces. Repeat. change material as you progress, tell a story with texture, simple sounds on each change.

State change of an object (empty space, ice hole, igloo) building animation

Simple Environment with a prefab

Prefab can be clicked and several options selected

Each option transforms the prefab in a different way

Each transformation takes an amount of time

Timer is visible to the player

Maximum number of transformations

Current and Max transformations visible above prefab

Terrain and environment design using Unity3d Toolkit

Dry area (no/little water)

Texturing based on height and proximity to placed meshes

Stick to a non-realistic theme

Plant life customised and distributed

Simple assets from Terrain Asset Pack

Minor retexturing and colorization

Flying camera viewpoint

Fog/Viewdistance calculated

Day night toggle (not smooth cycle)

Object data stored in external file. Load and Save game states.

Random variables at runtime

variables effect object movement (speed, orbit distance)

variables effect object size (scale, colorization)

Option to randomise variables

Option to save randomized variables to a XML

Option to load previous XML variables

Orbiting bodies and pathfinding between them

Objects use kepler orbits on a 2d plane (zero eccentricity)

Objects are all spherical

All objects have their orbit shown as a line

Objects can have sattelites

Objects can be formed into rings or belts (same orbital distance)

Travel max speed and acceleration are variables settable during game

Pathfinding determines where the target will be after a certain amount of time and

caculated trajectory of object

Path drawn as a line

Path avoids other objects

Velocity of firing object added to the speed variable.

Gravity has no effect on fired object

Orbiting Bodies and dynamic threat on nearby objects

As above for object placement and movement

Each object can have a total threat generation assigned

Globally threat falloff due to distance is a variable

Objects inherit threat value from all other objects

Optimize so that objects without threat generation are not calculated

Display total threat as color

Simple character moving between rooms (adventure game/The Factory)

Three rooms, each with a door to the other

Charcter is not directly controllable

Clicking on a door will cause the character to walk from the room

Level transitions (each room is a scene)

or all rooms are in one scene and only the active camera changes

Hover over GUI (explaining where this door leads)

Fixed camera viewpoint for each room.

Object interaction (open box, turn handle) first and third person

Matching charcter animations with animated props

Simple weapon model, effects and projectile with random elements

Firstly from fixed perspective. Can see weapon and target

Weapon and projectile variables are randomized at runtime

BlankFire button to trigger the animation and effect

RealFire button to trigger the projectile as well

Add in 3 toggleable viewpoints

Particle effects for projectile and muzzle flash

FPS Freeaim and delayed turning (adventure/non-twitch FPS camera)

Simple FPS character view

Simple weapon model (no firing action)

Cursor aims weapon and causes the model to turn when moved to the screen edge

Weapon tracks much slower than the cursor can move

Character turns slower than cursor can turn it

Three layers of tracking

Object seeking another (missile tracking a moving target)

Very Basic AI

Object detection range (sight, sound, tech, light level, movement)

More advanced AI programming

Movement Modes for straight point movement (Sublight, Skitter, Wormhole, FTL, Warp)

Mostly velocity changes and effects

Modular Ship design and randomizer (lowpoly)

Several Multipart prefabs

Frame parts

Modular parts

Particle additns to modules and frames

Controllable Diving game character (ascend, decend, air, nitrogen, stamina)

Code Modification

Asset POC

3d Puzzle Game Assests (5 blocks or stackable bricks)

3d Weapon Assests (one rifle weapon and one melee weapon)

3d Ship Asset (player ship and 3 enemy ships of different sizes)

3d Character Asset (simple placeholder humanoid player model, fully rigged and animated)

3d Scene Assets (3 simple container models, same theme)

3d RTS Assests (3 simple vehicles and one simple building)

2d GUI Assests (menu with 5 options, health bar, resource counter)
