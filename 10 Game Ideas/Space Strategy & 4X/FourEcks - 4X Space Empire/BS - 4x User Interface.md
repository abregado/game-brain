---
title: "BS - 4x User Interface"
source: "Game Stuff/Game Ideas/BS - 4x User Interface"
modified: 2021-06-22
type: design-doc
area: design-theory
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["4X Decoupled UI", "Design: Interface and Micromanagement", "FourEcks / 4X Space Empire"]
words: 471
summary: "Concept to decouple 4X UI from the simulation, listing problems and options such as clout points, reorganization timers, change queues and automation."
tags: ["area/design-theory", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

### Concept

**Idea:** Decouple the user interface from the simulation, both in programming and design.

**Goal:**

1.  Reduce micromanagement by reducing the number of possible interactions per real world time unit.

2.  Make the simulation truly independent from player action timing (benefits multiplayer syncing)

3.  Promote players in a multiplayer “realtime with pause” game having the game paused as little as possible.

4.  Solidify the “choice meta”

Decoupling interface and simulation in the code is easy. But there are a number of issues with doing it in the game design.

**Problem 1: Delayed Player Feedback**

The player makes a settings change, and cant see the effect immediately, or they can see the effect immediately but it does not represent the actual state of the game.

**Problem 2: Complexity of UI Design increases**

How to deal with change confirmation? How to show that something has been changed? How to reset back to the previous state? UI like this has no examples to work from (in the games branch).

**Problem 3: Nebulous time costs leads to greater player cognitive load**

A player now needs to weigh up the opportunity cost of making a change, and in the worst case, the order of the changes they want. Perhaps this actually leads to MORE micromanagement and meta.

### Options

**Clout points**

Every change you make to your empire's setup costs a special resource. As you make changes, these costs are tallied, and when you Save the settings, the total is paid. This way the player can make several changes back and forth without changing anything, while waiting for enough resources to build up. Sets of changes that are dependent on one another can also be actualized on the same tick.

**System reorganization timers**

You can change any number of settings in a system, but once you commit those changes, you cannot make any other changes for a fixed number of ticks. Each \[system/planet/management unit\] has its own timer.

This may also create an interesting game loop of iterating over each management unit. Players will also want to provide enough queued orders to last until the reorg timer is complete, otherwise the system wastes time being idle.

**Change Queues**

Whenever the player makes a change to something, the change is actually added to a queue. This queue is then completed in (unpaused) game time, rather than instantly.

This means that a player of a real-time with pause game can only use the paused time for thinking and strategizing, not actually micromanaging. In a multiplayer game, this could also encourage players to spend as little time as possible paused.

**Automate the little stuff**

The player only controls the large direction of the game, and simply cannot make tiny changes. These parts which normally would be in the UI are moved to the simulation and are not exposed.
