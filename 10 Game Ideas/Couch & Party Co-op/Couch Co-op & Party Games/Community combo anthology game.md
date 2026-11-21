---
title: "Community combo anthology game"
source: "Game Stuff/Community combo anthology game"
modified: 2023-03-28
type: design-doc
area: jam
status: "designed"
projects: ["[[Couch Co-op & Party Games]]"]
concepts: ["Community Combo Anthology Game"]
words: 165
summary: "Design constraints for a community anthology game combining small submodule games by different devs: menu, shared systems, rules for submissions."
tags: ["area/jam", "project/couch-co-op-party-games", "type/design-doc"]
---

Community combo game

Design Constraints

- Submodule template repo?

  - Keep between scene Prefab

- Devs should completely control their own submodule project

UI

- Main Menu

  - Level select

    - Game details

  - Play from start

  - Play random

  - Settings

  - Dev list

  - Discord link

- Audio Settings (on/off/half)

- Back to menu

- Game Finished

  - Dev details and links

  - Restart this game

  - Return to menu

  - Next game in list

Shared things

- Audiosource checker

  - On scene start halves or sets to zero volumes.

- DontDestroyOnLoad object with

  - UIView for quit/game over.

  - Saves which games have been played, completed

- Control scheme

  - Rewired?

  - Directions

  - 2 Buttons

Rules

- Namespaces

- Single "keep between scene" object

- Foldername==Scenename

- Text file with specific formatting

  - Game name

  - Scenename

  - Dev name

  - Social link 1-3

  - Discord username

  - Thumbnail

- No additional don't destroy on load objects.

- No nsfw content
