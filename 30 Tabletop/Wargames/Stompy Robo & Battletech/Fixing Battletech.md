---
title: "Fixing Battletech"
source: "Game Stuff/Fixing Battletech"
modified: 2025-01-30
type: design-doc
area: wargame
status: "designed"
projects: ["[[Stompy Robo & Battletech]]"]
concepts: ["Stompy Robo", "Battletech homebrew"]
words: 1854
summary: "Design doc for a simplified, stompy Battletech-inspired tabletop game: pillars, heat tokens, arcs, mech/pilot/weapon specials, deployments, campaign aftermath, salvage tables and scenarios."
tags: ["area/wargame", "project/stompy-robo-battletech", "type/design-doc"]
---

# Fixing Battletech

## Things that are “Battletech-esque” to me

- Heat management

- Firing arcs

- Hitting enemies in the back

- Risking a turn and falling over

- Disabled mechs are still dangerous

- Kiteing the enemy

- Splitting fire

- Choosing when not to fire

## Bad things in classic 

- Rolling to hit a lot

- Missile clustering

- Can't aim at parts

- Moving really doesn't make a difference for heat

## Bad things in Alpha Strike

- No arcs

- No heat management

- No falling over

- No risk taking

## Pillars

**This is not Battletech:** I can free myself from making everything in Battletech compatible with this new system.

**Simplicity is king:** I want the game to be simple and quick to play compared to Alpha Strike and especially Classic.

**Should feel stompy:** You are controlling giant mechs. It should feel like it. Mechs are the most powerful things on the battlefield by a large margin.

**Miniature Agnostic:** You do not need special figurines to play this game

**Few but important choices per activation:** The choices that the player makes should be meaningful and impactful, not nuanced and obfuscated.

**Special Rules are exceptions to normal rules:** Special rules should not have their own mechanics, instead they allow you to ignore regular rules in certain situations.

**Nothing is modelled twice:** Whenever possible, things are simulated in only one way.

## Concrete ideas

Damage number with range

A mech could have 2l and 2m. This also shows how damage can be split.

Asymmetrical arcs

Arms arcs are bigger but also easier to exploit.

Center arc is smaller

Vehicles have turrets

Facing damage allocation

Allocate damage to each forward hex face. Players can easily see where a mechs blind spots are.

Replace heat with tokens. Fired everything and moved? Add a heat token. Did nothing, remove one. Roll a dice for every token at the end of the turn.

Don't just convert mechs

Make a subset of mechs that are balanced

Goldilocks range accuracy

Vulnerable status

Given as a penalty for taking a risk and failing. Makes this mech a better target for other mechs.

Use classic movement

Adjust damage for range and remove range modifiers

Make size matter somehow, in base it's just punch damage. Maybe deployment?

Place Speed based modifiers as tokens

No speed bonus when on road the whole time.

Campaign mode. All players build lists, then only those designs are available for the campaign.

Omni mechs are just multiple designs with the same cost, and a x1.1 or x1.2 modifier and you can choose before the mission which variant is used. Only armor, weapons and specials change.

Vehicles just have movement, damage threshold (0-2) and weapons. Different movement modes just modify the damage threshold. VTOL -1, Tracked +1. Threshold 0 means you auto hit and kill if you target it. Hitting a target and not killing it adds a heat token. Heat tokens reduce threshold.

Weapons (any combination of two adjacent ranges)

0/1/1

1/1/0

2/0/0

Or one range with a special

Use asterisks to mark “half” damage

Woods and cover just give Miss rolls (3+ and 5+)

Medium range out to 9 hexes

Short out to 3

Long out to 20

No range penalties to hit.

Move range bonuses/penalties to the Pilots +1/-1

2 tonnes is 1 HP

4 tonne is 1 weapon

1 move =

Pick armor and extra structure values. 1 to 7

Pick speed

Pick 1-6 weapons

Allocate weapons

Pick specials

Pick size/signature (effects structure)

Movement should be a modifier on offense and defense

Needed Mech Specials

Ignore Criticals

- Armored Actuators

- Protected Weaponry

- Ejectable Ammo

- Engine Redundancy

Superior Ejection System

Indirect Fire

No Arms

AMS

Put order tokens on your mechs. The first one finished gets to add an extra one.

- Advance

- Manuever

- Stand Still

- Eject

This determines the order of movement

More mechs, but they die faster?

Popcorn Initiative? Does not solve the cognitive load.

Pilot Abilities

Distraction: If this moves first, bonus to Initiative

Baiter: After this unit acts, pick an enemy mech. That mech moves next.

Captain: If on the board, Initiative bonus

Mentor: When this mech is activated, you can choose to move a different mech instead.

Deployments

Mechbay: place mechs + 2 Mechbay terrain pieces.

Only activate 2 mechs in the first turn, and 3 in the second. Mech’s spawn at the start of their activation at a mech bay. Each mech bay can only be used once per turn.

Dropship

Opponent places their mechs anywhere on the board

Place one mech outside 8 hexes of any opponent mech

Place all other Mechs within adjacency of another friendly mech

Drop pods

One player places their mechs activations tokens on the board, face down, anywhere they like.

Second player places their activation tokens facedown anywhere they like, but not within 8 hexes of any enemy token.

Then the second player replaces each token with a mech from their roster. Any mech can replace any token.

Then the second player replaces their tokens with the corresponding mechs.

Objective Types

Strike: Attacker will need to leave the board afterward

Occupy: Attacker will not need to leave the board

Raid: Multiple points to protect. Attacker needs to reach a series of hexes

**Weapon specials**

Energy: Ignore Cover

Indirect: Ignore Obstructed except Mechs

Seeking: -1 per Heat on the target

Warmup: Take a Vulnerable token when you decide to fire. +2 damage.

Burst Fire: +1 damage if you have no heat

Pierce/EMP: Crits on 11. +2 to crits.

Flame: Crits always cause Heat. Crit on 10. Weapon only does damage on crit. (16% crit chance)

Impact: Crits always cause Vulnerable, Crits on 10. Crits cause Armor damage instead of Structure. (16% crit chance)

**Mech Specials**

Flexible Actuators: Ignore one Difficult hex per turn (-1 Structure)

Reactive Armor: +1 Armor (-2 structure)

Protected weapons: Reroll Arm Crits (-1 structure)

Armored actuators: Reroll Leg crits (-1 structure)

Sealed Reactor: Ignore Heat Crits on a 4+ (-1 Structure)

Steady: Ignore Vulnerable crits on a 4+ (-1 Structure)

Lightweight Frame: You can make two Risky moves (-1 structure)

Low profile: +3 from Obstructed (-1 structure)

Foldable: +3 from Cover (-1 structure)

Skates: +2 free moves on Roads (-1 Structure)

Deployable: -1 to hit if you didnt move this activation (-1 Structure)

Stealth: Deploy 2 hexes closer than allowed. (-1 Structure)

Targeting Computer: Ignore Obstructed within 2 hexes when firing (-2 Structure)

Safety Overrides: You may fire two weapons, but gain 3 heat when you do. (-2 Structure)

A single special can be selected when the mech is designed.

Addon specials can be found during the campaign.

**Pilot Specials**

Pathfinder. At the start of each campaign, select one type of terrain that is Difficult. That terrain also gives this pilot Cover.

Gymnast: +1 Skill if piloting a Mech with 2 or more Agility

Heavyweight: +1 Skill if piloting a Mech with 6 or more Structure

Distracting: After you should activate your first mech, you may activate this mech instead.

Provoker: When this mech activates, choose an enemy mech in Short range. That mech must move first.

Weapon Specialist: When firing with one random weapon type, +1 Skill. Determine the type randomly from weapon types on your mech lineup.

Opportunist: +1 Skill when operating a mech with weapons covering all ranges.

Quickdraw: +1 Skill when operating a mech with more than one weapon.

Sniper: +1 Skill when firing at long range. -1 Skill when firing at medium range.

Brawler: +1 Skill when firing at short range. -1 Skill when firing at medium range.

Risk Taker: Always roll one extra dice when making Risky moves. Discard the worst dice.

Redliner:If you would gain a Shutdown token, roll a D6 per Heat token. As long as no 1’s are rolled, you don’t gain a Shutdown token. If you roll any duplicates, suffer D6 Structure damage.

Quick Flush: When you dump heat you may roll a D6. On a 1, only remove 1 Heat. On 6 you flush Heat and may fire this turn (which still generates one Heat)

Ambusher: Stealth: Deploy 2 hexes closer than allowed.

Sprinter: +2 Move if you use no Agility on a turn.

Command: When this mech should activate, you can activate another mech within Medium range instead.

Frontliner: When a mech within Medium range would activate, you may activate this mech instead.

Ghost: Reroll failed MIA and Ejection rolls that this pilot makes.

Techie: Reroll failed permanent damage rolls.

Post Battle Pilots

Roll a D6 for every MIA pilot. On a 1 they are Dead. On a 2-5 they return to your roster.

For every pilot who was in a mech that has zero structure, roll a D6. On a 1 they are MIA.

Post Battle Mechs

Roll a D6 for every mech at zero structure. On a 1-2 it has permanent damage.

1-2: Quirk. 3-6: -1 Structure.

Every mech that you didn’t use is repaired 100%. Quirks are not removed.

Where is the money?

It is assumed that you get paid enough for the mission to cover your running costs and repair bills.

Salvage

Roll 3D6 plus 2D6 if you won, and 2D6 for each mech you scrap from your roster. Take this many salvage units. You must have at least 8 mechs in your roster.

Together all players roll 4D6 on the Opportunity chart. The winner makes the first pick to buy. Once selecting an option, roll for the price. If you cannot afford it, then you lose your pick. Players alternate buying until they both pass, or there is nothing left to buy.

For each salvage you are lacking, you can roll 2D6 and spend that many credits.

After purchasing is done each excess salvage is converted into D6 Credits.

| Roll | Cost | Opportunity                                                                                                                                              |
|------|------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| 12   | x    | Choose                                                                                                                                                   |
| 11   | 15   | Ancient Mech: See below                                                                                                                                  |
| 10   | 13   | Roll twice on the Weapon chart. Pick one after you buy.                                                                                                  |
| 9    | 11   | Roll twice on the Upgrade chart. Pick one after you buy.                                                                                                 |
| 8    | 6    | Roll twice on the Tech ammo chart and pick one after you buy                                                                                             |
| 7    | 4    | Tech Ammo. or Nanites                                                                                                                                    |
| 6    | 6    | Gain 4D6x3 Credits or 2 Nanites                                                                                                                          |
| 5    | 7    | Quirk Repair kit. Immediately remove one Quirk or a lost Structure from a mech.                                                                          |
| 4    | 8    | Blackmarket Mech Upgrade. Roll the Upgrade after you buy                                                                                                 |
| 3    | 9    | Blackmarket Weapon Upgrade. Roll the Upgrade after you buy                                                                                               |
| 2    | 15   | Ancient Mech: One random campaign mech, with a Quirk, -1 Structure and an extra Mech Upgrade. Roll the Upgrade before you buy, and the Quirk afterwards. |

Scenarios

Convoy: Threshold 1 vehicles. Move 2 spaces per turn. Start 8-10 tiles away.

Attacker: +1 VP per tank destroyed

Defender: +1 VP per tank surviving, +3 VP per mech kill

Attacker can kill one vehicle when they stand in the space
