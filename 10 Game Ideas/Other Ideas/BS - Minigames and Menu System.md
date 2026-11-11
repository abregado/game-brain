---
title: "BS - Minigames and Menu System"
source: "Game Stuff/Game Ideas/BS - Minigames and Menu System"
modified: 2014-02-25
type: notes
area: other
status: "idea"
projects: []
concepts: ["Ingress Remake", "Design: Inventory System", "Train Carriage Swap Game", "Design: Game Template Menus", "Minigame Collection"]
words: 361
summary: "Dev checklist notes: Ingress remake idea, minigame ideas, inventory system spec, train-carriage game idea, and a game template checklist (splash, menus, pause, victory)."
tags: ["area/other", "type/notes"]
---

remake ingress portal linking game

- export lcations from ingress

- use same game mechanics

- turn based with muktiple teams

mini game ideas

- rotate rings to find combination

- lockpick game, listen for sounds

- rotate or slide squares to creat a path

- minimum moves to solve a simple dot to dot

- pause all moving rods in sequence, they only stay still for a limited time

inventory system

- slot limit

- type limit per slot

- quantity/size per slot

- ui display for filled and empty slots

- slot type with labels for name of container, cargo type and measurement unit (tank, liquid, litres)

&nbsp;

- item system

- item "size" from slot type

- item name list

&nbsp;

- function for adding an item, return true if t fits

- detect if an item is in an inventory

- adding and removing

analogies and game ideas

train carriages. choose which carriages to attach to the train to suit the cargo that is waiting. trains arrive with random carriges and you must swap them out for others. limit the changes, reward efficent play and put in s timelimit game.

Make a "new project" project

splash screen - binary gambit image, bsckgound image, sponsor/compo image, space to skip, default png names, single sound effect plays once

main menu - new game, sound and quit. background image, btton image, how to play link, music ramps up slowly. sound effects (off, quiet, normal, loud). buttons stored in an array for easy addition. Hover and click graphics.

How to play screen - imitation gamestate with the same inputs. fake enemies and powerups

OR

How to play screen - overlay with glowing areas of information. Info provided on mouseover. gamestate paused. uses actual current gamestate.

pause menu - grey out, texture overlay, game name/compo/company images, button image. escape and pause key to resume. also a click buton to resume. sound controls and shorthand key reference. button to quit

gamestate with pause button, empty game loop (sample movement render). sample sound/music. camera pre-setup

victory screen. background image, retry, share, email, comment, quit button.

localization settings. score and sendback data on user request
