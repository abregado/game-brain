---
title: "BS - 4x generic ethics"
source: "Game Stuff/Game Ideas/BS - 4x generic ethics"
modified: 2022-03-09
type: design-doc
area: game-idea
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["4X Generic Ethics System", "FourEcks / 4X Space Empire"]
words: 229
summary: "Three attempts at a self-contained 4X population ethics system with percentage tags, opposites and a method API."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

**Goal:** Population ethics as an easily expandable, self contained system that can be effected and read by other systems.

**Attempt 1: Track individual pops ethics.**

Every population unit has its own ethics. Moving them around affects the aggregate ethics blend.

Downsides:

- Lots of calculations.

- Promotes micromanagement.

**Attempt 2: Track only Planetary population Ethics as string tag, percentage pairs.**

Each planet tracks its own ethics. Ethics are identified with a string index, and each has a percentage of the local population who have this trait. Moving population to or from a group causes proportional mixing. Solves the issues of Attempt 1.

New Downsides:

- No ethical/demographic polarisation

**Attempt 3: Ethics have “opposites”**

Each ethic/demographic trait also has a list of other indexes. Whenever the trait percentage moves in a direction, the other traits on this list move in the opposite direction.

New Downsides

- Ethic setup is a little more complex

How can this system be used?

Methods

- MovePopulation(amount, popBodyFrom, popBodyTo)

- AddTrend(traitString, trendMagnitude)

- AddTimedTrend(traitString, trendMagnitude, timePeriod)

- GetPercentage(traitString)

- ProcessTrends()

Buildings can add a trend when they are constructed, and remove it when they are demolished. For example: A prison camp might add an Insecurity trait trend. An alien circus might add the Xenophile trait trend for a period of time after it happens.

Events can also read the current demographics by polling the system.
