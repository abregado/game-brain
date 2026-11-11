---
title: "Mech pricing reverse engineering"
source: "Game Stuff/Mech pricing reverse engineering"
modified: 2026-03-15
type: analysis
area: wargame
status: "idea"
projects: ["[[Stompy Robo & Battletech]]"]
concepts: ["Battletech homebrew", "Design: Point Costing Formula"]
words: 51
summary: "Short notes on a formula to reverse-engineer Alpha Strike point values from movement, TMM, defence and offence stats."
tags: ["area/wargame", "project/stompy-robo-battletech", "type/analysis"]
---

Mech pricing reverse engineering

TMM

0 = 2-4

1 = 6-8

2 = 10-12

3 = 14-18

4 = 20+

1+(TMM\*0.1) = DIR Mod

Move Score = MV/8 + (0.5 if Jump)

Def Score = Armor\*2 + Structure

Off Score = S + M\*2 + L + OV

(Def\*DIRMod)+Move+Off = Total
