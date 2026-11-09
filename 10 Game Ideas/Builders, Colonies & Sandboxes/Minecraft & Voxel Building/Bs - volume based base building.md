---
title: "Bs - volume based base building"
source: "Game Stuff/Game Ideas/Bs - volume based base building"
modified: 2026-01-31
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Minecraft & Voxel Building]]", "[[Survival Space Station]]"]
concepts: ["Volume-based base building", "Survival Space Station"]
words: 621
summary: "Implementation notes for a volume-based base-building prototype (canvas proto): floor/wall object placement rules, floor plan/bisect modes, plus first-person volume extrusion building with attribute bleed."
tags: ["area/game-idea", "project/minecraft-voxel-building", "project/survival-space-station", "type/design-doc"]
---

Claude canvas proto

Next step:

Object placing

Floor objects have a xy position, a radius and a room reference

Floor objects are represented as circles. They do not have facing.

When updating the model, check each floor object and update it as needed.

If a change makes a floor object enter a new area, put it in that area

If a floor object ends up outside an area, try to fit them in the old area

Floor objects cannot overlap

Each wall object has a 1d position (0-1, proportional of edge), a room (for facing), Size, Rules about if it needs an inside or outside edge, Rules about edge type

Wall objects are represented by rectangles with a small arrow inside to show facing. The rectangle is rotated to match the angle of their edge.

When the model is updated, check each wall object and update it as needed.

When a wall objects edge changes length, move them proportionally

If they need an outside edge and you extrude their edge, place them on the new edge

If their edge changes type and they no longer can go there, remove them

Check all edge objects fit on an edge (based on size) and if not first try to move them all to make them fit, keeping the order they are on the wall (based on proportional position). If they all dont fit, delete the last object and try adjusting them again.

Generate several wall object prototypes and several floor object prototypes with different values to test all the cases.

When in Object Placement mode, show another toolbar which has a button for each object prototype that can be placed. An area above this toolbar shows text describing the values of the selected prototype. When a prototype is selected we should also show a highlight on the model of its size and which edge/position is being hovered.

Draw another solid line around the entire models outside mode wall. Give it a gap between the outer wall and the new wall of distance equal to the width of the solid line.

Rooms are represented as 3 or 4 points in a convex shape.

Each volume has data

Each edge has data

Floor plan mode

Markers shown in the middle of each edge.

User clicks and drags on a marker to move the wall on the normal.axis

User clicks and drags on a vertex to move the vertex

Wall type mode

Clicking an edge cycles if the edge is a wall or not

Bisect mode

User hovers an edge inside a room and a preview is shown. Clicking will cut the room along that walls normal.

Start with a volume

On button press, cut it into faces, each linked to the volume.

Faces can be linked to two volumes

Click a face to cycle it off/metal/wood

Place corner and buttress objects along the face to add detail

Click to cut the volume in half

Recalc the faces.

Bs - volume based base building. First person perspective.

Players put down volumes, first designating a square on the floor, then giving a height.

When building, show a character sized object in the hologram to give an idea if the size.

New volumes can be extruded from the sides of already constructed ones.

Every object gets placed on a wall or floor.

Some objects, when placed on a wall, create another object in the back of the wall. This is how doors and pipe connections are created.

No pipes or wires can be placed freestanding, only between connection points.

Attribute bleed values given by the walls. Temp and gas exchange for example.

Walls can track a number of damages, each which apply an increase to an Attribute property.
