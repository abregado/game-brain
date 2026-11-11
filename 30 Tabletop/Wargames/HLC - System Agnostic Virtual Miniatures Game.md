---
title: "HLC - System Agnostic Virtual Miniatures Game"
source: "Game Stuff/HLC_ System Agnostic Virtual Miniatures Game"
modified: 2023-08-13
type: design-doc
area: wargame
status: "idea"
projects: ["[[Other Wargames]]"]
concepts: ["System Agnostic Virtual Miniatures Game", "Design: Line of Sight and Cover"]
words: 201
summary: "List of systems needed for a system-agnostic virtual tabletop miniatures game: mesh-agnostic LOS/cover, range-band movement, 3D terrain, blind/open view, model importer, dice/Lua solver, character sheets."
tags: ["area/wargame", "project/other-wargames", "type/design-doc"]
---

Systems required to make this work:

**Mesh agnostic Line of sight and cover**

Line of sight must be calculated from any part of a model to any part of another model. When targeting one model to another, a percentage of cover is given.

**Smooth movement using range bands**

Model movement destinations can be positioned anywhere within range. Models have multiple movement ranges. If a model moves, it is flagged with the movement range it used until the next time it moves.

**3d terrain system**

Terrain is made up of similar shapes, and decorations are added automatically. Ladders, stairs and access points are added by the designer.

**Blind or open viewmode**

A battle can take place where you can see your opponents models, or where you cannot. When in blind mode, you can only see models that your models have line of sight to.

**Model importer**

Any model with a suitable rig can be imported and used. This includes humanoid models and weaponry.

**Dice roller or lua solver**

Basic dice rolling, or lua scripts to calculate outcomes.

**Character sheets and statistics**

Global statistics that all models have, and model specific statistics. Can be shown on a tooltip, mouse over or character menu.
