---
title: "BS - 4x Fleet Combat"
source: "Game Stuff/Game Ideas/BS - 4x Fleet Combat"
modified: 2021-07-10
type: design-doc
area: game-idea
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]", "[[Stellaris mods]]"]
concepts: ["4X Fleet Combat", "FourEcks / 4X Space Empire", "Stellaris mods"]
words: 770
summary: "Design aims and options for 4X fleet management: reserve pools, templates, adversary intel, hulks, simple power ratings, a no-ships slider fleet option and a tactical advantage mechanic."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "project/stellaris-mods", "type/design-doc"]
---

Aims of Design:

1.  Fleets should be managed centrally, and the tools should scale with fleet size.

2.  User interface scales with fleet complexity

3.  As the defender, it should be easy to press a stalemate

4.  Reorganizing fleets should come with a strategic cost, or bonuses for not reorganizing.

5.  Technology can be spent to gain an advantage

6.  Larger fleet of lower tech ships is viable

7.  It should be easier and reliable to tell who will win an fleet engagement

8.  Solar Systems should have defensive advantages that are easy to evaluate.

Admirals traits and levels determine the maximum amount of ships in a fleet that can be given bonuses.

Fleets are automatically refilled up to their planned size.

## Fix what is there with extensive changes

**Fleet manager**

Ships that are built go into a reserve pool.

Ships that are removed from fleets are put into a reserve pool.

Ships from the reserve pool can be added to fleets when the Reinforce button is pressed.

Fleets are built from Templates, which contain a list of ship types.

**Reserve ships**

Reserve ships have a location. When they are requested by a fleet, they gain a travel time to the fleet based on the distance to the fleet when they were added. The fastest way there is used, either along hyperlanes or a direct line but slower. Reserve ships do not move on the map, but just appear in the fleet after the timer is finished. If the target fleet is in combat, then it simply waits until the combat is finished before being added.

**Adversary Capability Intel**

As you fight against an empire's ships, you build up Intel points against them. When enough have been collected, a research project is made available which can give a ship bonus against that empire. These are much easier to get than generic tech ship bonuses.

**Admiral Morale**

An admirals skill determines how long they stay in combat before retreating.

**Fleets taking losses**

During combat, ships that run out of hit points are either destroyed, hulked or enter emergency ftl. Ships which run using emergency ftl rejoin the fleet after the battle, assuming the fleet won the battle. Hulked ships stay with the fleet, but do not contribute to its power and do not fight. They also slow the fleet down. An option on the fleet allows you to dump the hulks, but this leaves them as salvage in the system if you are in enemy space. If dumped in friendly space, then they are added back to the reserves after a long cooldown.

Hulks which are repaired, either by returning

**Simple scaling Ratings**

Your fleets have power ratings from 100 - 1. 100 being your largest fleet. Other fleets are scaled against this one. Enemy fleets are scaled based on relative power to your largest fleet. Combine this with Adversary Intel tech bonuses and the player should be able to more easily make tactical decisions.

## Remove the concept of Ships (Option 2)

Fleets are collections of resources, with a tech bonus applied. The player chooses to customize each fleet design with a number of sliders:

- Staying Power \<\> Map Speed

- Repair Cost \<\> Build Cost

- Damage \<\> Special Bonus

The player designs a fleet to spend a certain number of Fleet Support points.

Technologies increase the extremes of these two sliders. The damage output of a fleet is fixed based on technology level

Each fleet also gets one special modifier.

- Bombard: Increased damage caused to fleets slower than this fleet

- Defense: Increased damage caused to enemy fleets when in home systems

- Deep Strike: Self Repair

- Raider: Destroyed ships have chance to simply be damaged after retreat

Apart from what is paid as upkeep for the Fleet Support points and for repairs, ships should not have an upkeep cost.

**Retreat damage**

When a fleet component reaches zero, it is disabled. Based on its distance to a Shipyard at the time of disabling, it gets a respawn time. Once its repair cost is paid, this timer starts ticking down.

## Tactical Advantage

Separate how long a combat goes from the number of hitpoints and DPS of a fleet.

Tactical advantage is a tracked number per fleet. When TA reaches zero, a fleet can no longer deal damage and so will retreat.

TA is “damaged” by enemy fleets that are fighting it.

TA damage is affected by total fleet size and relative fleet size, and a bonus that fleets can have built into them (see sliders idea above)

Defensive structures have very high TA pool.
