---
title: "Lab week proto - Volume base builder"
source: "Game Stuff/Lab week proto - Volume base builder"
modified: 2023-12-04
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Minecraft & Voxel Building]]"]
concepts: ["Volume-based base building"]
words: 916
summary: "Design for a volume-based base building prototype: Blender-like cube placement, face moving, extrusion, subdivision, wall swapping, object placement, plus data structures and graphics workflow."
tags: ["area/game-idea", "project/minecraft-voxel-building", "type/design-doc"]
---

## Building System Description

Every time I play a survival crafting game with base building, I feel like the building mechanics are shite. Why do I need to place 6 objects just to build the smallest cube house? Generally this also requires a whole bunch of inventory management as well, changing between roof, floor, wall, door parts and rotating them appropriately.

Then it clicked. I am creating the building’s surface in these games when what I actually care about is in the volume!

Why not do it like they do in Blender? Place a cube with 1 click. Then click the faces to change the size, or extrude a whole new volume from the side. Subdivide, extrude and grab functionality all work very well from a first person view.

But that is a lot of maths. So with this prototype, let’s fix the volumes to always be irregular cubes, and fix one of their axes to be straight up. Lets disallow faces from being part of more than two volumes. Now it is very simple. Also, ChatGPT can do the maths for me now.

How extrusion looks in Blender.

[*https://drive.google.com/file/d/1jpFMX0QFFQ-4RZP2mzSFKQaM40GgBKcl/view?usp=sharing*](https://drive.google.com/file/d/1jpFMX0QFFQ-4RZP2mzSFKQaM40GgBKcl/view?usp=sharing)

## UX Axioms

Left click progresses to the next step or accepts if there are no more steps.

Right click moves back a step or cancels if there are no more steps.

Everything can be edited and the changes propagate immediately, at least for this prototype.

## Player Tools/UX Design

**Tool 1: New Volume placer.**

Hover state: Hologram blue if safe to place, red if intersecting any other volume.

Places a basic cube

Player can input a y axis rotation amount

**Tool 1.1:** Face mover along normals

Hover state: Blue if face can be moved, red if not.

Click a face that has no neighbour faces connected to other volumes

Move the mouse to select a new normal depth.

Click again to place

**Tool 2: Extrude volume from face.**

Hover state: Blue if face has no attached objects, Red if it does.

Click any face of an existing volume that has no attached objects.

Click a second time to extrude out to that point.

**Tool 3: Volume subdivider**

Hover state: Blue if face/direction combo can result in a cut, Red if not

Click any face of an existing volume where the face, its neighbours in cut direction and the opposing face are not connected to other volumes.

Mouse wheel to flip axis of cut.

Click again to cut the volume. A non-blocking wall is placed between the two new volumes.

**Tool 4: Wall Swapper**

Hover state: Blue when wall can be swapped, Red when not. Highlight objects which are on face.

Click any face of any unbuilt structure that has no structures built on it

Use the mouse wheel to swap which kind of wall will be built here.

Options:

- Open Arch. No wall here. Probably some pillar parts to show there is a division. This will join two AtmosphericVolumes

- Solid Wall. This will divide an AtmosphericVolume into two.

- Doorway wall. A wall with a cutout. Just so we have more than one option. Doorway Walls create a Gap between two AtmosphericVolumes,

**Tool 5: Object Placement**

Hover state: bounding box of object. Blue if safe to place. Red if intersecting with more than one face, or another object. Also highlight blocking face or objects.

Mouse wheel to select object type

Mouse wheel click to change direction (in/out)

Objects only placeable against surfaces (walls, floor and ceiling)

Each object has allowances as to which surface types it can be placed against.

Left click to place.

**Tool 6: Wall remover**

Hover state 1: Blue to show which volume is hovered

Hover state 2: Blue to show original volume. Second volume is Blue if join is possible. Red if not.

Left click to select a volume

Left click an adjacent volume

Joins the two volumes together into one.

## Data structure of a building complex

BuildingComplex Class

- Y-axis rotation **float**

- Volumes **Volume\[\]**

- WorldPosition **Vector3**

RawVolume Class

- Faces **Face\[\]**

- LocalPosition (centrepoint or one corner) **Vector3**

- ~~atmo **AtmosphericVolume**~~

Face Class

- sharedVolumes **Volume\[2\]**

- mountedObjects **Mountable\[\]**

- FaceOrientation **Enum (Floor, Wall)**

- FaceDesign **ScriptableObject**

- ~~Gaps **Gap\[\]**~~

Mountable Class

- Face **Face**

- Facing **int**

- WallFacingAllowed **enum**

- FloorFacingAllowed **enum**

~~AtmosphericVolume Class~~

- ~~connectedVolumes **Volume\[\]**~~

- ~~Gaps *via connectedVolumes.faces.gaps*~~

~~Gap Class~~

- ~~Connection **AtmosphericVolume\[\]**~~

FaceDesign Class ScriptableObject

- Corner cap prefab

- Buttress prefab

- Floor cell prefab

- Ceiling cell prefab

## Graphics workflow

Floors and Walls will need to be procedurally generated because they could be any size.

As a base, use a 1x1x1 cube with the origin in one of the corners. This can be scaled to any size.

### Wall Face

L shaped details are added the corners

Buttress-like bracing parts are added along the wall, based on the length.

### Floor Face

Flat grid cell like parts are placed based on length and width of the floor. There are different parts for the top and bottom of a Floor face, since Floor faces are also Ceiling Faces.

References to prefabs for each of these decorative components are stored in a ScriptableObject class.

### Mountable Objects

For the purposes of this prototype, the mountable objects will be limited to non-functional decorative items. Some examples could be:

Sessel/Standing Lamp (Floor face only, orientation 1)

Ceiling Lamp (Floor face only, orientation -1)

One way Air vent (Wall/Floor face, orientation 1/-1, creates Gap)

Control panel (Wall face only, orientation 1)
