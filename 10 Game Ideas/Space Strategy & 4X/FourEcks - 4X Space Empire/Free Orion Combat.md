---
title: "Free Orion Combat"
source: "Game Stuff/Game Ideas/Free Orion Combat"
modified: 2014-09-24
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["FreeOrion Combat Redesign", "Design: Space 4X Combat", "FourEcks / 4X Space Empire"]
words: 1545
summary: "Detailed redesign proposal for FreeOrion tactical combat: tactical locations per system, long range phase, detection/stealth levels, fleet discipline, ammunition, supply/blockade rules and reaction options."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

Free Orion Combat

Aims:

- A simple to understand, quick to configure battle arrangement that is interesting to engage with

- More control over battle outcome, risks and consequences

- Increase in time-to-kill of spacecraft

- More prominence of attrition battles

- Increase in opportunities to retreat

- Increase in difficulty of blockading a system

- visualisation of ships in space

- information warfare is more important and powerful

- opportunities for 3+ player combats

Concepts

- discrete tactical locations based on system generation

- stick with the three-step battle already implemented

- long range vs short range combat (Long range phase)

- fleets as smallest control unit

- Harassment of defence fleets, or of blockading ships

- Guerilla tactics an option

- Place importance on keeping supply open for both the attackers and defenders

- Discipline meter for fleets

- designed subsystem degradation

- Ammunition

- Hitpoint increase

**Phases of Combat**

Some of these take place before the player has interaction, and the rest after. The new phases of combat are:

- Detection

- Players move fleets

- Long Range Combat

- Close Range 1

- Close Range 2

- Close Range 3

- Out-System Movements

**Hitpoint Increase**

Ships need to have somewhere between 50% and 100% more hitpoints in this system.

**Abstraction of Long Range Combat**

All long range combat takes place before any of the combat phases. Fleets which did not move can fire long range attacks. Each point of long range combat is randomly assigned to an enemy fleet (even those that moved). Then each fleet reduces this number by its available Point Defence score, and the remainder is allocated randomly to the fleet in allotments of 1 damage. This is to represent the wide variety of long range combat (system wide missile, mine and optical combat). After this is resolved, the standard three phases are carried out.

**Close Range Combat**

Close Range Combat only occurs when two opposing fleets are at the same tactical location. This works the same as existing combat.

**Levels of Detection**

Matching Stealth with Detection means you can see the exact makeup of a fleet, Hull class, size and quantity of ships, total attack/defence. Having higher detection by 20% means you can see the damage that a fleet has sustained and the stats of each Ship Design. Having 20% higher Stealth means you opponent will only see the quantity and size of ships. Having double Stealth means your opponent will only see the quantity of ships rounded up to the nearest multiple of 10 (for 2-99 ships) or nearest multiple of 30 for (100-999 ships). Detection and Stealth can be modified based on the Tactical Location you take.

If a fleet takes part in Long Range Combat then its LR Rating is visible to all opponents

If a fleet takes part in Close Range Combat then its CR Rating is visible to all opponents

**Discipline Meter for Fleets**

Each fleet has a Meter showing how organised it is. When formed this meter drops to zero, and when modified (ships added/removed/destroyed) this meter drops by an arbitrary amount. These meters go up much faster while stationed in a system with a Drydock, but also increase slowly when in systems with supply. The meter is a direct modifier to the fleets attack rating. Larger fleets have a higher maximum bonus, but smaller fleets are more tactically adaptable.

**Battle notification**

Each player should be notified about each battle which is taking place. Players can only adjust their battle strategies once per turn, and the resolution of their choices is carried out during the next movement phase. Ending the turn should not be possible when battles are outstanding without the player verifying he is uninterested.

**The Tactical Map**

Each system has a map showing each of the Tactical Locations available. These include each of the planets, asteroid belts and starlane exits in the system. Specials should be displayed next to their relevant location. Hover information about each location should also be available. There is also a special location for each starlane exit which displays the name of the linked system.

**Tactical Locations**

Each tactical location can have a number of modifiers to fleets that are stationed there. Asteroid Belts and Large Planets will increase Stealth, Gas Giants might increase supply, while high gravity planets could increase effectiveness of Point Defence.

**Fleets and Fixed Emplacements**

Colonies, Outposts and Fleets are all shown as objects on the Tactical Map, each located at one of the Tactical locations. Objects cannot be in between these locations.

**Colony and Outpost as Combat entities**

Based on research, Colonies and Outposts will have a set of combat characteristics. Each has similar stats to a fleet but cannot be moved. The Long Range damage stat represents Mines, Orbital Laser Batteries and System-Wide cruise missiles. The Short range damage and Point Defence represents a fleet of non-ftl interceptor craft that the colony has at its disposal. Larger colonies may also generate movable in-system fleets for use, that can be moved between locations (but can’t leave the system).

**Player Interface**

When opening a Tactical System map, the player can interact with his/her movable objects by dragging and dropping them to a new location. Every movable object can be moved to any of the Tactical Locations each turn. The enemy players cannot see your moves.

After dragging fleets about you can hover a tactical location to see the likely effect of a battle at this location. This quick calculation only takes into account intelligence on ships you have detected, and assumes that enemy fleets will stay where they are.

**Battle Playback**

When a player opens a Tactical System Map he/she is presented with an exact view of the current situation. By selecting “Playback” the player can see what each fleet did in the last turn, and see the choices his opponent made. This is to glean some idea of the overall strategy. To playback the whole event, the player needs to click through several times, so that they can stop at each phase to see what happened.

**Reaction Options**

Each fleet can have a reaction option set just as they have now. Engage, Hide or Retreat. Engage means that the fleet will participate in long range combat if not moved, or will move to the new location specified. If an enemy fleet is in the same Tactical Location they will fight three rounds of Close Combat.

Hide means that the ship will stay where it is, gaining a Stealth Bonus, and a Detection Malus. If an enemy fleet moves into the same Location then one round of Close Combat will be completed and then the Hidden fleet will move to an empty Tactical Location. Hidden Fleets can still be damaged by Long Range Combat (and may use Point Defence) but will not participate in it.

Retreat means the ship will move to a Starlane Exit, engage in 3 rounds of combat (in which the last round they do not fire) and then leave the system via that exit. Retreating Fleets will take into consideration their Fuel level when choosing an exit and will prioritize connections to friendly systems over others.

**Target Selection during Close Combat**

Fleets will randomly engage one enemy fleet at the same Tactical Location, prioritizing Fleets that are Engaging, over those that are Retreating, and those that are Retreating over those that are Hiding. Each ship in the fleet will fire upon a random ship in the opposing fleet just as they do currently.

**Supply**

A system can not be blockaded from a single direction. If makes blockading systems behind enemy lines harder, as they will have several starlane exits all linked to the empire. Frontline systems will be much easier to blockade. Attackers will also need to keep their exit from being captured.

**Ammunition**

Each fleet has a collective amount of ammunition available, represented as “number of phases of combat at full capability”. Engaging in LR combat uses one ammo, and CR combat costs one per phase engaged in. If a fleet has no ammunition then it suffers a 50% malus to its damage output and cannot engage in LR combat. If a fleet is in on a Tactical Location that is in Supply then it does not expend ammunition. If it is at a Tactical Location in supply and does not fight, then it regains one phase of ammunition. This gives the aggressive side a time limit in completing its goals, and could see rolling system based combat with peaks of intensity. Also, the attacking fleet can “siege” the defenders by controlling all star lane exits and then initiating Guerilla combat. Defenders could also use stalling tactics until reinforcement arrive.

**Winning a Battle**

Obviously if you destroy all of your opponents forces you win, but Now there are levels of victory. You could occupy a system without conquering it long enough to establish a colony or outpost. You could make a lightning raid against a special resource, costing your opponent its bonus for a few rounds. You could simply blockade a single exit until your opponent makes an aggressive move. You could keep his fleets tied up in Guerilla warfare for many turns, cycling your fleets to keep them fresh while your opponent is whittled down.
