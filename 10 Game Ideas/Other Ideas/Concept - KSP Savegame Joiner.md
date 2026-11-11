---
title: "Concept - KSP Savegame Joiner"
source: "Game Stuff/Game Ideas/Concept_ KSP Savegame Joiner"
modified: 2017-10-13
type: design-doc
area: other
status: "designed"
projects: []
concepts: ["KSP Savegame Joiner"]
words: 450
summary: "Spec for a script/mod that synchronises two singleplayer KSP saves monthly, with merge rules, edge cases and mod UI features."
tags: ["area/other", "type/design-doc"]
---

Situation:

Two people are playing KSP in singleplayer. Every 30 in game days, the game is saves and both saves are synchronized so that ships from eachothers fleets show up in echothers game. The game prompts the player every 30 days to wait for others who have stopped at the same date.

Aim:

Write a merger script which adds ships in flight to both games, updates Kerbal status, but does not merge ongoing contracts.

Items to be merged:

- Craft in Flight

- Assigned Kerbals

- Completed contracts

Not to be merged:

- Craft designs

- Tech tree

- Science, Money, Reputation

- Building Upgrades

- Active Contracts

- Unassigned Kerbals

Edge Cases

- A ship which was there on both saves last sync is missing from one save:

  - Reasons: One player crashed or recovered the ship

  - Action: Remove the ship from both saves

- A ship which appears new on both saves

  - Reasons: Both players launched a ship named the same thing

  - Action: Add both but modify the name of one

- A ship which was on one of the last saves is still in both, but they are different

  - Reason: One player added to or removed items from a ship, or moved the orbit of a ship.

  - Action: If one is the same as the last save, take the one that is different and apply to both. If neither are the same as the last save, take the craft with the greater part count and replace it on both. Sync Kerbals from both, as they may have changed.

- A Kerbal is MIA or KIA in one game

  - Action: Make that Kerbal MIA or KIA in both games

- There are two Kerbals with the same name who are active in different games.

  - Reason: The random name generator was being generous

  - Action: Rename one of the Kerbals to Mr Kerbin II and update in both games.

- A ship has a \[\*\] in the name

  - Reason: This is a private craft,

  - Action: Dont update this across to other saves

Mod Features

- Set an alarm in Kerbal Alarm Clock

- Pause the game and give a pop up when the month is finished

  - Option to email partners to join in or finish their month

  - Option to send your save up to the server

  - A light to show which other players have uploaded their saves

  - A button to download the new save

  - Option to continue another month with the current synced players.

- Loading a game which has reached the end of the month will pause it and show the main mod gui.
