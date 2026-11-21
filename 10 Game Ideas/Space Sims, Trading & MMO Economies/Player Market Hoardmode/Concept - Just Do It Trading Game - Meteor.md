---
title: "Concept - Just Do It Trading Game - Meteor"
source: "Game Stuff/Game Ideas/Concept - Just Do It Trading Game - Meteor"
modified: 2020-12-11
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Player Market Hoardmode]]", "[[EVE-like Player Economy]]"]
concepts: ["Player Market Trading Prototype", "Player Market Hoardmode", "EVE-like player economy"]
words: 557
summary: "Prototype spec for a player-market trading game where buy/sell orders are set by tagging inventory items with barter ratios; includes screens and failure analysis (dummy accounts). Opens with a self-reminder to just build the mechanic."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/player-market-hoardmode", "type/design-doc"]
---

I want to make a player market trading prototype to test a new way of creating market orders. Every time I try to make this I end up designing some crappy systems to control resource flow and attempt to make the game fun.

Listen to your own advice Ben! Just make the damn mechanic you want to test.

Aim:

- A commodity trading game where you set market orders (buy/sell) by simply tagging items in your inventory.

- The system must not support multiboxing

Components

- Inventory System

  - Objects stacked by type

  - Able to add “Ghost” items to reserve slots for items that you don’t have yet

  - Limited Capacity

  - Reserving space for resources

  - 25-30 different item types with simple icon graphics and names

- Trading Inventory

  - In inventory, selecting a type of resource allows the player to set your buy and sell price for each item.

  - This is a barter system, and the player is setting ratios between items.

- Get Resources Screen

  - Probably included with the inventory screen

  - A player can click a button to get some resources for free (randomized)

  - After receiving resources there is a cooldown before more can be acquired

  - There are a number of different resource packages with increasing cooldown lengths and decreasing items per second.

- Buy screen

  - Select the item you wish to buy

  - Based on your sell options, the best offers from other players will be made available to you.

  - These offers of course do not take your ratio tags into account, but only find players who are offering the item you want, and want the items you have

  - Button for temporarily flag all my items as sellable (initiated deals only)

  - sales are logged but the buyer/seller remain anonymous

- Get Score screen

  - Players are given a set of “sales” they can make

  - these sales are a combination of items

  - more complex combinations are worth more points

  - sales are randomized and are replaced as soon as they are made

  - scales give players score which is tracked on a rolling highscore board

Gameplay Drivers

Well, there is not much gameplay to be driven here, but the goal is to test the mechanic. Getting things for free and matching them into sets should be enough to get players to keep playing for a little while.

Benefits of the new system

I mainly designed this new sales system to lower the entry barrier to players. Many trading games have complex trading set ups and I think this causes a lot of players not to bother with that component of the gameplay.

When players become idle they will continue to offer trades until no more trades can be made.

Players can see what they need and the supply/demand of each item can be modified through both resource generation (faucet) and “sales” (sink) at any time. This could also be seasonal/fluctuations over time to ensure stagnation does not occur.

Failures of the New system

Not exactly a failure with the inventory mechanic, but with the simple simulation overall. Once enough players are involved someone will discover that you can make dummy accounts with fixed ratios for two items that will flatten out the supply/demand curve. A fluctuating system would work better for this
