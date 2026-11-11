---
title: "Easter train dump"
source: "Game Stuff/Easter train dump"
modified: 2022-04-20
type: design-doc
area: game-idea
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["FourEcks / 4X Space Empire", "Design: 4X Raiding and Diplomatic States", "Design: 4X Development and Population", "Cranquest"]
words: 1308
summary: "Design dump for a 4X game: interaction prototype, system flipping and raiding, diplomatic states, resource levers, eco/mil tech, treaties, empire creation options, development, colonisation, population and overlay UIs."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

4x interaction prototype

N circles, scattered

Destroy colliding circles

Connection each to closest 3

2d camera keyboard scrollable

Drag select

Shift/Ctrl select to add remove

Leftclick new selection

Right click clear selection

When a selection is up, UI to increase and decrease appears

Story ideas Cranquest

- A difficult journey

- Personal discovery

- Answer to a mystery

- Culmination of a battle

- Meeting of two friends

- Mundane wish, extraordinary obstacle

- It's a set up

4x winning strategy is to stay at peace, but if you don't keep fighting the war will come to you. Prisoner's dilemma, the more people stay at peace, the better it is for you to go to war.

External connections get a portion of total allocated

Systems have an defensive bonus amount.

Planets and developments give a defensive bonus.

System flips if a counter fills.

No movement until one side has 2x

Double movement if one side has 3x

System flips are targetted per system.

Player can select several systems in a row and have them automatically begin to flip.

Systems first lose their ownership, then build the attackers ownership.

Raiding starts if one side has more.

Portion that is more as percent the total determines raiding strength.

Raiding steals half of what it costs

Generates fleet XP

Increases fleet attrition on both sides (more on agressor)

No static bonuses against raiding, only fleet power.

Raiding is selected per target system.

Three states: aggression (war), alert (closed borders), trade (open borders)

Player can set a link to match thier opponent, or stay at a given ratio.

Levers

- Fleet recovery (countered by attrition)

- Fleet capacity

- Exploration speed

- Survey speed

- Development speed

- Ecotech increase

- Miltech increase (per opponent)

- Infrastructure/Bureaucracy

Interactions

- Choose your status with each neighbour

- Choose a default status

- Choose fleet division amongst links, auto matching rules.

- Trade deals with neighbours you have open borders with.

- Select for each system if you want to develop, hold or release.

Trade is just resource swapping, which frees up your private sector for other things.

Each link can "carry" one trade

If both systems in a link are developed, they get more trade slots.

So, both empires must agree to develop border systems.

But this also makes them more juicy raiding targets.

Strategic resources

Choose 4 out of 5 common resources (or randomly distributed)

choose 2 out of 5 rare resources (or randomly distributed)

Each empire gets one unique resource (and can name it)

These are the resources your empire can utilize.

Ecotech bonuses are based on these.

Ecotech bonuses

Two types

- Recipe to turn a resource into a lever

- Exploitation: bonus %to raw extraction

- Allow increased development levels on planets and systems.

Miltech bonuses

- Tactics: % fleet power against enemy

- Weapons: increase enemy attrition

- Defense: decrease own attrition

- Mobility: redeployment speed

Systems have a list of generated resource/lever pairs.

Developing a system lets it produce the next item in the list

The list is revealed over time based on survey spending.

Each item costs double the previous level to survey and develop

Planets are similar to systems, but only get surveyed when colonized

Planet pop cannot exceed capacity

Capacity increases as the planet is developed

Should Each level give access to a resource as well?

Development cost and max level based on habitat compatibility.

Pop grows at its own speed

Development can only proceed if pop is maxed

**Treaties**

Defensive treaty states what percentage of your fleet (or a fixed number) must be deployed against which empires

Diplomatic treaty automatically changes your political state with an empire on a trigger

Or it could lock your diplomatic state for a given time

You can attack people to force them into a treaty

Treaties are used for subjugation as well

**Empire creation**

Options are exclusions from a rule or exceptions.

They can also be used to make the game simpler.

- Cant select certain diplomatic states

- Certain treaty options not available

- Group of planets uncolonizable

- Planets around a Type of star not colonizable

- Development limits

- Targeted miltech not possible.

- No planet development, but also no pop caps

- Only one resource but it does everything x5

- Only public sector

- Only private sector

- Military is automatically and evenly distributed

**System development**

- Player marks systems with a development level.

- 0 level means you want to give the system up

- There is a development screen where you can set the development order

- Development points are spent on top priority first

- The max you can spend per tick on each development is set in the development screen.

- Increasing this number costs you infrastructure

- Excess infrastructure is automatically spent on this.

Empires can develop faster and in a more targetted way if they are not spending infrastructure to change thier economy.

**Colonization**

Player selects any planet and chooses a desired development level.

If that planet is in the players territory it begins developing.

First level for colonies is very expensive

Price (and therefore time) is based on suitability for your species (bloat feature?)

Once a planet is developed, population can be moved there with infrastructure.

**Pop growth**

Is global to your empire

A counter ticks up and when full a new global pop is created.

The next time infrastructure ticks over, it is used to move pops to a planet.

Planets with more space are prioritized

Planets that are overpopulated cost more to develop and produce less.

Since infrastructure is spent on pop movement first, private sector cannot change while global unsettled pops are waiting

Refugees go into global pop and so must be dealt with before private sector.

Yes this means refugees can be weaponised

Overlays

- Exploration/survey

  - Select which systems you want explored

  - Select which level to survey each to

  - Selecting an enemy system for exploration will explore it if it is a neighbor system

- Development

  - Select your desired development level for each system

  - Setting an enemy systems development level to more than zero means the setting will take effect when/if you capture it.

  - Setting one of your systems to development level 0 means you will give it up. It will become neutral over time.

  - See if a system has an unsurveyed level

  - See the next developable development level for each system.

  - Hover state of system shows development progress and all dev levels

- Military and Raiding

  - See which empires you have which Diplo state with

  - Set which systems you will attack when in hostile Diplo state

  - Set which area you want to defend. Fleet power is placed automatically based on this area.

  - Set special rules for system specific fleet power.

  - See current effects of power differential and attrition costs per system link

  - See resources generated by each raiding link.

  - Hover information shows expected and actual fleet power, attrition rate.

- Economy overlay

  - See every tapped resource per system. As a total.

  - See trade links between friendly neighbours

  - See enemy income per system that you have explored/spied.

- Research overlay

  - Show where miltech experience is being generated

  - Show where ecotech is being generated

  - List each research pool

    - Miltech per enemy

    - Global miltech

    - Global ecotech

- Colonies screen

  - Screen divided in middle

  - List on one side with colonies and possible colonies

  - Overlay on map on the other side

  - Selecting colony from list shows it on the map

  - Selecting colony on the map shows it in the list

  - See next development level for each planet

  - See if a planet is in your territory

  - Select desired development level for each planet.
