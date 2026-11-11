---
title: "RTS Movement mods"
source: "Game Stuff/RTS Movement mods"
modified: 2023-06-11
type: reference-data
area: design-theory
status: "unknown"
projects: ["[[RTS Ideas]]"]
concepts: ["Design: RTS Movement Types"]
words: 155
summary: "Small table of RTS movement classes (tank, rover, bot, spider, flying) versus terrain walls and slope thresholds."
tags: ["area/design-theory", "project/rts-ideas", "type/reference-data"]
---

## Sheet: Sheet1

|  | flat | wall |  |  |  |
|---|---|---|---|---|---|
| ground | x |  |  |  |  |
| flying | x | x |  |  |  |
|  |  | 10.0 | 15.0 | 25.0 | 80.0 |
| tank | 12.0 | x |  |  |  |
| rover | 22.0 | x | x |  |  |
| bot | 27.0 | x | x | x |  |
| spider | 90.0 | x | x | x | x |
| flying | x | x | x | x | x |
|  | flat | slope < 30 | 80.0 |  |  |
| tank | x | 0.5 |  |  |  |
| rover | x | 0.7 |  |  |  |
| bot | x | 1.0 |  |  |  |
| spider | x | x | x |  |  |
