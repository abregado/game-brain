---
title: "BS - Ui bridge game"
source: "Game Stuff/Game Ideas/BS - Ui bridge game"
modified: 2026-10-27
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Elite-like Space Flight & Trading]]"]
concepts: ["Bridge Simulator", "Design: Shield Frequency and Scanning"]
words: 362
summary: "Design notes for a bridge-simulator style space combat game: shield frequencies, scanning, weapons targeting meshes, armor, damage control, flight rules."
tags: ["area/game-idea", "project/elite-like-space-flight-trading", "type/design-doc"]
---

Components provide stats and widgets

Shields need a target and track that target at a radians per second rate.

Point defense is simple, until it isn't and requires it's own station

Combat is slower, more about finding weak spots than just reducing hit points

Over the course of a fight, more information becomes available

Better sci scanning play gets data faster

A fighter is a main screen with two-three world space screens, maybe a phone.

Hull size determines what kind of control is necessary

Fighters are fast enough to avoid the larger missiles, buffet ships need to rely on shield and point defense

Recovering from combat takes time and good play to speed up.

Flight involves setting rules for distances from various targets. Use a weighted function system.

Larger weapons require pre setting targets positions on a mesh of the target and then getting a matching angle on it. Multiple target positions can be set per target. Whether a weapon will fire at a target ship is a Boolean per target ship.

Changing shield frequency requires halting recharge. Scans show a band that the frequency might be. Scanning play can narrow it faster.

Weapons automatically change frequency over time to match active targets, but every target will have a different frequency.

Penetration power and range can all be modified in a triangle. Power effects everything. Higher penetration means the distance from the shield frequency that will ignore it.

Armor is damage reduction, but it's ablative. It can't be repaired and takes damage slowly.

Specific parts have less armor but can't be targeted until scans have narrowed down a firing solution. Also the angle of attack has to be more precise to fire.

Flight shows the expected path based on current rules and information.

Smaller ships have more turning speed.

Smaller engineering does not allow fine turning, instead swapping between a small number of presets. Maybe those can be changed when in dock.

Internal shielding cam be set up on some systems, if you know what they are shooting at.

Damage control crews set to repair or reinforce

Weapons and scanners as two separate resources. You can't just exchange one for the other
