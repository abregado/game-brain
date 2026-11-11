---
title: "Bs - 4x moddable values"
source: "Game Stuff/Game Ideas/Bs - 4x moddable values"
modified: 2022-12-04
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["FourEcks / 4X Space Empire", "Design: Moddable Value System"]
words: 119
summary: "Technical design of a moddable value system for a 4X simulation: raw, derived and collected values, priority, child collections, separate view and simulation tick rate."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

Bs - 4x moddable values

Parent object.

**Raw values**. Values based on direct input . Recorded each tick.

**Derived values**. Calculated via a function each tick. Recorded. Has a priority. Higher priority goes first. Priority zero can only use base values.

**Collected valu**es. Calculated on demand. Not recorded.

Children collections.

Each object has a number of each value type all declared in data. Data also declares which child collections the object type has /must have.

Each tick, values are calculated and recorded.

Derivation functions can read children and parent.

View is separate from simulation. Increasing spped increases the simulation tick rate. It also is increases the view update rate. Visual elements request data from the simulation every n ticks.
