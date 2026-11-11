---
title: "BS - Surface Generation"
source: "Game Stuff/Game Ideas/BS - Surface Generation"
modified: 2013-06-12
type: design-doc
area: design-theory
status: "designed"
projects: []
concepts: ["Design: Procedural Surface Generation"]
words: 297
summary: "Ordered list of procedural planet/surface generation layers: heightmap, faultlines, rivers, erosion, forests, minerals, then placement of ruins, cities, towns and roads."
tags: ["area/design-theory", "type/design-doc"]
---

BS - Planet generation layers

Create randomised heightmap

Create faultlines

increase/decrease height along fault lines (volcanos) to create stone layer

randomise meteor impacts

determine catchment areas

create rivers + set ocean level

erode stone layer along rivers

erode stone layer to create soil layer

determine rainfall (or use uniform rainfall)

redetermine catchment areas

erode soil layer along rivers

create lakes

erode cliff faces (coastal and inland lakes)

create rain shadows

Grow basic plantlife (grasses and shrubs)

Pixellate basic plantlife area to place forest locations

Expand Forest locations outwards, increase height from the centre during expansion.

Mask water level and stone layer (mineral layer)

break into three depths

randomise density in each depth

From catchment areas, determine best 5 flattest soil layer areas.

Remove options not connected to the ocean

Find location nearest to the biggest mineral deposit that is also next to any river or lake.

Place capital city ruins

remove forests in a solid circle around this point.

Determine arible land around area and place settlements on best locations (random quantity). Uses rainfall (median value is best) and soil layer flatness

remove forests in smaller area around these points

Build cities at the other options from before (even if they are not connected to ocean)

build roads between all settlesments and the nearest city. Also roads between the nearest cities.

Select land area adjacent to roads and place towns

Place additional towns based on shallow mineral density that are nearby to existing towns (based on travel distance, using roads)

build roads to these towns

Increase the quality of roads between these cities and the nearest cities. Also between cities.

Determine distance from a city based on road distance for each town.

Increase the size of vital towns (those that are close to mainroads will be larger)
