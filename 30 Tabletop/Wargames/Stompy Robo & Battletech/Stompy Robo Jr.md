---
title: "Stompy Robo Jr"
source: "Game Stuff/Stompy Robo Jr"
modified: 2026-08-16
type: design-doc
area: wargame
status: "designed"
projects: ["[[Stompy Robo & Battletech]]", "[[Other Wargames]]"]
concepts: ["Stompy Robo", "Design: Mech Special Abilities", "Design: Wargame Deployment Scenarios", "Design: Wargame Terrain Rules"]
words: 1086
summary: "Design notes for a simplified, faster 'Jr' variant of the Stompy Robo mech wargame: restricted movement/range values, simple heat, fixed 1-3 point special abilities, simplified criticals, deployment scenarios, objectives and terrain rules."
tags: ["area/wargame", "project/other-wargames", "project/stompy-robo-battletech", "type/design-doc"]
---

Stompy Robo Jr

Goal of the design is that the players put their Mecha in danger on purpose because it yields a good result. Hiding and making conga lines does not yield good results. Promote sustained movement and kite orbiting/tangential fire.

Movement only 6, 12 or 24

TMM 1 2 and 4

Ranges are only \<6 or 6+

Only two Damage values

Range modifiers replaced with lower medium damage or more short damage

Forest move ends when entering or exiting

Mech bases are different sizes

No criticals

No heat, or simple heat.

No jumping

No standstill

No hit mods aside from TMM

Cover is just -1 damage dice

Rear hit is +1 damage dice

Lower damage units are more useful, how?

Phases

Strategy Phase (initiative and targeting)

Movement phase

Ew phase

Shooting

Clean up

Simple heat

Shooting generates one heat

Declare not shooting at start of round.

If you choose not to shoot, remove heat.

+1 to be hit per heat

+1 to critical rolls per heat

At end of shooting, add one heat to every unit that fired

Fixed smaller set of abilities

3 point specials

KEEN. Enemy units cannot deploy within X of this unit

ESCORT. The unit can always deploy touching another friendly unit

SCAN. The unit can scan objectives at double range

MARK. The unit gives a bonus to hit to all friendly units against any enemy it can see

WARN. The unit gives a bonus to defense to all units if it can see the firer

FADE. The unit can deploy closer to the enemy in the first turn

DISRUPT. The unit reduces enemy bonuses from the above 5 things

2 point specials

GYRO. Immune to the first movement critical hit.

LOCK. Immune to the first weapon critical hit.

PLATE. Immune to losing extra structure and losing abilities from critical damage

RIBS/RACK. Immune to instant destruction critical hits (like ammo or reactor hits)

(Reactive Internal Bulkhead System or Reactive Armour Containment Kit)

NULL: Ignore the effects of MARK, WARN, KEEN and SCAN.

JET: Unit can ignore terrain for one of its movements per turn.

1 point specials

BAIL/ZERO. Pilots reroll injury checks

ADAPT. Choose one of the units abilities and add a second one of the same cost to the mech. At the start of the battle, select one of the abilities to be active. Once at the start of this units activation, you may remove the ADAPT ability to swap between the two other abilities. For the purposes of damage, those two abilities count as one.

HOMING

BEAM

CANNON

Critical hit table

Design constraint: Criticals should affect every mech proportionally the same.

| Roll | Effect                                                                      |
|------|-----------------------------------------------------------------------------|
| 1-2  | Mobility hit                                                                |
| 3-4  | Weapon hit                                                                  |
| 5-6  | Roll a dice, on a 1 Instant destruction. Otherwise lose an ability or 1 HP. |

Motive hit: Unit has to move first

Weapon hit: one range band goes to zero damage

Extra damage: suffer one extra damage or lose one ability

Reactor hit: Instant destruction

MV, TMM, Arm, Struct, Short, Long

Deployment Gameplay

Facing is important?

### Patrols meet. 

Patrols meet. Two groups of units operating dark have bumped into each other unexpectedly. Combat begins at close range.

Roll off. Winner places one of the enemies units within 6” of the center of the board. The other player places one opposing unit in a position where it can see the first players unit, and the first players unit can see it.

Players now alternate placing units.

No unit can be placed within 6” of an enemy unit.

Units MUST be placed within 12” of an existing friendly unit, or within 18” of a friendly unit that has SCAN.

Units can always be set up on the table edge at a point nearest to a friendly unit.

No unit can be placed within 12” of an enemy unit with KEEN (the first unit placed is immune to this).

Units with FADE can deploy 3” closer to the enemy than normally allowed.

Units with ESCORT can always deploy within 1” of friendly units.

### Failed ambush / Honeypot

Players alternate placing beacons 12” apart. Then one random player places all units within 12” of the beacon. Then the other places based on placement specials. One turn where only units with KEEN or SCAN can act.

### Hot deployment 

One group sets up. None of their units can be within 12” of each other. One group arrives by drop ship, setting up two units within 2” of a single point anywhere on the board. At the end of each turn, they can deploy two more Mechs within 2” of the beacon. Any unit the beacon can see gets Marked twice at the start of the ewar phase. Any unit within 12” of the beacon gets attacked with 2 at the start of the shooting phase.

### Long Range encounter

Same as Patrols meet up increase to 12”/18”/24” deployment. SCAN, FADE and ESCORT are less important because of this.

Objectives

Apply damage to stationary target

Deal damage without taking losses

Keep units inside zone(s)

Destroy marked unit

Apply EWar multiple times to particular unit

Scan multiple points

Leave from edge

Escort unit from edge

Explore beacons

### Infantry and other vehicles

Don't have similar rules. Use asymmetry to make them weak but many.

### Terrain

Carparks/single story buildings/overpass. Flat raised areas that support size 1 or 2 but heavier must count it as difficult/dangerous/sticky terrain

Water tower/industrial pipes. Gives cover. Can be seen through but not moved through.

Red barrels/chem tanks. Gives cover but if a shot misses you still take 1 damage on a 4+.

Road/concrete. 2 extra move points if you start and end movement on a connected concrete section.

Dangerous. Starting/Passing/ending in this terrain, roll d6. 4+ take one damage.

Sticky. Passing through this terrain roll d6. 4+ your movement ends inside the terrain.

Explosive. If using this terrain, the first shot that misses you this turn on a 4+ causes one damage.

Difficult. Starting/passing this terrain costs 2”.

Dense (x) mechs up to x size ignore the terrain effects.

Cooling. No heat on firing if you are utilizing this terrain.

Hot. Extra heat if you are utilizing this terrain.

**Terrain should present risk and opportunities.**

### Movement idea

All mechs move 4 or 6 inches and have a run speed matching their movement. You can only use the run speed if you move to a spot you can see and do not turn at the end.
