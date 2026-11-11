---
title: "Monster catching mini game ideas"
source: "Game Stuff/Monster catching mini game ideas"
modified: 2026-02-01
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Pocket Monster Games]]"]
concepts: ["Pocket Monster game", "Design: Match-3 Battle System"]
words: 361
summary: "Design for a monster-battle minigame played as a grid icon-dragging match-3 puzzle where move icons, tiredness and flee icons are driven by monster stats and training."
tags: ["area/game-idea", "project/pocket-monster-games", "type/design-doc"]
---

Goal

- A mini game that is easy to understand

- Both monsters stats effect the mini game

- Player can effect the opponents actions

Monster catching mini game ideas

Grid dragging Japanese game

- Icons represent each of the creatures attacks

- Player abilities and items appear as icons

- Negative effects are also icons

Each turn you have unlimited time to think but once you start dragging you only have 3 seconds to move.

All triples and more neighbouring trigger, regardless if you want , and regardless if they are bad. The amount affects the power.

Tiredness is also represented as icons but they cannot be removed.

A pair of icons represent the flee action. If they come together then your creature forces you to change out.

Training a move makes more of it's icon appear.

Training effects the spawn rate of new icons.

The starting state can also be modified via training.

Moves have as stats

- Icon

- Time per turn it can trigger

- Times per fight it can trigger

- Power function (number of icons as parameter)

- Icon effect on you

- Icon effect on opponent

Monsters have

- Stats (atk, def, HP)

- Starting icon numbers

- Icon respawn weights

Monsters in battle have

- Temporary stat change list

- List of matches made

- Icon queue

During a fight, icons can be pushed into your queue. These are spawned first. Excess icons are chosen using the weights.

Enemy ai can work by making random swaps. The wild non aggressive creatures start with many hesitate icons and spawn many flee icons. If you wait, the creature will generally flee. Wild aggressive monsters start with many attack icons but spawn hesitate and flee icons. These creatures will give up after a strong start. All wild creatures spawn flee icons, so battles can end at any time.

Intimidate: add flee icons to the enemy queue

Feint: add hesitate icons to the enemy queue

Outrun: add tiredness tokens to both queues

Graphics

- Monster idle

- Monster hit

- Monster defeated

- Monster flee

- Monster appear

- Monster attack

- Attack vfx

- Move icons
