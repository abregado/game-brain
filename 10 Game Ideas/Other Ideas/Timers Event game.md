---
title: "Timers Event game"
source: "Game Stuff/Game Ideas/Timers Event game"
modified: 2013-06-22
type: design-doc
area: game-idea
status: "idea"
projects: []
concepts: ["Timers Event Game", "Design: Inventory Systems"]
words: 210
summary: "Technical outline of a UI-driven game with timers, commodities, items, actions and inventory class."
tags: ["area/game-idea", "type/design-doc"]
---

Screen made up of 4 elements

Timers:

These have the following properties:

- Title

- hover text

- icon

- min/max activation time

- min/max available time

- action on click

Timers count down until their activation time is finished, then they start counting down their available time. If clicked on before their available time is finished they activate the action that is linked to them. If their available time runs out they start counting down their activation timer again.

Commodities

These have the following properties:

- quantity

- hover text

- name

- icon

Commodities have no properties and are displayed in a grid inventory. Their name and hover text is only shown when the player hovers over them. Their icon and quantity are shown at all times

Items

These have the following properties

- name

- hover text

- action list (buttons for each)

- image

Items have actions which can be triggered with buttons directly on the item. Items often have unique properties

Actions

These give and take commodities and are stored in a static class.

Inventory Class

Properties:

- total slots

- item capacity

- width of display

- location of display

- items held array

These contain commodities and the functions related to modifying quantities.
