---
title: "Claude ideas"
source: "Game Stuff/Claude ideas"
modified: 2026-04-08
type: brainstorm
area: game-idea
status: "idea"
projects: ["[[Diablo-like Action Shooter]]", "[[Non-Game Projects]]", "[[D&D Homebrew]]"]
concepts: ["Diablo-like action shooter", "Discord bots", "D&D tools and generators", "Utility apps"]
words: 361
summary: "Brainstorm of app/bot ideas for Discord and utilities, plus a detailed design for a Diablo-like action shooter character controller (weapon stats, fire modes, dodge roll rules, controls)."
tags: ["area/game-idea", "project/d-d-homebrew", "project/diablo-like-action-shooter", "project/non-game-projects", "type/brainstorm"]
---

Claude ideas

Discord bot that asks a question every week

Discord bot that applies a role based on user questions

Discord bot that does chat roulette

Discord bot that records attendance during an online event

Finger choosing app

Deck app

Dice roller

Splitwise replacement with touch

Todo calendar sync

DnD Tools and generators

Rulebook summary

Force sheet creator

Mech search

Diablo firearm action controller idea

Action combat diablo-like character controller.

Weapon stats

- Speed decrease (weight)

- Dodge recovery time

Weapon fire mode stats

- Fire rate

- Accuracy best (degrees)

- Accuracy worst (degrees)

- Tracking speed (to new target)

- Setup time after roll

- Speed decrease while firing

Contextual change between firemodes based on movement vector relative to aiming vector.

- Standing still increases fire rate or accuracy (based on weapon)

- When moving backward relative, increase fire rate but decrease accuracy (enemies are probably closing in)

- When moving forward, decrease accuracy but increase tracking time

- When moving

Dodge rolling disables your weapon for a length of time. Smaller weapons recover faster than heavy weapons. Switching weapons also disables your weapon for the same length.

Weapons have one fire mode per hand they take. A third Focus based firemode becomes available based on weapon combination

Dodge rolling is NOT faster than walking. It gives i-frames and has a recovery time afterwards where walking speed is reduced and dodge is disabled. Weapon fire modes have a cooldown after rolling, based on the mode, not the weapon.

Equipment Slot is either a triggerable effect, or an auto-trigger (on hit, on roll, ect). Maybe better that it is always an auto-trigger? Or it replaces the third shooting button, in the case your weapon does not have one (or you don’t want one).

Suit ability, if it has one, replaces Dodge and is always a movement effect.

Controls

Left and Right Triggers - Primary and Secondary fire

A - dodge in direction of movement (or looking if shading still)

Left stick - move

Right stick - look/aim

Once trigger depressed, stay locked to target, when target dies, reacquire based on stick, or auto target closest if in deadzone.

Primary fire
