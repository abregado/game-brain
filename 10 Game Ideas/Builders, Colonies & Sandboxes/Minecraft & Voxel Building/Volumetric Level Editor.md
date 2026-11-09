---
title: "Volumetric Level Editor"
source: "Game Stuff/Volumetric Level Editor"
modified: 2026-07-08
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Minecraft & Voxel Building]]"]
concepts: ["Volumetric Level Editor", "Volume-based base building"]
words: 251
summary: "Design for a simple volumetric level editor using axis-aligned additive/subtractive cubes with texture priorities, boolean operations and BSP; extras and a note that it could be a Blender plugin."
tags: ["area/game-idea", "project/minecraft-voxel-building", "type/design-doc"]
---

Volumetric Level Editor

## MVP

You create cubic volumes that are axis bound. No rotation, so every wall is going to be on a cartesian axis.

Cubes can overlap in arbitrary ways.

Editor needs tools for:

- Modifying cube dimensions

- Handles for moving one cube face in and out

- Handles for moving the entire cube in 3d and on two axis at once (like in unity/blender)

- Option for scaling cubes

Cubes have a number of attributes

- Is this a Subtractive or Additive cube

- Roof texture

- Wall texture

- Floor texture

- Texture priority

Building the level would first do boolean add operations on all Subtractive cubes so they become one mesh, then do Boolean exclude operations for each of the Additive cubes. Then flip the normals on all walls. Faces get a material reference based on the cube directional texture and texture priority. Texture priority is for faces from multiple cubes overlap.

Do BSP magic on this mess, then it’s done.

## Extra points

- Arbitrary Cube rotation

- Cube grouping

- Transform modifications on whole groups

- Multi-cube attribute editing

- Arbitrary polygons (always concave?)

- A decent set of camera options (orbit, turntable, FPS)

## Notes

Now i think about this, it could be a Blender plugin

Building the level would first do boolean add operations on all Subtractive meshes so they become one mesh, then do Boolean exclude operations for each of the Additive meshes. Then flip the normals on all walls.
