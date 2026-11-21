---
title: "Miniatures VTT"
source: "Game Stuff/Miniatures VTT"
modified: 2026-05-19
type: design-doc
area: wargame
status: "designed"
projects: ["[[Other Wargames]]", "[[Stompy Robo & Battletech]]", "[[Kill Team & 40k Homebrew]]"]
concepts: ["Miniatures VTT", "Battletech homebrew", "Kill Team homebrew"]
words: 122
summary: "Requirements for a simple virtual tabletop for miniature wargames (Godot 3D or TypeScript canvas): no auth, movement pathing, army list tab, JSON-configurable stat columns for Kill Team and Battletech."
tags: ["area/wargame", "project/kill-team-40k-homebrew", "project/other-wargames", "project/stompy-robo-battletech", "type/design-doc"]
---

VTT

Make it 3D with GODOT. If that fails then its 2D with typescript/node/canvas

No authentication, everyone can move everything.

Game system settings json

- List of unit stat columns

- Cover percentages

Pathing when moving, with preview ghost showing to hit to all targets at that position.

Two types of movement, pathing along ground, or direct line (for jump)

Facing selection.

Max movement

Button for resetting movement

Army List Tab with stats for mechs, both player and enemy. Buttons for adding those mechs as tokens to the VTT.

Stat columns are customizable in a json file (so the VTT can be used for Kill Team and Battletech)

Things Im not going to do:

Different terrain speeds, you can calc this yourself.
