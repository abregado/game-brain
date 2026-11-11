---
title: "Stellaris Tiericide"
source: "Game Stuff/Game Ideas/Stellaris Tiericide"
modified: 2021-03-16
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Stellaris mods]]"]
concepts: ["Stellaris mods", "Design: Tech Trees"]
words: 2970
summary: "Spreadsheet redesigning Stellaris ship tech tiers (hulls, weapons, defenses), with tech weights, costs, prereqs, ethic aggression table and a weapon stat table."
tags: ["area/game-idea", "project/stellaris-mods", "type/design-doc"]
---

## Sheet: Hulls

| Tech | Tier | Cost | Prereq | Specialization | Weight | Special Weight | Bonuses |
|---|---|---|---|---|---|---|---|
| Ships | Starting | 0.0 |  | Voidcraft | 0.0 |  | Corvette, Destroyer, Cruiser, Battleship hulls |
| Improved [Hull] Hulls | 1.0 | 2500.0 | Ships | Voidcraft | 12.0 | 1.5 has Standardized Hull Patterns, 3x has Specialization, 2x Supremacy Tradition | Hull HP + |
| Advanced [Hull] Hulls | 2.0 | 4000.0 | Ships | Voidcraft (Rare) | 12.0 | 1.5 has Improved Hull, 1.5 has Standardized Hull, 3x has Specialization, 2x Supremacy Tradition | Hull HP + |
| Standardized [Hull] Patterns | 1.0 | 1500.0 | Ships | Voidcraft | 12.0 | 1.5 has Improved Hull, 1.5 has Advanced Hull, 3x has Specialization, 2x Prosperity Tradition | Hull build Speed 25%, Hull Cost 5% |
| Corvette, Destroyer, Cruiser, Battleship, Titan Variants |  |  |  |  |  |  |  |
| [Hull] Specialization | 2.0 | 8000.0 | Ships | Voidcraft | 12.0 | x0 if any other Specialization | Hull HP +, Fleet Command +10 |
| [Hull] Specialization 2 | 4.0 | 8000.0 | Ships | Voidcraft | 12.0 | x0 if any other Specialization 2, x0 has same Specialzation 1 | Hull HP +, Fleet Command +10 |
| Corvette, Destroyer, Cruiser, Battleship |  |  |  |  |  |  |  |
| Juggernaut |  |  | Ships |  |  |  |  |
| Mega Engineering |  |  | Ships |  |  |  |  |
| Titans |  |  | Ships |  |  |  |  |
| Command Interfaces 1 | 2.0 | 500.0 | Ships | Voidcraft | 60.0 | x2 Militarist Ethic, x2 Supremacy Tradition | Fleet Command +10 |
| Command Interfaces 2 | 3.0 | 500.0 | CI 1 | Voidcraft | 60.0 | x2 Militarist Ethic, x2 Supremacy Tradition | Fleet Command +10 |
| Command Interfaces 3 | 4.0 | 500.0 | CI 2 | Voidcraft | 60.0 | x2 Militarist Ethic, x2 Supremacy Tradition | Fleet Command +10 |

## Sheet: aggressiveness

|  | agro | brave |  |  |  |
|---|---|---|---|---|---|
| honorbound | 1.75 | 1.5 |  | 8.75 | 3 |
| zealots | 1.25 | 1.0 |  | 6.25 | 2 |
| capitalists | 1.0 | 0.5 |  | 5 | 1 |
| imperialists | 1.5 | 1.0 |  | 7.5 | 2 |
| slavers | 1.5 | 0.5 |  | 7.5 | 1 |
| decadent | 0.5 | 0.5 |  | 2.5 | 1 |
| crusaders | 1.0 | 1.25 |  | 5 | 2.5 |
| purifiers | 2.0 | 1.0 |  | 10 | 2 |
| hive | 2.0 | 1.0 |  | 10 | 2 |
| swarm | 2.0 | 1.1 |  | 10 | 2.2 |
| machine | 1.0 | 1.0 |  | 5 | 2 |
| assimilators | 2.0 | 0.8 |  | 10 | 1.6 |
| exterminators | 2.0 | 1.0 |  | 10 | 2 |

## Sheet: Weapon Scratch

| Tech | Tier | Cost | Prereq | Specialization | Weight | Special Weight | Bonuses |
|---|---|---|---|---|---|---|---|
| Weapons | 0.0 | Starting |  |  |  |  | Laser, Mass Driver, Missiles, Strike Craft, Point Defense |
| [Weapon] Effectivness | 1.0 |  | Weapons |  |  |  | Bonus Damage +30% |
| [Weapon] Effectivness | 2.0 |  | WE 1 |  |  |  | Bonus Damage +30% |
| [Weapon] Effectivness | 3.0 |  | WE 2 |  |  |  | Bonus Damage +30% |
| [Weapon] Effectivness | 4.0 |  | WE 3 |  |  |  | Bonus Damage +30% |
| Laser, Mass Driver, Missiles, Strike Craft Versions |  |  |  |  |  |  |  |
| Change Mass Drivers to Materials expertise |  |  |  |  |  |  |  |
| Infinite [Weapon] Damage | 5.0 |  | WE 4 |  |  |  |  |
| Infinite [Weapon] ROF | 5.0 |  | WE 4 |  |  |  |  |
| [Weapon] Point Defence 1 | 2021-03-02 00:00:00 |  | WE 1 |  |  |  | Bonus Damage +30% |
| [Weapon] Point Defence 2 | 4.0 |  | WE 4 |  |  |  | Bonus Damage +30% |
| Flak and Point Defense versions |  |  | Laser or Projectile Spec |  |  |  |  |
| [Weapon] Specialization 1 | 1.0 |  | WE 1 |  |  | x0 if has other specialization |  |
| [Weapon] Specialization 2 | 3.0 |  | WE 3 |  |  | x0 if does not have Spec 1, x0 if has other Spec 2 |  |
| Early Special Weapons |  |  |  |  |  |  |  |
| Torpedo | 2.0 |  | Missile Effectivness 2 |  |  | x0 unless has Missile Spec |  |
| Swarmer Missiles | 2.0 |  | Missile Effectivness 2 |  |  | x0 unless has Missile Spec |  |
| Kinetic Battery | 2.0 |  | Projectile Effectivness 2 |  |  | x0 unless has Proj Spec |  |
| Plasma Thrower | 2.0 |  | Laser Effectivness 2 |  |  | x0 unless has Beam Spec |  |
| Late Special Weapons |  |  |  |  |  |  |  |
| Disruptors | 3.0 |  | WE 3 |  |  | x0 unless only Beam and Proj Spec |  |
| Proton Launcher | 3.0 |  | WE 3 |  |  | x0 unless has Missile and Beam Spec |  |
| XL Weapons |  |  |  |  |  | x0 If has no Effectiveness 3, x0 has no Specialization |  |
| Arc Emitter | 4.0 |  | WE 4, Disruptors |  |  | x0 unless Beam and Proj Specs |  |
| Particle Lance | 4.0 |  | WE 4 |  |  | x0 unless Beam Spec |  |
| Mega Cannon | 4.0 |  | WE 4 |  |  | x0 unless Projectile Spec |  |

## Sheet: Weapon techs

|  | tier | component unlock | price increase | damage increase |
|---|---|---|---|---|
| tech_lasers_1 | 0.0 | SMALL_RED_LASER, MEDIUM_RED_LASER,LARGE_RED_LASER |  |  |
| tech_lasers_2 | 1.0 |  | 1.3 | 1.3 |
| tech_lasers_3 | 2.0 |  | 1.3 | 1.3 |
| tech_lasers_4 | 3.0 | SMALL_XRAY_LASER, MEDIUM_XRAY_LASER,LARGE_XRAY_LASER |  |  |
| tech_lasers_5 | 4.0 |  | 1.3 | 1.3 |
| tech_energy_lance_1 | 4.0 |  |  |  |
| tech_energy_lance_2 |  |  |  |  |
| tech_plasma_1 |  |  |  |  |
| tech_plasma_2 |  |  |  |  |
| tech_plasma_3 |  |  |  |  |
| tech_arc_emitter_1 |  |  |  |  |
| tech_arc_emitter_2 |  |  |  |  |
| tech_disruptors_1 |  |  |  |  |
| tech_disruptors_2 |  |  |  |  |
| tech_disruptors_3 |  |  |  |  |

## Sheet: Sheet6

| key | cost | power | min_damage | max_damage | hull_damage | shield_damage | shield_penetration | armor_damage | armor_penetration | min_windup | max_windup | cooldown | range | accuracy | tracking | missile_speed | missile_evasion | missile_shield | missile_armor | missile_health | missile_retarget_range | end |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| # Lasers |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SMALL_RED_LASER | 10.0 | -5.0 | 6.0 | 16.0 | 1.0 | 0.5 | 0.0 | 1.5 | 0.0 | 2.0 | 20.0 | 35.0 | 40.0 | 0.9 | 0.5 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_RED_LASER | 20.0 | -10.0 | 15.0 | 40.0 | 1.0 | 0.5 | 0.0 | 1.5 | 0.0 | 2.0 | 20.0 | 35.0 | 60.0 | 0.9 | 0.3 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_RED_LASER | 40.0 | -20.0 | 36.0 | 96.0 | 1.0 | 0.5 | 0.0 | 1.5 | 0.0 | 2.0 | 20.0 | 35.0 | 80.0 | 0.9 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| SMALL_XRAY_LASER | 13.0 | -13.0 | 7.69 | 20.71 | 1.0 | 0.5 | 0.0 | 1.5 | 0.0 | 2.0 | 20.0 | 35.0 | 40.0 | 0.9 | 0.5 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_XRAY_LASER | 26 | -23.0 | 19.53 | 52.07 | 1.0 | 0.5 | 0.0 | 1.5 | 0.0 | 2.0 | 20.0 | 35.0 | 60.0 | 0.9 | 0.3 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_XRAY_LASER | 52 | -45.0 | 46.15 | 124.26 | 1.0 | 0.5 | 0.0 | 1.5 | 0.0 | 2.0 | 20.0 | 35.0 | 80.0 | 0.9 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| # Mass Drivers |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SMALL_MASS_DRIVER_1 | 10.0 | -5.0 | 5.0 | 16.0 | 1.0 | 1.5 | 0.0 | 0.5 | 0.0 | 1.0 | 18.0 | 25.0 | 50.0 | 0.75 | 0.5 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_MASS_DRIVER_1 | 20.0 | -10.0 | 13.0 | 40.0 | 1.0 | 1.5 | 0.0 | 0.5 | 0.0 | 1.0 | 18.0 | 25.0 | 75.0 | 0.75 | 0.3 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_MASS_DRIVER_1 | 40.0 | -20.0 | 30.0 | 96.0 | 1.0 | 1.5 | 0.0 | 0.5 | 0.0 | 1.0 | 18.0 | 25.0 | 100.0 | 0.75 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
|  | 13.02 |  | 6.51 | 20.71 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|  | 26.04 |  | 16.57 | 52.07 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|  | 52.07 |  | 39.05 | 124.26 |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SMALL_MASS_DRIVER_4 | 22.0 | -13.0 | 11.0 | 35.0 | 1.0 | 1.5 | 0.0 | 0.5 | 0.0 | 1.0 | 18.0 | 25.0 | 50.0 | 0.75 | 0.5 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_MASS_DRIVER_4 | 44.0 | -23.0 | 28.0 | 88.0 | 1.0 | 1.5 | 0.0 | 0.5 | 0.0 | 1.0 | 18.0 | 25.0 | 75.0 | 0.75 | 0.3 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_MASS_DRIVER_4 | 88.0 | -45.0 | 66.0 | 210.0 | 1.0 | 1.5 | 0.0 | 0.5 | 0.0 | 1.0 | 18.0 | 25.0 | 100.0 | 0.75 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| # Plasma |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SMALL_PLASMA_1 | 15.0 | -10.0 | 12.0 | 25.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 40.0 | 0.8 | 0.4 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_PLASMA_1 | 30.0 | -17.0 | 30.0 | 63.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 60.0 | 0.8 | 0.2 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_PLASMA_1 | 60.0 | -34.0 | 72.0 | 150.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 80.0 | 0.8 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| SMALL_PLASMA_2 | 20.0 | -13.0 | 16.0 | 33.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 40.0 | 0.8 | 0.4 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_PLASMA_2 | 40.0 | -23.0 | 40.0 | 83.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 60.0 | 0.8 | 0.2 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_PLASMA_2 | 80.0 | -45.0 | 96.0 | 198.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 80.0 | 0.8 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| SMALL_PLASMA_3 | 25.0 | -17.0 | 20.0 | 42.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 40.0 | 0.8 | 0.4 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_PLASMA_3 | 50.0 | -30.0 | 50.0 | 105.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 60.0 | 0.8 | 0.2 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| LARGE_PLASMA_3 | 100.0 | -59.0 | 120.0 | 252.0 | 1.5 | 0.25 | 0.0 | 2.0 | 0.0 | 2.0 | 20.0 | 40.0 | 80.0 | 0.8 | 0.05 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| # Disruptors |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| SMALL_DISRUPTOR_1 | 15.0 | -10.0 | 1.0 | 18.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 2.0 | 20.0 | 50.0 | 30.0 | 1.0 | 0.6 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_DISRUPTOR_1 | 30.0 | -17.0 | 1.0 | 45.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 2.0 | 20.0 | 50.0 | 50.0 | 1.0 | 0.35 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| SMALL_DISRUPTOR_2 | 20.0 | -13.0 | 1.0 | 23.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 2.0 | 20.0 | 50.0 | 30.0 | 1.0 | 0.6 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_DISRUPTOR_2 | 40.0 | -23.0 | 1.0 | 58.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 2.0 | 20.0 | 50.0 | 50.0 | 1.0 | 0.35 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| SMALL_DISRUPTOR_3 | 25.0 | -17.0 | 1.0 | 30.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 2.0 | 20.0 | 50.0 | 30.0 | 1.0 | 0.6 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| MEDIUM_DISRUPTOR_3 | 35.0 | -30.0 | 1.0 | 75.0 | 1.0 | 1.0 | 1.0 | 1.0 | 1.0 | 2.0 | 20.0 | 50.0 | 50.0 | 1.0 | 0.35 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| # Autocannons |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| AUTOCANNON_1 | 15.0 | -10.0 | 8.0 | 16.0 | 1.25 | 1.5 | 0.0 | 0.25 | 0.0 | 2.0 | 14.0 | 15.0 | 30.0 | 0.85 | 0.75 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| AUTOCANNON_2 | 20.0 | -13.0 | 10.0 | 21.0 | 1.25 | 1.5 | 0.0 | 0.25 | 0.0 | 2.0 | 14.0 | 15.0 | 30.0 | 0.85 | 0.75 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| AUTOCANNON_3 | 25.0 | -17.0 | 14.0 | 27.0 | 1.25 | 1.5 | 0.0 | 0.25 | 0.0 | 2.0 | 14.0 | 15.0 | 30.0 | 0.85 | 0.75 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| # Kinetic Artillery |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| KINETIC_ARTILLERY_1 | 120.0 | -70.0 | 150.0 | 450.0 | 1.25 | 2.0 | 0.0 | 0.5 | 0.0 | 3.0 | 25.0 | 50.0 | 120.0 | 0.75 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |
| KINETIC_ARTILLERY_2 | 155.0 | -90.0 | 195.0 | 585.0 | 1.25 | 2.0 | 0.0 | 0.5 | 0.0 | 3.0 | 25.0 | 50.0 | 120.0 | 0.75 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 | 0.0 |  |

## Sheet: Defenses

| Tech | Tier | Cost | Prereq | Specialization | Weight | Special Weight | Bonuses |
|---|---|---|---|---|---|---|---|
| Defenses |  |  |  |  |  |  | Tier 1 hull/armor/shield |
| Tier 1 Hull item. 3/5 HP of Armor, Same price |  |  |  |  |  |  |  |
