---
title: "Game Starting Loops"
source: "Game Stuff/Game Starting Loops"
modified: 2025-02-13
type: analysis
area: analysis
status: "designed"
projects: ["[[RTS Ideas]]"]
concepts: ["Design: Early Game Loops", "Analysis: Foundation", "Analysis: Planet Crafter", "Analysis: Space Haven", "Analysis: RimWorld", "Analysis: Valheim", "Analysis: Mars First Logistics", "Analysis: Space Trash Scavenger", "Salvage Machine Game"]
words: 745
summary: "Analysis of first-30-minute loops in several games (Foundation, Planet Crafter, Space Haven, RimWorld, Valheim, etc.) followed by a designed first 5 and 25 minutes for Ben's own salvage/research-node game."
tags: ["area/analysis", "project/rts-ideas", "type/analysis"]
---

# How are your first 30 minutes spent

## Foundation

1.  Choose one of 5 almost identical starting locations. This is more of a cosmetic “personal taste” choice

2.  There is only one thing to build.

3.  Build one of your options

4.  1-2 things unlock

5.  Goto 3.

This loop gets longer as the game goes on. In the end game you only build a new thing every 20-30 minutes.

## Planet Crafter/Subnautica

1.  You only can be outside the starting pod for 60 seconds

2.  The pod contains a crafter, check it

3.  See the upgrade you want

4.  Remember the ingredients

5.  Go out to find resources

6.  Return

7.  Goto 3.

You always know what you need to find next. You will probably get distracted, but you always have this base level next step mission you are trying to do.

## Space Haven

Game starts with a pre-constructed base “that won’t last long”

1.  Follow the instructions to build one of each of the things you need to build to survive

Proper game does not start before 30 minutes is up

## Rimworld

Does nothing to help you except “Colonists need beds”

1.  See a colonist need

2.  Fill a colonist need

## Space Trash Scavenger

Regular tutorial

1.  Use Grapple to collect resources

2.  Put resources in Atomizer

3.  Collect Resources

4.  Spend Resources

5.  Goto 1

## Valheim

1.  Build an axe from the hand crafting menu

2.  Build a Hammer from the hand crafting menu

3.  Build a workbench

4.  Workbench does not work, so you need to build a house

The game just lets you figure out what to do at each step. But it does make sure you know what the goal is.

## Mars First Logistics

Shows you one loop, then just says nothing more

1.  Open map

2.  Select job

3.  Drive to pickup or fast travel there

4.  Design vehicle

5.  Drive to delivery point

6.  Goto 1

First loop takes 3 minutes! Amaze.

# Our first 5 Minutes

Player is stuck in one room

The door is clearly visible but is partially covered with broken debris

**Player wants to exit**

On one wall is a pipe output, but the player has no pipe tool.

**Player wants to know what it is**

Only tools are Pick up object and Deconstruct debris

As there is nothing else to do, the player should start clicking on things to deconstruct them

One large piece of debris reveals a Salvaging machine

Some other more interesting looking pieces drop a Power cell

Putting a power cell in the Salvaging machine powers it up and starts the drone moving. It salvages automatically.

Investigating the Salvaging machine shows it can be upgraded with drone items

**Player wants more drones**

Player finds another Salvaging machine

**Player wants more Power cells**

Eventually there is only debris that the machine cannot deconstruct.

The player deconstructs one and gains a key item

Player unlocks the door

# Our next 25 Minutes

Next area has several locked exits. Each exit is labelled.

**Player wants more key items**

Middle of the room is a Machine that needs a bunch of items put in: Research Node.

Gives the player the Pipe tool

New Research Node appears, this one with a Pipe Input.

Player adds pipe from previous room

Unlocks Machine moving tool.

New research node appears, also with an input

**Player wants more outputs**

Player moves Salvaging machines from previous room to this one

Remaining time loop

Player unlocks a door

Player sets up Salvaging Machines in new spaces

Player adds Power Cells and Drones

Player explores for special debris, machine parts and outputs

Player pipes outputs back to starting area for unlocks

Unlocks:

1.  Machine Spawner: Requests items and inputs and then creates a new machine. First machines given are in a fixed order, but then the player can choose from unlocked machines.

Deconstruct Debris tool

Player needs to click a few times on a debris object to destroy it. Some objects yield an item.

Pickup item tool

Player can pick up objects and they go into the global inventory. They can also be placed into slots.

Salvaging Machine

Has a drone that it sends out to deconstruct nearby debris. Resources are piled on the salvage machine neatly. Needs a Power cell item to start work. Eventually the power cell runs out. Power cell and drones are returned to inventory when the machine is picked up.
