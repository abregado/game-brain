---
title: "Stompy Robo Jr Mechs"
source: "Game Stuff/Stompy Robo Jr Mechs"
modified: 2026-05-05
type: design-doc
area: wargame
status: "designed"
projects: ["[[Stompy Robo & Battletech]]"]
concepts: ["Stompy Robo"]
words: 1011
summary: "Mech roster for Stompy Robo Jr with company, movement, TMM, armor, structure, damage, specials and cost calculations."
tags: ["area/wargame", "project/stompy-robo-battletech", "type/design-doc"]
---

## Sheet: Sheet1

| Company |  | Name | MV | TMM | Arm | Str | Short | Long | Specials | Cats | Base Cost |  |  | Modified Cost |  | Simple Cost | TMM Mod | 0.4 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Harken | DGO-14 | Dingo | 18 | 3.0 | 1.0 | 3.0 | 2.0 | 1.0 | 3.0 | 0.0 | 13.5 | 0 | 0 | 24.3 |  | 2.0 |  |  |
| Harken | JKL-09 | Jackal | 18 | 3.0 | 2.0 | 2.0 | 3.0 | 0.0 | 3.0 | 0.0 | 13.5 | 0 | 0 | 24.3 |  | 2.0 |  |  |
| Orvec | WRA-03 | Wraith | 18 | 3.0 | 1.0 | 2.0 | 1.0 | 2.0 | 3.0 | 0.0 | 13.5 | 0 | 0 | 24.3 |  | 2.0 |  |  |
| Volker-Straus | BRN-07 | Bruin | 12 | 2.0 | 3.0 | 7.0 | 2.0 | 3.0 | 2.0 | 0.0 | 24 | 0 | 0 | 33.6 | 9.3 | 3.0 |  |  |
| Cerulean | RGR-20 | Ranger | 12 | 2.0 | 5.0 | 3.0 | 4.0 | 2.0 | 2.0 | 0.0 | 24 | 0 | 0 | 33.6 |  | 3.0 |  |  |
| Cerulean | CON-31 | Conductor | 12 | 2.0 | 4.0 | 5.0 | 0.0 | 4.0 | 2.0 | 0.0 | 24 | 0 | 0 | 33.6 |  | 3.0 |  |  |
| Volker-Straus | SGE-19 | Siege | 6 | 1.0 | 7.0 | 10.0 | 7.0 | 5.0 | 2.0 | 0.0 | 45 | 2 | 0 | 45 | 11.4 | 4.0 |  |  |
| Orvec | PYR-11 | Pyre | 6 | 1.0 | 9.0 | 6.0 | 8.0 | 4.0 | 2.0 | 0.0 | 45 | 3 | 0 | 45 |  | 4.0 |  |  |
| Harken | WAR-40 | Warden | 6 | 1.0 | 8.0 | 8.0 | 5.0 | 6.0 | 2.0 | 0.0 | 45 | 0 | 1 | 45 |  | 4.0 |  |  |
| Orvec | SNT-47-A | Sentinel | 6.0 | 1.0 | 2.0 | 5.0 | 1.0 | 1.0 | 1.0 |  | 13.5 | 0 | 0 | 13.5 |  | 2.0 |  |  |
| Orvec | SNT-47-B | Sentinel | 6.0 | 1.0 | 5.0 | 6.0 | 2.0 | 2.0 | 2.0 |  | 24 | 0 | 0 | 24 |  | 2.0 |  |  |
| Harken | TPD-22 | Trapdoor | 18.0 | 3.0 | 1.0 | 1.0 | 6.0 | 0.0 | 1.0 |  | 13.5 | 1 | 0 | 24.3 |  | 2.0 |  |  |
| Harken | KTE-14 | Kite | 18.0 | 3.0 | 1.0 | 1.0 | 1.0 | 3.0 | 1.0 |  | 13.5 | 0 | 0 | 24.3 |  | 2.0 |  |  |
| Eidolon | TGS-87 | Tigris | 24.0 | 4.0 | 2.0 | 1.0 | 6.0 | 4.0 | 7.0 |  | 27.5 | 1 | 0 | 60.5 | 0.1 | 5.0 |  |  |
| Eidolon | VGD-34 | Vanguard | 16.0 | 3.0 | 5.0 | 3.0 | 5.0 | 5.0 | 6.0 |  | 33.66666667 | 0 | 0 | 60.6 |  | 5.0 |  |  |
| Eidolon | HER-89 | Herzog | 8.0 | 2.0 | 8.0 | 4.0 | 6.0 | 6.0 | 2.0 |  | 43.33333333 | 1 | 1 | 60.66666667 | 0.06666666667 | 5.0 |  |  |

## Sheet: static

| Company |  | Name | MV | TMM | Arm | Str | Short | Long | Specials | Simple Cost |
|---|---|---|---|---|---|---|---|---|---|---|
| Harken | DGO-14 | Dingo | 18.0 | 3.0 | 1.0 | 3.0 | 2.0 | 1.0 | 3.0 | 2.0 |
| Harken | JKL-09 | Jackal | 18.0 | 3.0 | 2.0 | 2.0 | 3.0 | 0.0 | 3.0 | 2.0 |
| Orvec | WRA-03 | Wraith | 18.0 | 3.0 | 1.0 | 2.0 | 1.0 | 2.0 | 3.0 | 2.0 |
| Volker-Straus | BRN-07 | Bruin | 12.0 | 2.0 | 3.0 | 7.0 | 2.0 | 3.0 | 2.0 | 3.0 |
| Cerulean | RGR-20 | Ranger | 12.0 | 2.0 | 5.0 | 3.0 | 4.0 | 2.0 | 2.0 | 3.0 |
| Cerulean | CON-31 | Conductor | 12.0 | 2.0 | 4.0 | 5.0 | 0.0 | 4.0 | 2.0 | 3.0 |
| Volker-Straus | SGE-19 | Siege | 6.0 | 1.0 | 7.0 | 10.0 | 7.0 | 5.0 | 2.0 | 4.0 |
| Orvec | PYR-11 | Pyre | 6.0 | 1.0 | 9.0 | 6.0 | 8.0 | 4.0 | 2.0 | 4.0 |
| Harken | WAR-40 | Warden | 6.0 | 1.0 | 8.0 | 8.0 | 5.0 | 6.0 | 2.0 | 4.0 |
| Orvec | SNT-47-A | Sentinel | 6.0 | 1.0 | 2.0 | 5.0 | 1.0 | 1.0 | 1.0 | 2.0 |
| Orvec | SNT-47-B | Sentinel | 6.0 | 1.0 | 5.0 | 6.0 | 2.0 | 2.0 | 2.0 | 2.0 |
| Harken | TPD-22 | Trapdoor | 18.0 | 3.0 | 1.0 | 1.0 | 6.0 | 0.0 | 1.0 | 2.0 |
| Harken | KTE-14 | Kite | 18.0 | 3.0 | 1.0 | 1.0 | 1.0 | 3.0 | 1.0 | 2.0 |
| Eidolon | TGS-87 | Tigris | 24.0 | 4.0 | 2.0 | 1.0 | 6.0 | 4.0 | 7.0 | 5.0 |
| Eidolon | VGD-34 | Vanguard | 16.0 | 3.0 | 5.0 | 3.0 | 5.0 | 5.0 | 6.0 | 5.0 |
| Eidolon | HER-89 | Herzog | 8.0 | 2.0 | 8.0 | 4.0 | 6.0 | 6.0 | 2.0 | 5.0 |
