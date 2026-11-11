---
title: "Planetary Conditions Beta"
source: "Game Stuff/Game Ideas/Planetary Conditions Beta"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]", "[[RTS Ideas]]"]
concepts: ["FourEcks / 4X Space Empire", "Design: Planetary Conditions"]
words: 1123
summary: "Spreadsheet of planetary condition types for a space 4X (atmospheric, geological, biosphere, anomaly, habitability, homeworld, terrain-specific bonuses) with spawn chances and bonus/penalty effects."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "project/rts-ideas", "type/design-doc"]
---

## Sheet: Sheet1

| Name | Type | Chance | Bonus/Penalty | Chance of Biosphere | Chance of Anomaly |
|---|---|---|---|---|---|
| Verdant Mix | Atmospheric | 1.0 | Bonus to Food, Growth, Housing | 40.0 | 0.0 |
| Thin Oxygen | Atmospheric | 11.0 | Structure Cost +30% | 15.0 | 0.0 |
| Nitrogen Mix | Atmospheric | 18.0 | Strucutre Cost +40% | 5.0 | 0.0 |
| Airless | Atmospheric | 60.0 | Structure Cost +100% | 0.0 | 2.0 |
| Dense Mix | Atmospheric | 20.0 | Structure Cost +200% | 0.0 | 5.0 |
| Volatile Mix | Atmospheric | 10.0 | Structure Cost +500% | 0.0 | 10.0 |
| Archean | Geological | 2.0 | Structure Cost +100%, Mining +60% | -20.0 | 50.0 |
| Permean | Geological | 5.0 | Growth Bonus +20%, Housing Bonus +20% | 20.0 | 2.0 |
| Continental | Geological | 3.0 | Growth Bonus +50%, Housing Bonus +50% | 40.0 | 2.0 |
| Glacial | Geological | 30.0 | Electronics Bonus +50%, Food Penalty -80%, Structure Cost +50% | 0.0 | 20.0 |
| Regolith | Geological | 60.0 | Mining Bonus +20%, Food Penalty -50%, Structure Cost +20% | 0.0 | 10.0 |
| Coral Colonies | Biosphere | 10.0 | Luxuries Bonus |  |  |
| Microbes | Biosphere | 15.0 | Goods Bonus |  |  |
| Semi-Sentients | Biosphere | 10.0 | Labour Bonus |  |  |
| Herbivores | Biosphere | 15.0 | Food Bonus |  |  |
| World Trees | Biosphere | 10.0 | Defense Bonus |  |  |
| Abundant Forests | Biosphere | 10.0 | Housing Bonus |  |  |
| Edible Plants | Biosphere | 10.0 | Growth Bonus |  |  |
| Exploitable | Biosphere | 14.0 | Trade Capacity Bonus |  |  |
| Progenator Ancestors | Biosphere | 2.0 | Research Bonus |  |  |
| Progenator Deathworld | Biosphere | 1.0 | Research, Advanced Parts Bonus, Housing/Food/Growth Penalty |  |  |
| Ice Ring | Anomaly | 20.0 | Defense Bonus |  |  |
| Asteroid Ring | Anomaly | 20.0 | Offense Bonus |  |  |
| Radioactives | Anomaly | 20.0 | Advanced Parts Bonus |  |  |
| Progenator Ruins | Anomaly | 5.0 | Research Bonus |  |  |
| Ionosphere Storms | Anomaly | 5.0 | Defense Bonus |  |  |
| Volatile Deposits | Anomaly | 5.0 | Planetary Weapons Damage Bonus |  |  |
| Huge Mesa | Anomaly | 5.0 | Shipyard Bonus |  |  |
| Spice Melange | Anomaly | 5.0 | Starport Capacity Bonus |  |  |
| Core Canyons | Anomaly | 5.0 | Mining Bonus+, Cost Penalty |  |  |
| Orbital Construct | Anomaly | 2.0 | Offense/Defense Bonus |  |  |
| Shield Construct | Anomaly | 2.0 | Double Defense Bonus |  |  |
| Ancient Planetforming | Anomaly | 2.0 | Housing/Food/Growth/Cost Bonus, Large Ore Penalty |  |  |
| Ancient Warzone | Anomaly | 2.0 | Housing/Food/Growth/Cost Penalty, Large Ore Bonus |  |  |
| Construct World | Anomaly | 1.0 | 100x Ore, -100% Food, 10x Build Costs |  |  |
| Sentient Moon | Anomaly | 1.0 | 10x Build Cost, 10x Planetary Weapon Range, 10x PW Damage |  |  |
| Verdant | Habitability |  | No Penalty | Population Growth +25% |  |
| Habitable | Habitability |  | 20% Build cost increase | Population Growth +0% |  |
| Barely Habitable | Habitability |  | 50% Build Cost Increase | Population Growth -25% |  |
| Unfriendly | Habitability |  | 80% Build Cost increase | Population Growth -35% |  |
|  | Habitability |  | 100% Build cost increase | Population Growth -50% |  |
|  | Habitability |  | 125% Build cost increase | Population Growth -60% |  |
|  | Habitability |  | 150% Build Cost increase | Population Growth -70% |  |
| Dangerous | Habitability |  | 200% Build cost increase | Population Growth -85% |  |
| Deadly | Habitability |  | 250% Build Cost increase | Population Growth -90% |  |
| Uninhabitable | Habitability |  | Cant Build |  |  |
| Prewarp Infrastructure | Homeworld |  | Housing x30 |  |  |
| Edible Plants | Bonus |  | Food |  |  |
| Valuable Commodities | Bonus |  | Luxuries |  |  |
| Microbes | Bonus |  | Goods |  |  |
| Ferric Crust | Bonus |  | Metals |  |  |
| Silicates | Bonus |  | Electronics |  |  |
| Radioactives | Bonus |  | Advanced Parts |  |  |
| Huge Mesa | Bonus |  | Trade |  |  |
| Protective Landmass | Bonus |  | Damage Resitance and Structure Health |  |  |
| Anomalous Materials | Bonus |  | Research Bonus |  |  |
| Warm Ocean | Terran |  | Food |  |  |
| Coral Colonies | Terran |  | Luxuries |  |  |
| No Surface Water | Terran |  | Housing |  |  |
| Abundant Forests | Terran |  | Build Costs |  |  |
| Microbes | Terran |  | Goods |  |  |
| Rotational Stability | Lava |  | Electronics |  |  |
| Ferric Crust | Lava |  | Metals |  |  |
| Molten Ocean | Lava |  | Advanced Parts |  |  |
| Stable Continent | Lava |  | Trade |  |  |
| Dead Caldera | Lava |  | Damage Resitance and Structure Health |  |  |
| Surface Radioactives | Rock |  | Advanced Parts |  |  |
| Huge Mesa | Rock |  | Trade |  |  |
| Caverns | Rock |  | Damage Resitance and Structure Health |  |  |
| Core Canyons | Rock |  | Metals |  |  |
| Silicates | Rock |  | Electronics |  |  |
| Subterranean Ice | Desert |  | Food |  |  |
| Stable Weather | Desert |  | Trade |  |  |
| Meteor Craters | Desert |  | Housing |  |  |
| High Albedo | Desert |  | Electronics |  |  |
| Atmospheric Dust | Desert |  | Damage Resitance and Structure Health |  |  |
| Frozen Hydrogen | Ice |  | Electronics |  |  |
| Molten Core | Ice |  | Metals |  |  |
| High Gravity | Ice |  | Advanced Parts |  |  |
| Captive Comet | Ice |  | Research Bonus |  |  |
| Atmospheric crystals | Ice |  | Damage Resitance and Structure Health |  |  |
