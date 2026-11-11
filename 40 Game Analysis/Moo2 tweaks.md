---
title: "Moo2 tweaks"
source: "Game Stuff/Moo2 tweaks"
modified: 2023-05-09
type: design-doc
area: analysis
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["Moo2 Mod", "Analysis: Master of Orion 2"]
words: 688
summary: "Wish list of UI improvements and gameplay changes for Master of Orion 2 (map overlays, fleet planning, ship design, practice battles, spy options)."
tags: ["area/analysis", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

# Moo2 UI tweaks

**General**

- Sort lists by column header

- Right click info formatted like a tooltip, but not activated on hover

- Indicate what you can right click?

**Universe Map**

- After drawing wormholes, move other systems so they never lie on top of the line

- Clearly indicate systems inside a nebula

- Fuel range shown

- Label systems in range that are unexplored

- Sensor range shown

- Show total pop on right, and a second number if it will go up/went up this turn.

- Defence range. Show travel distance in X turns for each fleet. Adjustable somewhere. To determine which colonies you can defend.

- Measuring tool

**Star System Popup**

- List planets in a row

- Info below each planet

- Mark defences

- Separate area for fleets which are “in system” and those that are “out system”

**Colony Screen**

- Ghost for transported pop

- Production with numbers

- Mark new pops

**Fleet Screen**

- Link to ship designs and designer

- Show where instances of a given ship design are on the map

- List Fleets By planet

  - Show leader

- Show ship experience

- Plan attack

  - Choose target

  - Select arrival turn

  - Select ships/fleets to participate

  - Show which fleets will be late or have to wait before leaving

- Show undefended planets (Those that enemy fleets can reach before a friendly fleet can)

**Colonies Screen**

- Show turns until next pop growth

- Mark new pops for one turn

**Leader Screen**

- Leader experience points are now shown in Leaders screen.

**Planets Screen**

- Favourite planets, and show the designation on the universe map

**Diplomacy Dialog Screen**

- Show tech level, current level and cost when trading techs

**Races Screen**

- Technologies that other races have that you don’t have are visible without initiating diplo screen (unless at war, or ignoring)

- Give description on race traits which of them will be attached to the population (in case you want to capture them during invasions) and which are not.

  - Maybe show each of their worker/troop types and the bonuses associated. Each worker icon means one thing.

- Show an estimation of chance of success when deploying spies against other races.

**Research Screen**

- Show miniaturisation bonuses and new modifications for equipment on your existing designs.

- Mark techs that other races have already

- Mark fields that you are ahead or behind in

**Ship Design**

- Show available modifications to a weapon, which is not yet available due to missing miniaturisation, as a greyed out button.

- Way to save / export / import ship designs

- Marking of ships as “deprecated” whenever they need an obvious refit (new engine / armor / computer / … tech available)

**New UI Stuff**

- Practice battles against ship designs you have scanned

  - Race screen changes

    - Are in the Race intel screen to show designs you have encountered.

    - Show designs you have seen but not scanned

    - Show how give an idea of how likely it is that this ship type is still in use

  - Flow

    - Set fleet composition for both teams

    - You can use any current ship designs, but not specific ships

    - Run one battle, then ask to run 100x super fast and give the heuristics

- Queuing movement

- Pathfinding shortest

  - Uses Wormholes

- Map based Races/Diplo screen

  - Show enemy fuel ranges based on scanned ships/ known tech

  - Show system threatened by foreign fleets

- 

**New Gameplay Changes**

- Implement SOMETHING to improve toxic planets, even if it turns them to barren on the first step.

- Add the option to create planets from asteroids or gas giants in systems that have no hospitable planet to build the terraformer with (terraforming-ship?)

- More than 5 shipdesigns

- Add an option for spies to adjust relations towards you (or other races) by using propaganda.

- Add an option for spies to do reconnaissance against other races to see, if they deploy spies against you, an estimation of how many and what their assignment is.
