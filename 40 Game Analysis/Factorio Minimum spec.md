---
title: "Factorio Minimum spec"
source: "Game Stuff/Factorio Minimum spec"
modified: 2015-08-16
type: reference-data
area: analysis
status: "unknown"
projects: ["[[Factorio mods & ideas]]"]
concepts: ["Factorio mods / ideas", "Analysis: Factorio"]
words: 545
summary: "Spreadsheet calculating the minimum production chain ratios (green science, belts, cogs, inserters, circuits, plates) for Factorio."
tags: ["area/analysis", "project/factorio-mods-ideas", "type/reference-data"]
---

## Sheet: Sheet1

| Item | Quant | Time | Modifier | Seconds | Needs |  |  |  |  |  |  |  |  |  | Actual |  |  |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|  |  |  |  |  | GSP | TB | Cog | Ins | EC | CW | IP | CP | IO | CO | GSP | TB | Cog | Ins | EC | CW | IP | CP | IO | CO |  |
| Green Science Pack | 12.0 | 6.0 | 0.75 | 8 | 1.0 | -1.0 |  | -1.0 |  |  |  |  |  |  | 1.5 | -1.5 | 0 | -1.5 | 0 | 0 | 0 | 0 | 0 | 0 |  |
| Transport Belt | 2.0 | 0.5 | 0.5 | 1 |  | 1.0 | -1.0 |  |  |  | -1.0 |  |  |  | 0 | 2 | -2 | 0 | 0 | 0 | -2 | 0 | 0 | 0 |  |
| Cog | 2.0 | 0.5 | 0.5 | 1 |  |  | 1.0 |  |  |  | -2.0 |  |  |  | 0 | 0 | 2 | 0 | 0 | 0 | -4 | 0 | 0 | 0 |  |
| Inserter | 2.0 | 0.5 | 0.75 | 0.6666666667 |  |  | -1.0 | 1.0 | -1.0 |  | -1.0 |  |  |  | 0 | 0 | -3 | 3 | -3 | 0 | -3 | 0 | 0 | 0 |  |
| Electronic Circuit | 3.0 | 0.5 | 0.5 | 1 |  |  |  |  | 1.0 | -3.0 | -1.0 |  |  |  | 0 | 0 | 0 | 0 | 3 | -9 | -3 | 0 | 0 | 0 |  |
| Copper Wire | 5.0 | 0.5 | 0.5 | 1 |  |  |  |  |  | 2.0 |  | -1.0 |  |  | 0 | 0 | 0 | 0 | 0 | 10 | 0 | -5 | 0 | 0 |  |
| Iron Plate | 70.0 | 3.5 | 1.0 | 3.5 |  |  |  |  |  |  | 1.0 |  | -1.0 |  | 0 | 0 | 0 | 0 | 0 | 0 | 20 | 0 | -20 | 0 |  |
| Copper Plate | 20.0 | 3.5 | 1.0 | 3.5 |  |  |  |  |  |  |  | 1.0 |  | -1.0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 5.714285714 | 0 | -5.714285714 |  |
|  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | 1.5 | 0.5 | -3 | 1.5 | 0 | 1 | 8 | 0.7142857143 | -20 | -5.714285714 | Consump |
| 10x Iron |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| 3x Copper |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
