---
title: "Damage Types"
source: "Game Stuff/Game Ideas/Damage Types"
modified: 2013-06-12
type: brainstorm
area: design-theory
status: "idea"
projects: ["[[Star Ruler mods]]"]
concepts: ["Design: Damage Types", "Design: Shield Mechanics", "Design: Module Damage Systems", "Design: Dynamic Balance Points", "Star Ruler mods"]
words: 983
summary: "Extensive design brainstorm on ship combat damage models: damage types, shields, module damage, flowchart damage bleed, hull breaches, and firing activity flow, citing many games."
merged_versions: ["Game Stuff/Game Ideas/Damage Types.odt"]
tags: ["area/design-theory", "project/star-ruler-mods", "type/brainstorm"]
---

**Damage Types**

Damage Categories with variable % resistances (eve)

Damage Categories with fixed resistances (starcraft, pokemon)

Fixed Damage point reduction (Quake)

Range Band determines damage (Full Thrust)

Damage over time (Warcraft III, DOTA, TD)

Special Utility Damage: Crew, Speed, Sensor (MOO2)

Temporary Damage "Shock" (Jagged Alliance 2)

Peircing Damage without HP loss (Full Thrust)

Critical Hit damage: Extra HP loss (Fallout)

Critical Hit special damage (Battletech)

Enveloping Damage: Immune to positional advantage, sandpapering (MOO2)

Damage causes vulnerability for a period of time. Debuff (MMORPG)

**Shield Mechanics**

Multi arc protection with HP soaking (MOO2)

Single arc (360) protection with HP soaking (eve)

Fixed damage reduction interger (no soaking) (full thurst)

Fixed damage reduction percent (no soaking) (MOO2)

Damage capping (starcraft immortals)

Deflection: Chance to miss (star ruler, MOO2)

**Module Damage Systems**

Chance to explode each time hit (Battletech magazines)

Explode when zero HP (everyhting)

System "air armor": Maximum damage per hit, rest is bled out/absorbed (car wars)

System arc location (star ruler)

System specific location (gratutious space battles)

System flowchart for damage bleeding (battletech) \*\*\*\*\*

Jettisoning sections of your ship

Modules grouped into ship sectors, each secotr is targettable.

Combinate ideas

Damage reduction from armor is removed only if the weapon cannot penetrate the armor.

Damage reductio only effects damage to systems.

Damage type utility and speed. Lasers hit immediate, railguns next turn, missile in 2 turns. The damage from each is better/worse for planning and prediction.

Structural Damage as HP that are rarely lost due to direct attack but are effected by systems loss. Example, ship hp drops only when a system is destroyed. Enough hp loss to ship destroys it.

Structural damage as centrepoint system. Once enough systems in the flowchart are damaged, the structure starts to take damage.

Damage that penetrates armor is divided by a number. If the result is 1 then one damage is applied to the first system in line. If 2, then one damage is applied to the first 2 systems in line. If 3, then 2 damage is applied to the first system in line, and 1 to the second. This number could be different for different weapons/weapon categories.

Hull breach system. Each attack that penetrates armor causes a hull breach that will effect a set of systems onboard. The player must choose to seal the breach (more danger of extra damage) or to purge the breach (removing those systems immediatly but stopping further risk of damage). Perhaps there are only so many teams on a ship that can be allocated to sealing breaches. If they are all already busy, then new breaches must be purged. Ships are hulked when all their crew are purged/died in fires.

Hits that cause no damage have lingering effects. This way thick armor can be shaken to lower levels with ablative fire and then penetrated with a middling attack. Similr with tanks I guess. Many hits will glance off.

Players may order "Brace for impact" whereby systems that are expected to be hit can harden for a turn.

Each ship has a N/S/E/W module which determines where the damage comes from in an attack on that quadrant. Larger ships have more than one per facing. Elongated ships have more on the sides than on the front. Vice versa for tall ships.

Systems arranged in a flowchart, each system has a number of allowed linkages. Dmage bleeds through the flowchart. Armor can be placed on the outside of this to protect the ship, but only has one linkage. Bulkheads could have two linkages. Engines also have one linkage so can have no armor covering them.

Ship damage increases instead of hp decrease. More damage accumulated means higher chance of modules breaking at any time.

Use a "living points balance update" system. Track which items and weapons players use, and adjust costs of them dynamically. Ones that are popular, and therefore better/imba, become more expensive over time, and the least used ones become cheaper.

Activity flow for firing

Player selects which weapons to fire

Each weapon has an activation delay (most have zero)

once delay is up determine hit locations

apply damage to locations

check for penetration

apply penerative damage to systems

check system destruction

apply system explosion damage to hull

check hull destruction

---

## Differences from other versions

_This document existed in several versions. The text above is the most complete one, unchanged. Below are the lines that appear only in the other versions._

### Only in “Damage Types” (Game Ideas, modified 2012-05-06)

Module Damage Systems
Structural Damage as HP that are rarely lost due to direct attack but are effected by systems loss
Systems arranged in a flowchart, each system has a number of allowed linkages. Dmage bleeds through the flowchart. Armor can be placed on the outside of this to protect the ship, but only has one linkage. Bulkheads could have two linkages.
