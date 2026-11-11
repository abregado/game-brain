---
title: "BS - Survival Crafting ideas"
source: "Game Stuff/Game Ideas/BS - Survival Crafting ideas"
modified: 2024-02-11
type: brainstorm
area: design-theory
status: "idea"
projects: ["[[EVE-like Player Economy]]"]
concepts: ["Design: Survival Crafting", "Design: Equipment Durability Tiers", "Design: Resource Extractors", "Design: Loot Extraction Drones", "Design: Crafting Rules", "Analysis: Survival Crafting Collection and Crafting", "Design: Base Building", "Design: Multipoint Exploration", "Design: Forced Return Home Loops", "Generational Spaceship Dome Survival", "Design: Creature Behaviour and Spawns", "Design: Persistent Server Characters"]
words: 3157
summary: "Dated dumping-ground notes (CC0) on survival-crafting design: base/durability systems, crafting rules, extractors, drones, exploration beacons, loot and progression ideas, plus analysis of other games' collection/crafting."
tags: ["area/design-theory", "project/eve-like-player-economy", "type/brainstorm"]
---

NB4: This document is CC0. An idea being presented here does not mean I think it is a good idea. This is a dumping ground.

# 11.02.24

## No durability loss while in the base

To promote building near to the resources, or having bases dedicated to resource gathering

## Resource nodes near a base as building slots

Buildings and workbenches in your base are free, but take up supply slots. Supply slots are based on how many resource nodes are within your base area.

## No equipment and ammo inventory

Instead of producing items to build up over time, have workbenches recharge equipment an amount per minute. Tools and equipment have an amount they can be recharged relatively quickly, but additional clips and charges take longer to fill. Don’t allow the player to build up huge buffers, instead have them craft additional copies of tools and weapons to use as storage.

## Base Airlock stashes your equipment

Either a Suitport or just a room with equipment slots. [*https://en.wikipedia.org/wiki/Suitport*](https://en.wikipedia.org/wiki/Suitport)

Have the mechanics so that inside the base you don’t need tools. Then take them away from the player when they enter so they can be repaired and maintained automatically.

## Consider which are Fungible items and Non-fungible items in your design

Tiering as increasing combinations. EG:

- Tier 1 is just stats (give me the biggest number)

- Tier 2 has modifiers (give me the biggest total number)

- Tier 3 has gemstone slots (give me the biggest total of multiple items in one inventory slot)

- Tier 4 has set bonuses (give me the biggest total of all inventory slots)

- Higher tier allows more specialisation and focus, but also more combinations and harder to get exactly what you want.

Resources are pseudo fungible or only local fungible. Each item can be turned into multiple items, but the map of malleability has islands.

## Be aware of what is automatable and what is not when designing tech upgrades

Some items cannot be automated, but those items get bonus to drop rates and game advances.

## Differentiate equipment tiers by durability management system

Low tier stuff has simple durability and repair requirements. EG:

- Stone tier just has unlimited durability (the character crafts a new one every time automatically in the animation)

- Metal tier can be repaired (sharpened) with an item that can only be crafted in a base (whetstone)

- Industrial gear must be left in a workbench at a base to be repaired over time.

- Futuretech gear as Industrial gear but also has a battery that depletes when too far from the base.

Basically, the higher the tech of items, the longer they last, but the longer they are out of service. To be safe, it might be worth taking a lower tier tool on a longer expedition.

Start at “higher” tier, develop lower tier the further you go. Starter equipment works fast, is simple to use and is simpler to manage. As the game progresses, it becomes more complex, but you can use it further from the starting area. Highest (starter) tier should literally be “build a base in 1 click”. Later on you need to move the logs around from self cut trees yourself. Starter tool should be an omni tool that does everything basically automatically in a single step, later you have multiple tools and a complex production chain.

## Tech epoch for tools and equipment.

You cannot repair a high tech tool at a lower tier base. This means that upgrading to the highest tier every time has a period of time after which you want to keep all the infrastructure for both tiers. You can fall back a tech level if you get far from your base and your tools start to fail. Expansion into a new area becomes either building travel infrastructure, or pioneering with lower tech and building a new isolated industrial production base.

## Prospecting lines

Resource spawn as lines that overlap. Find the area with the best overlaps. Show the found lines on the map so players can prospect.

# 15.12.23

## What do players want as a minimum in a survival crafting game?

Maybe we should divide this up more because I feel like what players want and what they think they want are different things. So maybe let us start with “What do successful OWSC games offer players?”

- Problems to soften and then solve

- Loops that get longer into irrelevance.

- Reasons to build cool shit

- Feeling that they are making a mark on the world

- Work as a team on a goal

- Exploration: reasons to go out

- Danger: reasons to stay in

- Aha! Moments

- Feeling of progression: “remember when X was a problem?”

## Resource extractor level up

Goals for the design

- Player can do a more interesting game loop while the extraction is completing

- Move resource extraction gameplay from direct interaction to a design puzzle

- Give reasons why the player wants to come back and check on the extractor while it is working

- Align player and character goals/expectations.

- Minimise “Why can’t I just…?” moments

- Give a reason why “base in a backpack” is not what you want.

Extractor gameplay ideas

- Each resource has an optimal zone in which maximum resources can be gained.

- The generator has a maximum number of links

- Generator can only be placed on a horizontal surface

- Player can set a larger amount of total resources to gain a boost later in the harvest cycle.

- Extractors can only be placed in range of a base

- Players return to an extractor and can select to eject any resources, allowing it to continue collecting.

- Players place the core orb and not the extractor

- CLEAR THE EXTRACTION AREA!

- A smaller number of links gives a bonus to waste product generation.

# 5.12.23

## Games that I thought had good/bad collection

Horizon: hinder yourself to get more rare parts during combat

Monster Hunter: ingredients are rewards for playing the main loop

Last of Us: You don’t need to click on everything, just press loot as you walk past.

Grounded: clear locations for each resource, ingredients are gained from core gameplay (fighting)

Dying Light 2: same useless amount of ingredients often repeated

Monster Hunter: high per type ingredient amounts (grindy)

Conan: random items drop on all enemies, so why even collect?

Conan: Multiple resource types from the same node.

Empyrion: Shooting lasers at low res, low poly objects from point blank range.

Project Zomboid: You can loot everything around you from the same menu

Barotrauma: collection is always exciting.

## Games that I thought had good/bad crafting

Animal Crossing: animation pauses after every craft?!

Divinity 2: Crafted items are far less powerful than found/purchased items, hidden recipes.

Minecraft: Puzzle recipes, hidden recipes (in old versions)

ZeldaBotW: Long crafting animations

Icarus: Recipes just because it is expected, Ingredient choice to be “realistic”, multiple ingredients in a recipe that come from the same gather point (bone, fur, leather)

Spiritfarer: Skill based crafting minigames

Factorio: auto intermediates

Grounded: every item was necessary, minimal per ingredient type count, craft from nearby inventory

Witcher 3: Potions are necessary and different per fight

Last of us: Ingredients are good for two recipes each which are both important.

## I want to play it again, and I want to do better next time.

Give me things that i can do better next time

## Signs your crafting system has failed

If the player no longer knows why they are crafting something.

If the player is crafting an item and not planning on using it.

## Rules for Crafting

1.  It isn’t the core gameplay loop

2.  It does not interrupt the core gameplay loop

3.  It is relevant to the core gameplay loop

4.  It is exactly as simple as it needs to be

## Different ways of discovering information

Why build my house here? Proximity to resources, no dangerous predators,

## Don’t have a useless day night cycle

If your day night cycle is only a visual effect, and makes it hard to see at night, you failed. If the player would behave the same at night if it was bright enough to see, you failed.

## Different animal behaviours

So many games have one simple behaviour for all creatures. Turn and attack. Chase. Ect. Lethal Company managed to have every creature behave differently. If upon seeing a creature, the player’s behaviour is always the same, then the creatures can all be the same. Each creature having different behaviour based on where you encounter it is A tier. Having creatures interact with each other in different ways is S tier.

## Varied creature spawns

At a minimum have different creatures spawn in day/night. Different creatures should spawn in different areas. Let the player learn where the creatures spawn. Give them obvious clues that in this area, a particular creature spawns (tracks, dens, marks, old kills)

## Tool racks

Instead of crafting tools, you build tool racks in your base. You can only carry 1 tool at a time. If the tool is lost you can long-press interact on the holder to craft a new one. The old one, if still in the world, is destroyed.

## Loot extraction drones

After fighting or finding dropped loot, place a drone down. It will, over the next few minutes, collect all the items from the floor and then fly back to base. Now make the character not be able to carry loot, and only be able to deploy limited drones before returning to base. Sortie \<-\> Return loop strengthened without excessive clicking and inventory management.

Perhaps it is only worth placing these near where creatures spawn. So the player first needs to clear the enemies, then set the drone up, then either defend the area or find somewhere nearby where they can cover the drone.

Instead of being attackable, drones could be interrupted by creatures and send an alert to nearby players for assistance. This way a player could set up a route of several drones to keep an eye on, or find a vantage point where several resource spots are visible.

The drones efficiency could be based on the shape, size and placement of nearby nodes, so that players need to scout out the best areas within range of their base. This would promote learning the immediate base area very well so you can deploy drones on your way out to explore.

## Bases build automatically over time

Resources required are pulled out of thin air at a slow rate so that building is constant

Players can speed up construction by providing resources.

## Base building queue

The player can design an entire base, including tiers not yet accessable. By accessing a terminal, each section of the base can be prioritized to modify the order in which objects are built as resources become available. This makes the base into the build order for the current playthrough.

## Extrusion base building

Start with a cube and extrude the volumes.

## Gap based damage.

Each face takes damage, but does not have hit points. Instead, faces have a damage reduction, and left over damage adds Gaps to the face, allowing creatures to get through and atmosphere to leak out.

## Task based Xp bonuses

When you select a skill in a skill tree, you also gain a large xp multiplier for doing tasks related to that skill tree.

If a player selects a skill tree, it is probably because they want to do that job

**Aligning character and player desires makes the game more affecting**

## Per server characters

The server owner can hire crew and set which talents they have access to.

When a player joins the game, they can choose one of the hired crew.

The server owner can also set slots to be “player decided”

Money is split between all hired crew, so hiring too many means not progressing far with any.

## Join game loadout

Each player can buy items from a shop before joining the world

Limited weight stops players bringing too much

To start with, the player will not fill the weight

The first few runs see the player reach a point where they can fill the weight

Then money is spent to buy items with a better “effectiveness to weight ratio”

Consumable, unrepairable items can also be purchased

In multiplayer, all players drop together, and can leave together

Player meta inventory is stored per server

## Support fantasies

Powerful Hunter, Prospector, Base Administrator, Cartographer, Gardener, Interior Decorator

Not the real world versions! The fantastical versions!

## All construction is a blueprint

Players can “build” any structure or crafting bench in a ghost mode to plan their entire base.

## Scan drone

Throw a drone in the air that adds all nearby creatures and nodes to your view. If used within large range of a base, then additional information is shown.

## Known creature spawns

Creatures have dens that are visible. Players can collapse the dens to stop creatures from respawning here, but they will instead spawn at nearby dens and return here to rebuild.

## Known creature patrols

Creatures send patrol groups from their dens to other dens or locations. Players can tag creatures to have their paths marked on a map and warn of proximity. Large creatures might be pathed via locations that make good ambush sites.

## Weather (and night) are not downtime!

Give the player special things that can only be done at night time or during weather events, rather than just making these events more or less annoying to play in.

Suddenly players are eagerly awaiting these special events instead of trying to skip them.

## Clear locations deeper to increase output

Place a crafting bench next to the entrance to a POI, mine or resource area.

Fight your way deeper into the POI, marking resources as you find them

Creatures will unmark resources in their section of the POI given a short time to themselves.

Each marked resource increases the rate at which the POI crafting bench accrues resources

## If character progress is to be saved, then food costs go up

Time can always be advanced from a base, if all players are in a base.

When you do this, clocks are refilled from base inventory

Offline characters, who logged off in a base (bed? stasis?), also consume resources.

Other offline characters lose XP while this happens.

Player bodies/beds can be picked up and moved outside to abandon them.

Show burn rate, total resources and eta to empty for each clock resource to all players.

Any player in “time speed up mode” can cancel it at any time.

## Slow processing instead of Slow resource gain

Mining is quick and easy, no hitting a tree 100 times.

Once raw resources are deposited at the base, they take time to be changed into usable resources.

So everything is an intermediate

Crafting is automatic since raw materials cannot be used for anything

## Multipoint Exploration

Place three beacons.

Reach a point where you can see all three beacons (probably a high point).

The area is considered explored.

Cover 80% of a region to unlock all of the mining locations on the map.

Promotes finding high places or building watchtowers.

Efficiency can be achieved by always moving one beacon to make a new connecting triangle.

## Force a loop using base batteries

A base runs on a single battery which is plugged into a central location in the base.

Each battery keeps the base charged for a set amount of time.

Players need to leave the game regularly to bring a new battery.

## No mining, do combat instead

Go to an area with the resource you want (mining node, scavenge POI, ect)

Place a beacon

Fight enemies while beacon piles resources up

Finish fighting

Activate beacon to start an escort mission

Bring the beacon home while fighting.

## Quality of Life stuff

Crafting from chest inventory

Placing building components from chest

Dump inventory to correct storage

Shared storages

Auto fill clocks when returning to base

## Base as inventory

You don’t have a loot inventory on your character, just a usable tool loadout. Everything else ends up somehow automatically at your base.

## Rogue Legacy style progression

As in Icarus, players quit the map regularly.

Icarus’ loop was too long, and the benefits for starting again were too small.

More like Cookie clicker restart type, or rogue like games.

Structures and workbenches stay, but have a chance to be damaged.

# 01.01.2022

## Procedural world with boundaries

Takes place in a single dome on a generational spacecraft. Players get cloned when they die, and the world is simulated forward each time.

Overland Area has randomly placed, hand crafted points of interest. A layer of tunnels under the overland is randomly generated.

Player starting location is fixed.

Player builds a landmark to get a North direction, and a second to pin the map to an orientation.

Where the player walks on the overland is tracked, and paths begin to form. These can be widened by placing path poles which quicken the conversation to a path.

The player needs to return “home” regularly to recharge their energy. Every time this is done, the paths get weaker, unless they are marked with poles.

These poles are the way that players build up landmarks and explore the world. There is no minimap.

## Force a return home loop

Players have stamina

Movement and actions cost stamina

When stamina recharges, a little from the max stamina is removed.

Each longer action (loot, activate, ect) has a stamina cost.

If the max stamina goes below this, then that action is no longer available.

Players return home to regain stamina.

Max stamina never drops below that needed to run/jump/move.

Eventually the player can only move and not do any meaningful actions so will return by choice.

## Recipe delivery in a looter-shooter

Recipes are stored in a category of item called “Consumable tools”

These contain a number of recipes each

Each recipe requires a number of other items

Each recipe is unlocked by player knowledge

Finding one of these items is like finding an item choice.

## Craft from linked inventories

When inside your based location, you can access all inventories

## Simple inventory

Players have limited space in their inventory.

Inventory is just a list of objects.

Only resources take space (Tools don’t take space)

## Central Tool change workbench.

Central terminal where player equipment can be swapped. These objects go into the hotbar. Players can only change their hotbar setup by returning to these locations.

Limited charge tools are refuelled at this location, although other locations that are solely for refuelling are also available.

Returning to this location also fills any survival meters.
