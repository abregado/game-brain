---
title: "Concept - Tablet Automation 4X"
source: "Game Stuff/Game Ideas/Concept - Tablet Automation 4X"
modified: 2015-12-25
type: design-doc
area: game-idea
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]", "[[Elite-like Space Flight & Trading]]"]
concepts: ["Tablet Automation 4X", "Elite-like space trading"]
words: 555
summary: "Notes for a tablet-oriented Elite-clone/automation 4X where nodes and fluctuating-cost connections form clusters; players assign craft to routes/storage and automate resource flows. Includes loop, early/mid/end game and open problems."
tags: ["area/game-idea", "project/elite-like-space-flight-trading", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

Elite Clone ideas

Make space dynamic and interesting

- Links between locations fluctuate in cost and risk

- Different locations in isolation are not good

- Explore to find good clusters

Early Game

- Travel between nodes to find good clusters

- Limited fuel

- Recharge at certain nodes

- Find a good small cluster of low tier resources to create refuel station

- Build first respawn ship

- Find a movement collection which quickest builds respawns

- Automate this process to get more ships for automation

Loop

1.  Move between nodes spending fuel

2.  Examine node parts spending food

3.  Return to Fuel node to keep going

4.  Return to Food node to keep going

5.  Find good Food/Fuel combination

Setup Route Loop

1.  Select new route from here

2.  Select next system destination

3.  Select jump time (shows current queued other craft)

4.  Select to drop cargo or collect cargo

5.  Repeat 2-4 until return to start

6.  Calculate trip length, resources per time, jump conflicts

7.  Accept or go back a step

Connections have a random cycle length, frequency, amplitude. This effects fuel cost. They also have a cool down, warmup and time (food) cost

Warmup is fixed time

Cool down is based on number of craft in jump

Costs calculated based on jump time, not warmup/cool down.

The player can wait by a Connection to scan it.

Display as two lines, highlight points which are beneficial for the player

Costs which are higher than the maximum storage are “deadly” and will kill the player unless there is Food and/or Fuel generated in the destination node

Highlight times when the connection is deadly

Nodes have resource generation per time

Player can leave Craft in a Node to increase storage capacity

Each node only Generates one resource (Food, Fuel, Silicon, Metals)

Nodes may have more than one resource generated through Trade Automation

Each node can have a number of craft assigned to storage or to respawns.

Each craft can only be assigned if there is spare food resources

Craft can also be assigned to scout connections in this node

Automation is Accomplished by assigning Craft to routes or Storage

A craft assigned to storage consumes Food but increases max storage available to the player (for one resource)

A craft can be assigned to a route in order to share resources across nodes

The route must include nodes with fuel and food and must be circular

Routes can only be set up in the players current system

A route must be valid

A route can only be made between explored systems

At locations where a drop/unload is made, the system gains resource per tick

The player can take more craft with them, but they consume more resources

Mid Game

- Use more and more respawns to search further into the cluster

- Find a high tier cluster

- Set up complex automation

End Game

- New systems that consume new resources (weapons, armor, other)

- Trade routes with these obviously need to collect more resources to be valid

- Combine three very rare materials from great distance to make Victory Item

Problems

- Where does the second craft come from?

- Exponential expansion possible? Seems not

- Sincronizing multi jump routes will become quite hard after just a few in the same system

-
