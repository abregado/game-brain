---
title: "BS - Fleet Combat Proto"
source: "Game Stuff/Game Ideas/BS - Fleet Combat Proto"
modified: 2021-07-10
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["Fleet Combat Prototype", "FourEcks / 4X Space Empire"]
words: 1049
summary: "Design and dev plan for a fleet combat prototype / 4X test bed: screens, update loops for combat/map/repair, fleet design sliders and modifiers, strategy and extra features."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

## Why?

to answer some questions:

1.  How complex can a system like this become before the player is overloaded?

2.  Is it interesting to have the stationary defensive platforms movable?

3.  Can a 4x be fun and engaging without planet/empire management?

4.  What constitutes an interesting choice during fleet creation?

5.  Do we really need all this "intuitive realism" (like range, rate of fire, ect) to make combat tactical?

6.  What goals does a player need on the map to be motivated (apart from just destroy everything)?

As a test bed for:

1.  Trying out multiplayer frameworks

2.  Different Combat systems (id make that part modular)

3.  Simple node-link based economies

## Dev plan

Parts in order

1.  Combat system

2.  Combat detail screen

3.  Fleet creation screen

4.  Combat simulator screen

5.  Map Screen (predetermined fleets)

    1.  Fleet Icons

6.  Shipyard screen + repair/build points

7.  Special fleet bonuses

## Screens

**Combat simulator screen**

- Select a number of fleets to have fight

- Go!

**Battle detail screen**

- Fleet unit display

  - Hitpoints

  - DPS

- Totals

  - Current Hitpoints/ Current max hitpoints

  - Current DPS/Total DPS

  - % of DPS / % of HP

- Speed

- Supply

- Icon

**Fleet design screen**

- 3 Sliders

  - Power (Shields/Speed)

  - Cost (Repair/Build)

  - Damage (DPS/Special)

- Supply value text input

- Fleet breakdown at current Supply

- Values

  - Speed

  - Total HP

  - Total DPS

  - Template Name

- Icon

**Map Screen**

- System marker

- Jump lane effect

- Fleet marker (clickable)

  - Hover

  - Selected

  - Unselected

  - Moving/Stationary/Combat

  - Relative value (to your own largest fleet) with 5 scales (icon maybe)

- Fleet movement indicator

- Destination selection

- Shipyard marker (fleet respawn)

- Fleet Selector

  - Fleet name

  - Template Name

  - Supply

  - Current DPS / Current DPS %

  - Current HP / Current HP %

  - Speed

  - Status (combat/moving/stationary)

  - Relative value (to your own largest fleet) DPS/HP

**Shipyard selection screen**

- Show local ships waiting for repair/replacement

  - Disband fleet button (get a refund on some of the value, split over the next ticks)

- Build new fleet button (select fleet template and name)

  - Fleets immediately take up their full Supply points.

  - Ships begin to be built to fill the fleet.

## Game Update loops

**Combat Update**

1.  Random turrets chosen per fleet unit (on both sides)

2.  Damage numbers randomized +/- 5%

3.  Damage is applied to targets

4.  If a ship reaches zero HP, it is disabled (70%) or destroyed (30%)

5.  If a fleet's last ship is disabled or destroyed, then it goes into limbo. Calculate the distance to the nearest shipyard.

**Map Update**

1.  Ships that have a next waypoint but no timer start their timer.

    1.  Notify owner of the destination if controlled by the enemy.

2.  Ships that have a next waypoint count their timer down by 1

3.  If timer reaches zero, teleport to destination.

4.  Store the last system for purposes of retreat.

5.  For each system with more than 2 players fleets in it, do combat update.

6.  For each fleet

    1.  update replacement timers

    2.  Update self repair

7.  Do repair/build Update

8.  If a fleet is in a system alone and it does not own it, then start a timer to flip the system (the ship does not need to stay here).

**Repair/Build Update**

1.  Each Shipyard generates points in a store

2.  Points are spent on repairing ships in the local system.

3.  If there is enough saved to build a ship then do so: Prioritize

    1.  Local ship replacement

    2.  Remote ship replacement (home systems only)

    3.  Local Ship new build

4.  When a ship is built, calculate the travel time to reach the destination. Add it to the fleet and start a timer.

5.  Rebuild timers have a flat build time + distance\*speed

    1.  Build time based on supply points

**Movement Order Logic**

1.  Find path to destination

2.  Create path

3.  If in combat, first node in path must be where the fleet came from.

## Fleet Design

The player designs a fleet to spend a certain number of Fleet Support points.

The player chooses to customize each fleet design with a number of sliders:

- Staying Power (HP) \<\> Map Speed (Jump Timer)

- Repair Cost (per Supply) \<\> Build/Replacement Cost (Per Supply)

- Damage (Damage per tick) \<\> Special Bonus (various)

Each fleet also gets one special modifier.

- Defense Assets: Increase damage and HP and jump timer over time when stationary in home systems. Builds up each tick when not in combat.

- Interceptor: Increased movement speed when in friendly territory. Builds up each tick. Resets to zero if plotting course to enemy territory.

- Interdictor: Increase enemy jump timers entering or leaving this system.

- Support: Repairs other fleets in the same system. Repaired value increases each tick when in a home system. Resets when the fleet moves.

- Deep Strike: Self Repair value per tick when not in combat. Value ticks up when out of combat.

- Raider: Ships have a higher chance to be Disabled rather than Destroyed.

## Basic Strategy

The player who more effectively uses their Support Points, and who controls choke points correctly, will have the advantage.

Since the repair/build resources are limited in production, but are also wasted if not used, Taking too much damage all at once will mean falling back, and not pushing often enough will mean wasting resources.

## Other feature ideas

Each tick spent in combat with an opponent builds points towards buying a damage bonus against that opponent's fleets. Players can convert “spare” build/repair points into these by committing cheap units to border skirmishes.

When a system has been held long enough by a player, it begins to get developed. This increases the amount of build/repair points that a player gets, but these values are removed as soon as the system is taken by an opponent.

After a certain amount of time, each player can build a new Shipyard or Anchorage. One increases the build/repair points available, the other increases maximum supply.

Players can build fleets over their supply, but it increases the repair costs and timers by a proportionate amount for all purchases.
