---
title: "Concept-Planet Generation"
source: "Game Stuff/Game Ideas/Concept-Planet Generation"
modified: 2013-06-12
type: design-doc
area: design-theory
status: "idea"
projects: ["[[RTS Ideas]]", "[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["Design: Planet Generation", "Shared Relativistic Civgame"]
words: 171
summary: "Outline of a planet generation process: inputs (star, orbit, disk), layered composition, density and gravity checks, molten core and tectonics."
tags: ["area/design-theory", "project/fourecks-/-4x-space-empire", "project/rts-ideas", "type/design-doc"]
---

Planet Generation Concept

Aim:

1.  Realistic Outcomes

2.  Fine Detail

3.  Topography, Atmopshere and Oceans

4.  Interior composition

5.  Surface, Air and Core Temperature

6.  Surface area calculations

7.  Defined continents

8.  Realistic Mass Usage

Phase 1: Determine Mass, Orbit Distance and Energy Input

Inputs:

- Star Radiance/Temperature

- Orbit Distance

- Protoplanetary disk Density

- Disk width

Phase 2: Determine layed comosition

A majority of the heaviest elements make up the core, while successive layers collect diminitshing amounts of the heavier elements. The crust of the planet is finally formed from the remaining material. Several checks are made once these layers are formed.

Density/Radius of the planet

Mass/Gravity of the planet

If the planet is heavy enough to liquify the core materials, the planet gets a molten core

If the planet has an inert core, its temperature is lower and may collapse on itself, becoming an asteroid/debris belt.

Phase 3: Tectonic Movement

If the planet has a molten core, calculate for each consecutive layer if its melting point is reached.
