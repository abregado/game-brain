---
title: "BS - Bonsai Design"
source: "Game Stuff/Game Ideas/BS - Bonsai Design"
modified: 2020-12-11
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Playdate & Small Games]]"]
concepts: ["Bonsai Game", "Design: Idle Offline Progression", "Design: Tree Growth Simulation"]
words: 937
summary: "Design and todo notes for a mobile bonsai-growing game: grooming, consumables, play cycle, simulation todos, monetization, tools and buttons."
tags: ["area/game-idea", "project/playdate-small-games", "type/design-doc"]
---

Short Iteration Gameplay Ideas

Clearing imperfect leaves to maximize growth

Finding bugs under leaves and chasing them off, to get bonus growth

**The grooming phase**

After trimming and modifying the tree the player can view the tree more closely and remove small parts that look bad. Some buds and leaves turn slightly yellowish to show they are bad and will not work as intended (but still consume energy), and sometimes hidden bugs can be see under leaves or crawling on the branches. These bugs can be swatted for additional growth while the app is off. Any fruit or nuts that are on the tree can also be removed. These consume a lot of energy so will stunt the growth of both the tree and other fruit objects.

**Consumables**

Periodically the player is sent a package of consumables, maybe once per week at the slowest, but during early play they will receive some of each to be used in the tutorial. The types of Consumable are:

*Fertilizer.* This is applied to one tree and doubles the rate at which the tree grows for the next 24hrs. This also increases the amount of energy that the tree can store (based on premium level).

*Pots. This allows the pot of one tree to be increased in size. Bigger pots mean a larger maximum tree size.*

Energy Boost. *This causes fruit to grow twice as big for 48 hours.*

*Bleaching Paint.* Stops a few segments of branch from growing buds and gives them a lighter color.

**Play Cycle**

Player loads game

is shown images of each tree they have, and how many days of energy has been collected

Gifts are displayed on this screen can can be tapped to collect

Selects a tree to view

Watches new growth

Prunes/Trims branches (Instant, large impact)

Swaps pot if wanted (once per week)

**remove buds, fruit, bugs and leaves (this zooms in on the tree, more objects and details become visible)**

Swap to next tree or close program

Bonsai ToDos

## \*Usability\*

Camera reacts to bonsai size

Touch Screen camera control during tool application

Multiple bonsai stands/slots with menu display

Better display of what will happen, or a warning tooltip, when using tools

replay tools, watch again (deterministic or not?)

## \*Graphics and Sound\*

Fixed Textures from file, how does this look?

Seasonal Music Loops

## \*Backend\*

Facebook image sharing

Twitter sharing

Maximum stored growth

non-player readable save files

Branches and parent links are made using uniqueID, which are also used as the array index

breakout save/load into four steps in order (tree, branches, leaves, buds)

## \*Player Agency\*

Save/Load working correctly

Repotting Tool

Deleafing Tool

Saw tool only removes half of the branch but stops further growth (stumping)

## \*Simulation\*

More realistic sponstanious branching

Leaf dissasociation, yellowing and falling

Sun vector affecting branch direction

Random variation in environmental conditions

More Complexity in environmental conditions (sun and temperature)

no energy waste

unused energy is stored at the end of the tick

if there is enough energy for a bud, one is created

When buds change into a leaf or branch they consume the stored energy

When it is warm, sunny and there is a energy surplus, grow fruit

**\*Goalification\***

Goals per pot: Width of tree canopy is equal to the pot width

particualr shape from template

bulk of tree is below pot top

### 

### LEAF ASSOCIATION

Calculate total leaf energy, without dissociated leaves

If there is more energy than the tree needs, then it will disassociate itself from the oldest leaf

actual energy is still calculated from all leaves (including dissociated ones)

dissociated leaves will change to yellow and fall off

leaves now have unlimited life

seasonal energy modifier affects root energy, so that leaves becomes dissociated during autumn and are completely lost in winter

### Monetizations

Bring the player back each day

Maximum time saved is 2 days

The player needs to come back or “waste” their growth

different seeds for different species

offer a cut of a tree’s sales to the artist who makes it

each species could have its own soundtrack (death metal tree lol)

### Visual Style

text, video, knowledge links

panels of information about real world bonsai growth

What do I want it to “do”?

The tree should grow in pulses

The leaves should grow and fall off in seasons

during periods with low sunlight, the tree should not grow (or will grow slowly)

all other periods, the tree should grow and lose leaves, but continuously gain more leaves

in autumn, the leaves should stop growing so that they all eventually fall off

leaves should grow on the furthest branches first

sunlight as a leaf modifer rather than a fixed number

New Tool List

- Prune and Seal: Cuts a branch off and prevents a new one from growing

- Clip: Cut a branch and two new ones will grow in its place

- Lamp: Increase the average light levels

- Shade: Reduce the average light levels

- Wind: add a direction of wind and power level. Branch growth will be affected by this vector

- Pinch: Removes a leaf and replaces it with two new leaf growths

Buttons

- Pause/Play during playback

- Scrub: Select a moment to view and pause

- Tool Select/Drop Tool/Confirm action

- Second Gamestate for Tool Selection

save on close

playback on load

leaves and roots determine energy

onscreen controls

android version 1

tree types

different leaf shapes

seasons - deciduous trees

repotting: larger/smaller, limit max rootmass

water levels to control growth

flowers and fruits

gentle animation for leaves and branches

inactive buds

new sprouts randomly if there is energy left over
