---
title: "Rampart Balance Math"
source: "Game Stuff/Game Ideas/Rampart Balance Math"
modified: 2013-06-12
type: reference-data
area: game-idea
status: "prototyped"
projects: ["[[Xenosurge]]", "[[Tower Defense]]"]
concepts: ["Rampart-like Defence Game", "Tower Defense"]
words: 547
summary: "Spreadsheet balancing a Rampart-like tower/turret defence game: turret cooldowns, missiles fired, damage and enemy HP per phase, plus difficulty-level stats."
tags: ["area/game-idea", "project/tower-defense", "project/xenosurge", "type/reference-data"]
---

## Sheet: Sheet1

| turret cooldown | 3.5 |  | player build per second | 0.7 |  |  |  |  |
|---|---|---|---|---|---|---|---|---|
| combat phase time | 15.0 |  | build phase time | 20.0 | 14 |  |  |  |
| player accuracy | 0.33 |  | nodes on map |  |  |  |  |  |
| phase | turrets placed | Total Turrets | Missiles Fired | Damage Inflicted | New HP of enemies | Total enemies HP remain  | Lazers fired this round |  |
| 0.0 | 2.0 | 2 | 8.571428571 | 2.828571429 | 10.0 | 7.171428571 | 1.792857143 |  |
| 1.0 | 1.0 | 3 | 12.85714286 | 4.242857143 | 9.0 | 11.92857143 | 8.085714286 |  |
| 2.0 | 1.0 | 4 | 17.14285714 | 5.657142857 | 9.0 | 15.27142857 | 10.46428571 |  |
| 3.0 | 1.0 | 5 | 21.42857143 | 7.071428571 | 10.0 | 18.2 | 12.63571429 |  |
| 4.0 | 1.0 | 6 | 25.71428571 | 8.485714286 | 13.0 | 22.71428571 | 15.6 |  |
| 5.0 | 1.0 | 7 | 30 | 9.9 | 17.0 | 29.81428571 | 19.85714286 |  |
| 6.0 | 1.0 | 8 | 34.28571429 | 11.31428571 | 20.0 | 38.5 | 24.90714286 |  |
| phase | turrets placed | Total Turrets | Missiles Fired | Damage Inflicted | New HP of enemies | Total enemies HP remain  | Lazers fired this round |  |
| 0.0 | 3.0 | 3 | 12.85714286 | 4.242857143 | 10.0 | 5.757142857 | 1.439285714 | 4 normal |
| 1.0 | 1.0 | 4 | 17.14285714 | 5.657142857 | 7.0 | 7.1 | 6.378571429 | one troop one normal |
| 2.0 | 1.0 | 5 | 21.42857143 | 7.071428571 | 8.0 | 8.028571429 | 7.55 | one fire one normal |
| 3.0 | 1.0 | 6 | 25.71428571 | 8.485714286 | 8.0 | 7.542857143 | 8.014285714 | one corsair one troop |
| 4.0 | 1.0 | 7 | 30 | 9.9 | 11.0 | 8.642857143 | 9.271428571 | one troop one corsair |
| 5.0 | 1.0 | 8 | 34.28571429 | 11.31428571 | 13.0 | 10.32857143 | 10.82142857 | one fire one corsair 2 normal |
| 6.0 | 1.0 | 9 | 38.57142857 | 12.72857143 | 14.0 | 11.6 | 12.16428571 | two fire 2 normal |
| Level | Beginner | Hard | Proguy |  |  |  |  |  |
| missiles | 59.0 | 84.0 | 116.0 |  |  |  |  |  |
| damage | 47.0 | 76.0 | 94.0 |  |  |  |  |  |
| eff | 79.0 | 90.0 | 81.0 |  |  |  |  |  |
| ships | 18.0 | 27.0 | 29.0 |  |  |  |  |  |
| inf | 8.0 | 15.0 | 21.0 |  |  |  |  |  |
| blocks | 59.0 | 103.0 | 92.0 |  |  |  |  |  |
| destroyed | 24.0 | 70.0 | 58.0 |  |  |  |  |  |
| nodeturns | 19.0 | 22.0 | 30.0 |  |  |  |  |  |
| turrets | 6.0 | 7.0 | 8.0 |  |  |  |  |  |

## Sheet: Sheet2

_(empty)_

## Sheet: Sheet3

_(empty)_
