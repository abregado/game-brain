---
title: "Untitled 4X"
source: "Game Stuff/Game Ideas/Untitled 4X"
modified: 2020-10-15
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["FourEcks / 4X Space Empire", "Design: Pop and Job Systems"]
words: 1119
summary: "Spreadsheet data model for a 4X colony system: districts, jobs, species bonuses, resources, metropolitan buildings, stability/crime derived values."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

## Sheet: Colony

| Derived values |  |  |  |  |  |  |  |  |
|---|---|---|---|---|---|---|---|---|
| Population list | Species, Job pairs, approval rating |  |  |  |  |  |  |  |
| Training Rate | How often a pop will be moved to a higher priority job. |  |  |  |  |  |  |  |
| Local Storage | Resources stored here |  |  |  |  |  |  |  |
| Approval Rating | Simularity to Governing Ethics |  |  |  |  |  |  |  |
| Stability | Value / Threshold for event |  |  |  |  |  |  |  |
| Crime | Value / Threshold for event |  |  |  |  |  |  |  |
| Chance for Stability Event |  |  |  |  |  |  |  |  |
| Chance for Crime Event |  |  |  |  |  |  |  |  |
| Growth Rate | Days until new pop |  |  |  |  |  |  |  |
| Resource output modifier | Derived from Stability |  |  |  |  |  |  |  |
| Em/Immigration rate | Positive for Immigration |  |  |  |  |  |  |  |
| Variables |  |  |  |  |  |  |  |  |
| Job List |  |  |  |  |  |  |  |  |
| Import allowance List | Which resources are allowed to be imported |  |  |  |  |  |  |  |
| Export allowance List | Which resources are allowed to be exported |  |  |  |  |  |  |  |
| Local Storage caps | Minimum and Max values for each resource |  |  |  |  |  |  |  |
| District List |  |  |  |  | Jobs |  |  |  |
| Name | Current | Maximum | Housing | Building Slot | Technician | Farmer | Miner | Researcher |
| Homeworld Sprawl | 2.0 |  | 20 | 6 | 0 | 0 | 0 | 0 |
| Agricultural | 5.0 |  | 10 | 0 | 0 | 10 | 0 | 0 |
| Energy | 5.0 |  | 10 | 0 | 10 | 0 | 0 | 0 |
| Metropolitan | 1.0 |  | 4 | 1 | 0 | 0 | 0 | 0 |
| None |  |  | 0 | 0 | 0 | 0 | 0 | 0 |
|  |  |  | 44 | 7 | 10 | 10 | 0 | 0 |
| Building List |  |  |  |  |  |  |  |  |

## Sheet: Resources

| Name |  |
|---|---|
| Service | Consumed by Population. Excess converted into Integration Speed |
| Minerals |  |
| Energy |  |
| Food |  |
| Consumer Goods | Consumed by Specialist population |
| Alloy | Military grade metals. Made from Minerals |

## Sheet: Planet

| Max Zones/Districts |
|---|
| Agricultural |
| Energy |
| Mining |
| Cities |
| Size (Max all) |

## Sheet: Species

| Species Name | Job Bonus name | Job Bonus modifier | Job Bonus fixed |
|---|---|---|---|
| Bigguy | Miner | 1.1 |  |
| Bigguy | Researcher | 0.9 |  |

## Sheet: ZoneDistrict Types

| District Name | Housing | Building Slot | Technician | Farmer | Miner | Researcher |
|---|---|---|---|---|---|---|
| Agricultural | 2.0 | 0.0 | 0.0 | 2.0 | 0.0 | 0.0 |
| Energy | 2.0 | 0.0 | 2.0 | 0.0 | 0.0 | 0.0 |
| Mining | 2.0 | 0.0 | 0.0 | 0.0 | 2.0 | 0.0 |
| Metropolitan | 4.0 | 1.0 | 0.0 | 0.0 | 0.0 | 0.0 |
| Archeological | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 5.0 |
| Homeworld Sprawl | 10.0 | 3.0 | 0.0 | 0.0 | 0.0 | 0.0 |
| None | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |

## Sheet: Metropolitan Buildings

| Building Name | Effect | Requirement | Energy Upkeep | Max district Bonus | Agriculture Bonus | Energy Bonus | Mining Bonus | Metropolitan Bonus |
|---|---|---|---|---|---|---|---|---|
| Populated Outpost | Max built districts +2, -50% offworld shipping costs. |  |  |  |  |  |  |  |
| Colony Administration | Max built districts +5, City Districts give +1 housing. Districts +1 job. | 10 pops |  |  |  |  |  |  |
| Contenental Capital | Max built districts +15, City Districts give +2 housing, Districts +2 jobs | 20 pops |  |  |  |  |  |  |
| Planetary Capital | Max built districts +25, City Districts give +4 housing, Districts +3 jobs. |  |  |  |  |  |  |  |
| Storage facility | Resource storage +300 |  |  |  |  |  |  |  |
| Science Facility | 2 Researcher jobs |  |  |  |  |  |  |  |
| Foundry | 2 Metalurgist jobs |  |  |  |  |  |  |  |
| Factory | 2 Artisan Jobs |  |  |  |  |  |  |  |
| Theatre | 2 Entertainer Jobs |  |  |  |  |  |  |  |
| Precinct | 2 Enforcer Jobs |  |  |  |  |  |  |  |
| Education facility | 2 Teacher jobs |  |  |  |  |  |  |  |
| Office | 2 Bureaucrat jobs |  |  |  |  |  |  |  |
| Military base | 2 Soldier jobs |  |  |  |  |  |  |  |
| Amenities | 2 Clerk Jobs |  |  |  |  |  |  |  |
| Power grid | Energy districts +1 jobs | Colony Administration |  |  |  |  |  |  |
| Starport | -50% offworld shipping costs | Colony Administration |  |  |  |  |  |  |
| Mining company | Mining districts +1 jobs | Colony Administration |  |  |  |  |  |  |
| Packing Plant | Farming districts +1 jobs | Colony Administration |  |  |  |  |  |  |
| Space Agency | Max space districts +1 | Colony Administration |  |  |  |  |  |  |

## Sheet: Citizens

| CitizenID | ColonyID | Job |
|---|---|---|
| 1.0 | 1.0 | 1.0 |

## Sheet: Job Types

| JobID | Job name | Job Type | Resource added | Amount | Resource cost | Amount | Species Priority | Special |
|---|---|---|---|---|---|---|---|---|
| 1.0 | Farmer | Worker | Food |  |  |  |  |  |
| 2.0 | Miner | Worker | Minerals |  |  |  |  |  |
| 3.0 | Technician | Worker | Energy |  |  |  |  |  |
