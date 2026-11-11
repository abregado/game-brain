---
title: "Project Elite - Design Doc"
source: "Game Stuff/Game Ideas/Project Elite - Design Doc"
modified: 2014-04-02
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Elite-like Space Flight & Trading]]", "[[EVE-like Player Economy]]"]
concepts: ["Project Elite", "Elite-like space trading", "Design: NPC Station Economy", "EVE-like player economy"]
words: 635
summary: "Design doc for an idle/mobile space trading game where the player sets destinations and an autopilot flies; progress is reported through notifications and logs. Covers hand-designed locations, NPC station economy, events, task timing and Elite Frontier-style economy notes."
tags: ["area/game-idea", "project/elite-like-space-flight-trading", "project/eve-like-player-economy", "type/design-doc"]
---

### Player experience

The player is a space trader, but instead of piloting his craft manually through space, he only designates a destination and let's the autopilot do the flying. The actual flight is not visualised but instead the game will notify the player when tasks are completed using the notifications system (iPhone and Android).

With forward planning, a keen business sense and a little luck, the player will move up in the game world. More expensive ships and more dangerous trade routes await successful players.

### Space, Planets and Industry

While one might expect an infinite universe, this project requires locations to be hand designed and placed carefully to create the correct gameplay environment.

There must be exact the right mix of supply and demand, and enough clusters of close locations to create content for new players.

Some locations might include:

- Lagrange point stations

- Zero-g micro factories

- Asteroid bases

- Mining craft

- military staging area or carrier

- Gas giant collector

- Drydock

Each location has a series of industrial processes that convert resources at a fixed rate. Cash per installation is tracked, and as items are sold, new ones are added to buy orders. Products that are not sold very often will drop in price. A minimum price is based on the ingredients needed to make a product.

Some locations also have consumer demands, so will request supplies to keep on hand.

### Notifications

simple text notifications inform the player of the task just finishing, and the next queued task. If something unexpected happens, the notification is shown in bold or colored text. For example:// after dropping out of FTL the player would expect to receive a notification saying "FTL jump complete, approaching station eta 10 minutes". Instead, if unlucky, he might get a message "FTL jump complete, local authorities have requested a contraband search Eta 20 minutes"

### Logs

Each event end and beginning is logged for the player to review. If resources were consumed they are shown here.

### Events

There will be many types of event in the game. Some of these will be planned and expected (for example:// Spooling your drives before an FTL jump) while others will happen unexpectedly (pirate attacks or security checks). Most have variable length, and sometimes the player will only know roughly how long it will take. These can also consume resources, and also can have different outcomes based on available resources.

elite Frontier style economy

Opportunities for player run economies

Buy/sell from NPC market

Track consumption and manufacturing of NPC stations, input/output ratios and time per cycle.

Prices adjust based on stored amount and consumption.

Limited numbers of NPC freighters to balance the market

Try to go for limited everything (parking slots, cargo workers)

Simple "free" resources from any gas giant. Damages ship but gives fuel. Special ship and equipment to do this full time.

Costs per time, per time in transit, fuel use, repairs, few payment

task time is complicated (crew ready, reactor warmup, undocking clearance,distance to FTL safe zone, spool up, jump length, accuracy, dead zone after jump, docking clearance, contraband search, docking queue, unloading, crew minimum stay or shore leave).

Spending a little time each dock can save randomly using lots of time.

Fixed costs for changing sovrentry(vignette, security checks)

Combat simply most time and resources.

Simple choices: turn off reactor when landing or keep it hot so you can leave sooner?

unload cargo immediatly or wait scout the market?

Implement any features for other economy game ideas

Building/research?

Multiplayer - why if there is no interaction, player economies?

Different ship types

no direct interactions

Timers until tasks are complete

notify when task has completed, and if the planned next task has been interrupted.

Several minutes between close locations

several hours between different clusters of locations
