---
title: "BS -Topdown Exploration"
source: "Game Stuff/Game Ideas/BS -Topdown Exploration"
modified: 2021-07-14
type: analysis
area: design-theory
status: "idea"
projects: []
concepts: ["Design: Topdown Exploration"]
words: 381
summary: "Analysis of why exploration is hard in top-down games and ideas to fix it: beacons, look button, landmarks, environmental clues, location names."
tags: ["area/design-theory", "type/analysis"]
---

BS -Topdown Exploration

Problems with this combination

- Short view range

- Can see behind obstacles

- Expectation of minimap

- Hard to show depth or partial los blockers

- Hard to become lost

- All distances feel longer because you can't see the destination.

Possible reasons for this mix not working

- Player cannot easily make a mental map of the space

- Objects cannot be viewed from more than one angle, making them harder to remember for humans.

- 

Things that work in FPS that don't work here

- Distant, tall landmarks (skybeams)

- 

Ideas

**Travel between activatable beacons**

Avatars must stay within a certain range of beacons. To traverse the map, they need to travel between these fixed points. Once they arrive, the next waypoint is given, as well as one back. This gives short term goals while travelling.

**Look button**

The player can hold a button to move the camera in a direction they are pointing. Their character does not go off screen. They cannot move while using this option. Vernacular Drop does this

**Markable landmarks**

Players can mark objects as landmarks which then provide screen edge markers and range. They can mark up to three objects to allow for triangulation. If a landmark moves outside a maximum range then it is forgotten. Similar to beacons in Subnautica.

**Environmental clues**

Players can intuit what lies in a direction based on environment decorations. Space Station 13 does this with colored stripes on the floor tiles.

**Areas are not always the same**

Returning to old areas to check for changes could mean that the total map size can be made smaller. These map changes would need to be predictable if viewed a bunch of times. Randomization is likely to produce frustration, if used on areas of importance.

**Current Location name in UI**

Letting the player know roughly where they are, and when they exit an area may help them to chunk the map into memorable parts. Among Us does this.

**Obvious important locations**

Make it obvious which areas are destinations and which are just for traversal. Subnautica does this.

**Memorable chokepoints**

Since these will be traversed often, it is important that they look interesting. Perhaps combined with location names in the ui, make chokepoints as the transitions between areas.
