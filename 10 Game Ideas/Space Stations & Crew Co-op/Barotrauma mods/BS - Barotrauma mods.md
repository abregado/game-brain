---
title: "BS - Barotrauma mods"
source: "Game Stuff/Game Ideas/BS - Barotrauma mods"
modified: 2023-03-31
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Barotrauma mods]]"]
concepts: ["Barotrauma mods", "Barotrauma Talent Rework", "Barotrauma Filter Inventory"]
words: 1815
summary: "Design notes for Barotrauma mods: a talent rework per job promoting behaviour, many talent ideas, and a doable/not doable list with UI items and filter inventory autofill."
tags: ["area/game-idea", "project/barotrauma-mods", "type/design-doc"]
---

# Talent Rework

Goal. Increase player interaction and give more behavioural incentives.

## Base concepts

Talents that give fixed skill increases, to the Talent owner or to others, should instead give more skill gain percentage, and only in given circumstances. This is so that these Talents promote certain behaviours over a long period of time.

Each Job should have one (and only one) talent in the base set that gives a bonus to XP for completing a particular type of mission.

Each job should have one talent in the base set that gives a recipe for an item that every crew member will want.

Multiple crew of the same Job type with different Specialisations should be incentivised to do different things. For example, If there are two Security officers, one should be incentivized to leave the submarine as often as possible, while the other should be incentivized to stay on the sub.

Talents that increase XP gain should be in the first row

Talents that increase skill gain should be in the second row and at the top of specialisations.

## Class directions

### Captain

The Captains Gunslinger specialisation should be a no-brainer for crews without a Security Officer, but the bonuses should only work when on the sub. Otherwise the Skipper tree should make sense, again only when the Captain is on the sub.

Captain should have bonuses that increase Psychosis over time to bring the cigar and pipe into play.

Alone with Myself: When you are the only one on board the submarine, all crew gain skills 100% faster. You slowly but constantly gain Psychosis.

Talents to completely remove: Prodigy, Veteran

Talents to rework: Steady Tune, Sailor with No Name, Deputy/Lone Wolf, Helmsman, Inspiring Presence/Trickle Down

Talents to move: Drunken Sailor (second row), Inspiring Presence/Trickle down (specialisation start), Deputy, Lone Wolf (specialisation start)

### Medical

The Medic is the most required fourth class. Its base Talents should all be about healing and its specialisations should be about Genetic upgrades, Drug crafting, Away missions support.

Talents to remove: Medical Assistance,

Talents to rework: Blood Donor, Firemans Carry, Medical Expertise, Bloody Business

Talents to move: Miracle Worker (top of medic tree), Bloody Business (second row), Super Soldiers (top of chemist)

### Engineer

Since it is a main class, assume it is always on the crew. Its specialisations should be On board repairs, Ranged Security replacement, Wet Away missions.

Instead of repair speed, focus on Maximum condition bonuses

Talents to remove: Egghead

Talents to rework: Grounded, Melodic Respite, Military Applications, Grid Maintainer, Buzzin’/Cruisin

Talents to move: Heavy hitter (second row), Unstoppable Curiosity (first row), Fun with Fission (Physicist start)

### Mechanic

Since it is a main class, assume it is always on the crew. Its specialisations should be On board repairs, Melee Security replacement, Wet Away missions.

Instead of repair speed, focus on Maximum condition bonuses

Talents to remove: Retrofit (but at the top of all trees), Oiled machinery

Talents to rework: Ballast Denizen, Scrap Savant/Residual Waste

Talents to move: Miner (Specialization start), MECHanic (Robotics specialization end)

### Security

As the Security Officer is one of the optional classes, its specialisations should focus on since activity. On-board Security, Open Ocean away missions, Dry away missions. It should not get any buffs to skills that the other roles use, only weapons.

Talents to remove: Gun Runner

Talents to rework: By the Book, Scavenger, First aid training

Talents to move: Tandem Fire (first row), First Aid Training (second row)

### Assistant

This is a completely optional class, but it can be specialised for new players who show up part way through a campaign. Immunity to Reapers Tax, Catchup bonuses and Bonus skill gain for being in the same room as someone else all fit in here. Specialisations should be Not specialising, following one person around, Away missions.

Talents to remove: Revenge Squad, Loyal Assistant/Treacherous Scum

Talents to rework: Crew Layabout, Inspiring Tunes

Talents to move: An Apple a Day (second row), The waiting list (first row)

## Talent Ideas

There is always a bigger fish: Talent that gives the whole crew +200% repair/welding speed for a certain time whenever an abyss creature has been killed.

Angry Leader: Gain Psychosis slowly when others are in the same room as you. +25% crew skill gain.

Paramedic: When being dragged by you, unconscious crew members lose their vitality 75% slower.

Suit status: When you are outside the sub, unconscious crew members that are outside lose their vitality 50% slower.

Not on my watch: Talent that triggers when at least 2 Players are seriously wounded. Causes them be highlighted in red and their medical status shown when hovering over them with the mouse cursor.

Pair Programming: whenever you do electrical / mechanical repairs and someone else does the same task in the same room at the same Time, you and the other player get double ability gain.

My favourite Part: Talent that lets you chose a single Ship Part. You can repair it at very fast speed and if you repair / maintain it, it gets an efficiency bonus for a certain time. You also get the current State of the Ship Part shown in the UI wherever you are. Whenever anyone else touches that Ship Part, you get an angry-debuff

Red Cross (Blood Donor replacement): use alien blood on a crewmate with 500% duration. Gain a blood pack. Happens up to three times per round.

Running Silent: double Helmsman Ability gain for the Captain while driving with passive Sonars at high speed.

Maintenance inspection: Talent that causes any Item / Ship Part to increase efficiency by a certain percentage for a certain time.

Got him!: Talent that gives the crew a morale boost (+Ability Gain) after killing an alien beyond visible range

Item: Bait - some monsters will eat their peers' corpses. Craft a bait out of alien remains that can be used during outside missions to keep aliens from attacking players for a few seconds (optionally rigged with C4).

Sampling Procedure: Killing an enemy with the Paralysis condition yields guaranteed genetic material.

Live Human Testing: Injecting a crew member with Alien Blood gives you a genetic material once per round.

Multitasker: Assistant gets double Skill if it is a different one from last time. Promotes the player min/maxing by refusing to do one job.

Eagle eye: Captain gets weapons skill in addition when they get helm skill, so they don’t mind spending more time doing it.

Culling Protocol: Enemies killed during a Nest mission will drop more loot, if you are outside the sub.

Unwilling volunteer: Medical work on Prisoners yields double skill gain, or Exp in addition.

Streber: Assistant. Double bonus from any medals you are given.

# Doable

**Medical item icon rework**

- Silhouettes based on grouping and purpose

  - Bandages have a good silhouette

- Groupings by purpose:

  - Blood loss

  - General (Opiates)

  - Burns

  - Consciousness/O2

  - Specific conditions (Paralysis, Husk)

- Use more of the icon area!

**Non-grid based Inventory**

- Show icon, but also item name

- List items vertically

- Containers hold a lot more

- Stacks are still small, but item types are displayed once each

**Behavioural Talents**

Change Talents to promote PLAYER behaviour and make their time in game valuable. Having one person who you want to do two things simultaneously creates good tension and team investment.

Good existing Examples

- Assistant gets double Skill if it is a different one from last time. Promotes the player min/maxing by refusing to do one job.

- Captain gets weapons skill for piloting, so they don’t mind spending more time doing it

- Mechanic Miner, so they always want to go out of the sub

- Captains Lonewolf, they always want to be alone.

Bad examples

- EXP bonus just for taking a particular type of mission.

- Fixed boosts in all situations

- Passive bonuses for the whole crew.

New ideas

- Setup and payoff talents

  - Killing an enemy with the Paralysis condition at 100% yields more genetic material.

- Talents that give a bonus to behaviour on the sub, or outside it, but not both.

- Specialisations that are for outside or inside the sub, creating more pressure to take certain jobs.

- Don’t give EXP for mission type, but give an action that can be more easily done when certain missions are taken.

  - Enemies killed during a Nest mission will drop more loot, if you are outside the sub.

  - Medical work on Prisoners yields double skill gain, or Exp in addition.

- Promote a player doing a particular job AND promote them NOT doing a particular job

  - +100% Mechanical skill gain, -50% Electrical skill gain

- Talents that are active when holding an item

  - +Oxygen low condition resistance when Holding a Flamer or Fire extinguisher.

  - Bonus XP for having an item in your inventory

- Talents that effect if you want players near you or not

  - Things that benefit everyone if they leave you alone.

- Talents that make you claim parts of the sub as your domain

  - Last one to repair an item gives it a bonus

- Talents that make you more popular with your crew

  - Give them extra bonuses for doing something

  - Per round items you can give

**Inventory Filters and Autofill at Station**

[*https://evilfactory.github.io/LuaCsForBarotrauma/cs-docs/baro-client/html/class_barotrauma_1_1_inventory.html*](https://evilfactory.github.io/LuaCsForBarotrauma/cs-docs/baro-client/html/class_barotrauma_1_1_inventory.html)

Every inventory has a second inventory (called FilterInventory)

Open the FilterInventory with a tool item (Quartermaster PDA?)

When putting items in the FilterInventory slots, do not consume the placing item. Instead spawn a new one.

When picking up items from the FilterInventory, do not gain an item. Destroy the item in the slot as well.

Bonus points for FilterInventory having different background color.

When docking to a station:

- Make a tally of every item on the sub not in FilterInventorys

- Make a tally of items in FilterInventorys

- Move items to fill inventories to be the same as filter inventories.

- Prepare a list of missing items to give to show on the Quartermasters PDA

- Leave remaining items where they are

- Items that needed to be moved out of inventories get put in a crate in cargo.

**Streamlined repair Interactions**

When you have a screwdriver/wrench equipped and left click on a machine that needs repair, just start repairing it.

**Ship wide inventory simple**

An inventory that is only accessible when docked at a station. It opens linked any time you open some other inventory (while docked)

**Station inventory shop**

A large inventory that removes money when you take an item from it.

**Constructor inventory**

An inventory with one of every item. When you take an item, it reduces the amount of materials stored inside as if you crafted the item.

# Probably not doable

**Swim Stayput**

Automatically have the character offset currents as much as possible. By default I want my character to stay where it is.
