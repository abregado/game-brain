---
title: "4x economy short ideas"
source: "Game Stuff/Game Ideas/4x economy short ideas"
modified: 2025-05-15
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["FourEcks / 4X Space Empire", "Design: Economies"]
words: 856
summary: "Many design notes for 4X economy and military: connection data class, fleets, sliders, slots, resource types, Unity ScriptableObject sketches, trade and diplomacy ideas."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

Connections become their own data class

Each connection has two system references

Connections hold fleet data

Military process holds settings for each connection.

Player can set aggression for all lanes

Player can set accumulation settings for each:

- Target half opponent

- Target equal

- Double

- Uncapped accumulate

You can't set zero.

If you own both sides of a connection it is set to zero accumulation

Connections include two fleets for each side. One is the active fleet, the other is the reserve fleet.

Military process equalizes ships and builds new ones in update.

Move ships from reserve to active (using logistics)

Add new/repaired/rescued ships

Each tick we need to calculate the potential and move between fleets proportionally using the remaining logistics.

Player can set a budget for military spending. It is split between:

- Logistics- how many ships can move each tick and how quickly ships come out of retreat

- Construction- how quickly new ships are made, and how quickly ships are repaired

- Support - sets how many ships you can have active

Universe handles systems occupation changing

Universe has pathfinding for connections (distance, is neighbor, is reachable)

MilitaryMode shows corrections with a central point for interactions, and two icons for Strategy.

Slider military

Front

- Connection

- Fleet fleet1

- Fleet fleet2

Fleet

- EmpireID

- Value

- StrategyEnum: Hold, Retreat, Push

MilitaryProcess

Slider eco

Each end resource is shown as a slider

Infrastructure dictates how fast the sliders move

Exploration determines how fast systems and slots are uncovered

Development determines how fast slots are utilized

Science determines science growth

Military determines fleet buildup

Admin grows as your empire grows and cannot be set. It is just a waste sink.

Each system has slots

Each slot has a bool IsUtilized

Player selects which systems are to be:

- Explored

- Surveyed

- Developed

- Defended

Exploration screen shows

- All detected unexplored systems

- All slots unsurveyed in explored systems

- A slider to decide how much is used for exploration and surveying

- If there is nothing in the exploration list, then all goes to surveying

- If there is nothing in the surveying list, all goes to exploring

Development screen shows

- List of all surveyed slots sortable

- Buttons to reorder the slots, disable them, ECT

Military screen shows

- List of marked systems, border systems

- List of active battles

- Display of how much funding is used for upkeep

- Options for each system as to what value they try to keep.

When two empires have bordering systems each can select if they want to be passive or aggressive.

**Phase 2**

Slots give different resources

Each end resource can only be made with certain slots

Tech adds Slot-Resource relationships

Each end resource has a maximum based on how many slots are available that it can use.

Slots have a changeover cost once filled

This means that not all resources will be able to moved to 100%

Trade option between empires

Generates slots for both empires based on allocation

Trade resource is split between new markets and share development

One part utilizes trade slots that neighbour empires provide and pushes others out of there are no slots left.

The other builds a % modifier up over time that boosts what others get from you.

The goal to to make empires reliant on you so they want to support you in conflict

4x economy short ideas

Every system should be good/bad on three axes, one of which is temporal, one of which is decided at game start.

Axis1 examples (predetermined):

- Matches species homeworld

- Near homeworld

Axis 2 examples (temporal):

- Exploitation cost

- Development speed modifier

- Expansion bonuses

- Timeboxed bonuses

- Potential value in future due to tech

Axis 3 examples (other):

- Production bonus

- Unique resource

- Position

- Neighbours

- Defensiveness

All meaningful pop growth comes from the homeworld. Gives a good lever for balancing early, mid and late game eco performance.

Decouple the resource used to buy things from the resource needed to change the direction of the economy. Utility/Infrastructure and money. Or, Money cannot be spent to change the economy direction.

Losing the homeworld is game over?

Large starting state so early to mid game eco does not affect balance greatly.

Resource generation objects are not destroyed when territory is taken

No storage! Excess resources for not build up. Things only cost units per time.

- ResourceType (ScriptableObject)

  - typeId string

  - Icon sprite

- ExploitableType (ScriptableObject)

  - Resource string

  - Tech string

- Utility growth = total excess resources \*0.1

- When Utility reaches the growth cap, make one change

  - Changes

    - Exploit a resource

- Resources

  - Minerals

  - Energy

  - Crystals

- ProducerTypes (ScriptableObject)

  - typeId

  - technologyNeeded

  - Input

  - Output

Resource extraction bonuses based on distance from lines between colonies, or the planets of your trading partners planets.

Asynchronous diplomatic stances. You can let people in even when they don't reciprocate.

Fixed step movement. Continuous is terrible.

Only have tactical battles when the battles is even and the outcome will be wide reaching.
