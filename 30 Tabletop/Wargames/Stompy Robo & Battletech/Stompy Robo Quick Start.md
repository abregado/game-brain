---
title: "Stompy Robo Quick Start"
source: "Game Stuff/Stompy Robo Quick Start"
modified: 2026-02-20
type: design-doc
area: wargame
status: "prototyped"
projects: ["[[Stompy Robo & Battletech]]", "[[Other Wargames]]"]
concepts: ["Stompy Robo", "Battletech homebrew", "Design: Mercenary Campaign Layer", "Design: Wargame Terrain Rules"]
words: 3344
summary: "Full quick-start rulebook draft for Stompy Robo, a hex-based mech skirmish game: setup, phases, movement/agility, heat, firing with dice pools, criticals, support vehicles, a mercenary campaign layer, plus a list of ideas for weapon types, mech/pilot abilities and weather."
tags: ["area/wargame", "project/other-wargames", "project/stompy-robo-battletech", "type/design-doc"]
---

# Game Terminology

Unit

Mech

Support Vehicle

Unit Card

Movement scores

Armor

Structure

Weapons

Price

Pilot Card

Skill

Training

Squad Roster

Dice

Target Number

Movement points

Hex

Hex face

Unit Facing

Weapons

Weapon positions

Terrain Types

Difficult Hexes

Obstructed Hexes

Blocking hexes

Line of Sight

Tokens

Heat token

Vulnerable token

Critical token

Shutdown token

## Terrain Types

Each hex can have any combination type tags. Here are some examples:

**Water, Mud or Gravel**: Difficult

**Forest**: Obstructed

**Boulders, Light Wreckage**: Difficult, Cover and Obstructed

**Light Buildings**: Difficult, Cover and Obstructed

**Heavy Buildings**: Impassable and Blocking

**Wreckage**: Impassable and Obstructed

**Lava or Chasm:** Impassable

**Dust or Smoke**: Obstructed

**Crater:** Cover, Difficult

**Deep Water**: Cover, Difficult

# The Setup

## Determine objective

## Determine Weather and Terrain

## Determine attacker

Roll 2D6. Player with the highest score decides if they are attacker or defender.

## Select Squad

Both players select a squad of 4 mechs

## Defender deploys support vehicles

## Attacker deploys support vehicles

## Mechs are deployed

Defender places mech with highest sensor rating.

Attacker places a mech anywhere outside the defender's sensor range.

Players alternate placing mechs until all are placed.

## Pregame Shooting phase

Every mech that can shoot, may shoot. Mechs that shoot gain a heat token.

## Pregame End Phase

## First Initiative phase

#  

# The Battle

Each round of battle is resolved using a number of phases:

- Initiative Phase

- Movement Phase

- Firing Phase

- Cleanup Phase

## Initiative Phase

Each player rolls 2D6. Reroll a tied result. The player with the highest result is considered the winner.

## Movement Phase

### Activation order

During the Movement Phase, players activate their mechs until all mechs have been moved. Start with the player who lost the Initiative and alternate between players. Mechs with Shutdown tokens cannot be activated.

### Make move

The movement capabilities of a mech are shown with two numbers: Speed and Agility. Speed determines how far a mech may move, and Agility determines how much a mech can turn during its activation. The tables below show what you can spend each on.

##### MOVEMENT COST

|     | Forward 1 hex           | 1pt       |     |
|-----|-------------------------|-----------|-----|
|     | Backward 1 hex          | 2pt       |     |
|     | Target hex is Difficult | +1pt      |     |
|     | Road                    | special\* |     |

##### AGILITY COST

|     | Turn one hex facing | 1pt |     |
|-----|---------------------|-----|-----|
|     |                     |     |     |

### Risky Moves

During an activation a mech may spend one more Speed and one more Agility than it has available. The move is then considered Risky, and a Pilot (x) check has to be made at the end of the activation.

### Special movement rules

#### Difficult Hexes

Any hex which contains obstacles which will not stop, but might interfere with a mech's movement, counts as Difficult. Some examples of obstacles would be small buildings, trees or water. It costs one extra Speed point to enter a Difficult hex.

#### Road movement

As long as a mech or vehicle is moving between two hexes connected by a road it does not need to spend extra Speed for entering Difficult hexes.

#### Impassable Hexes

Some hexes cannot be crossed or entered by normal means. These are called Impassable hexes.



*Example 1: A mech with 5 speed and 1 Agility. Two Speed is spent to move forward two hexes. Then one Agility is spent to turn to the right. Finally three speed is spent to move into the hex with buildings (counts as Difficult)*



*Example 2: The same mech makes the same move but only pays 4 Speed and 1 Agility as the road reduces the cost to enter the Difficult hex.*

## End of Movement

#### Stationary penalty

If the mech ends its activation in the same hex as it started, place a Vulnerable token on it.

#### Pilot check for Risky movement

A Pilot check is a roll used to determine the consequences of a situation. The notation Pilot (x) check are used to show the difficulty of this roll.

Roll a number of white dice equal to the (x) component of the notation.

If any of the dice results are greater than the Skill of the pilot, then the check has failed. Add a Vulnerable token to the mech.



*Example: Assuming a Pilot skill of 6, A and C are successful while B and D are not and would gain a Vulnerable token.*

Place Activated token

Once a mech has been activated, place an Activated token next to it to show that it had its movement Activation for this turn.

## Firing Phase

### Remove Activation tokens

All Activation tokens from the movement phase can be removed now. Keep them nearby, as they are needed again in this phase.

### Decide cool off

Each player can now decide which of their mechs will cool off instead of attacking. A mech which cools off loses all of its heat tokens. Mark mechs that decide to cool off by placing their activation token next to them.

### Allocate shots

The players simultaneously decide which mechs will attack which targets by placing their activation tokens next to enemies.

#### Target selection line of sight

Choose a target. Draw a straight line between the hex center of the attacker and the hex center of the target. If this line does not touch the edges of any Blocking hexes, the target can be attacked.

### Resolve attacks

Now each attack is resolved in any order that the players choose.

## Firing Resolution

### Determine Range

Count the number of hexes to the target from the attacker. Count the target’s hex, but not the attacker's hex.

##### RANGE TABLE

| 0 (same hex) | Melee range  |
|--------------|--------------|
| 1-4          | Short Range  |
| 5-9          | Medium Range |
| 10+          | Long Range   |
|              |              |



*Example 2: A and C are 4 hexes away (Medium Range). B is two hexes away (Short Range)*

Take one white dice for each damage shown on the mech’s weapons chart for the given range.

|         | **SHORT** | **MEDIUM** | **LONG** |
|---------|-----------|------------|----------|
| Weapons | 1         | 4          |          |

*Example 3: B can be attacked with 1 Damage, C and A with 4 Damage.*

### Calculate dice target

To cause damage, the dice must equal or beat a target number.

The target number begins at 7 and is modified by a number of factors shown on the following table.

##### TO-HIT MODIFIERS

|     | Target is in Cover hex                                                | +2  |     |
|-----|-----------------------------------------------------------------------|-----|-----|
|     | There is at least one obstructed hex between the attacker and target. | +2  |     |
|     | Per Vulnerable token on the target                                    | -2  |     |
|     | Per Shutdown token on the target                                      | -2  |     |
|     | If you are firing into the targets rear arc                           | -2  |     |
|     | \*Ignore the effects of hexes that are adjacent to the attacker.      |     |     |

#### Obstructed Hexes

Any hex containing something that blocks vision or is likely to disrupt damage being applied to a target counts as Obstructed. This includes mechs, trees or light buildings. Obstructed hexes make it harder to hit targets.

#### Cover Hexes

Any hex that contains something solid that a mech could hide behind if it is in the hex. This includes craters, buildings or deep water.

#### Hitting the rear

If the line between the attacker's hex center and the targets hex center passes through the rear hex face of the target, the attack is considered to be hitting the rear.

### 

###  

### Make attack roll

Take the white damage dice and a single red dice and roll them together. The red dice is called the Gunnery dice.



Add the Gunnery dice to each of the damage dice. If the total is equal to or greater than the dice target, one damage is caused.

*Example 4: Assuming a target number of 7, A and B and D cause 2 damage C and E cause 3 damage.*

*Example 5: C, D and E all cause a single Critical token to be added to the target. This would still be the case if the target number was more than 12.*

For each damage caused, mark an armor or structure on the target's card. If any structure is removed, add a Critical token to the card. These are resolved later.

| Armor     | 1   | 2   |     |     |
|-----------|-----|-----|-----|-----|
| Structure | 3   |     |     |     |

| Armor     | 1   |     |     |
|-----------|-----|-----|-----|
| Structure | 2   | 3   |     |

| Armor     | 1   | 2   | 3   |     |
|-----------|-----|-----|-----|-----|
| Structure |     |     |     |     |

*Example 6: If you were dealing 3 damage to each of these mechs, the first two would have a single Critical Token added to their cards.*

#### Penetrating Hits

Regardless of the target roll, if the Gunnery die rolls a 6, each damage die that also rolls a 6 causes structure damage instead of armor.

##  

## Cleanup Phase

Complete each of the following steps in order

#### Remove Vulnerable Tokens

Any vulnerable tokens on the board are removed.

#### Critical Damage

For each Critical token on a mech, roll a D6 and consult the following table to resolve what happens.

##### CRITICAL HITS

<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 22%" />
<col style="width: 61%" />
</colgroup>
<thead>
<tr class="header">
<th>1</th>
<th>Leg Hit</th>
<th>Move 0</th>
</tr>
<tr class="odd">
<th>2</th>
<th>Arm Hit</th>
<th><p>First: Front arc only</p>
<p>Second: Half damage (round down)</p></th>
</tr>
<tr class="header">
<th>3-4</th>
<th>Knocked</th>
<th>Generate Vulnerable</th>
</tr>
<tr class="odd">
<th>5-6</th>
<th>Coolant</th>
<th>Generate 1 Heat</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

#### Remove Shutdown tokens

Any mechs which start the Cleanup Phase with Shutdown tokens have those tokens removed.

#### Remove Critical tokens

All critical tokens are removed from mechs.

#### Remove destroyed mechs

Mechs with no Structure remaining, or that suffered either an Ammo or Cockpit hit, are removed from the board.

#### Shutdown hot mechs

Mechs with 4 or more heat Tokens lose their Heat tokens but gain a Shutdown token. Other heat tokens are not removed. To remove these tokens, consult the Firing phase rules.

#### Decide winner

If one player has no units to activate, or the mission objective has been fulfilled, the game is over.

## Next Round

Begin a new round with an Initiative Phase.

##  

## Support vehicles

While mechs are the powerhouses of the battlefield, sometimes there will be other vehicles involved. These follow much simpler rules.

Any vehicle that is not a mech is considered a support vehicle.

### No facing cost

When moving a support vehicle, you can change its facing for free.

### Special movement types

There are several special types of support vehicle movement types. Wheeled vehicles are any vehicle that uses wheels to move. VTOL vehicles are those that can fly or hover, such as helicopters. Tracked vehicles use caterpillar tracks to move, like tanks.

Wheeled support vehicles gain 2 extra movement when moving exclusively along roads, but cannot enter obstructed hexes without road.

VTOL support vehicles ignore movement bonuses and penalties for obstructions and roads. They also have their Threshold reduced by 1.

Tracked support vehicles are the default type and suffer no penalties or bonuses to movement.

### Suffering damage

Damage is never tracked for support vehicles. They do not have unit cards.

A support vehicle is destroyed if it receives damage equal to or over its Threshold value from a single attack. If it is not destroyed by an attack, add a Vulnerable token to the vehicle.

One damage dice is added to every attack for each Vulnerable token a support vehicle has.

If a support vehicle would gain a Critical token, it is destroyed instead.

A Threshold of 0 means that the support vehicle will be destroyed if it is shot at. No to-hit roll is required.

### Firing

Support vehicles only have one weapon which has a 360 degree arc. Firing with a support vehicle uses the same rules as firing with a mech.

Support vehicles always have a Skill of 6.

Attacks made by support vehicles cannot cause Critical tokens to be added to their targets.

### Types of support vehicle

|           | **Move** | **TH** | **S** | **M** | **L** |
|-----------|----------|--------|-------|-------|-------|
| Artillery | 2        | 1      |       |       | 3     |
| Tank      | 2        | 2      | 1     | 1     |       |
| Mech Inf  | 3        | 1      | 1     | 1     |       |
| Hvy Tank  | 1        | 3      | 1     | 1     |       |
| Scout     | 4        | 1      | 1     |       |       |

Support vehicles always cost 6 points. Movement, Damage and Threshold cost 1 point each.

#  

# Campaign

## Setup

Build Local mech lists

Build Local support lists

Build local salvage list

Build local elite mech pilot list.

Players build their manufacturer, or choose from a pre-made manufacturer.

Players buy their starting stable.

Players choose their starting pilots.

## Pre Battle

The Team with the lowest XP total is considered the Underdog.

Underdog rolls 3D6 and drops lowest, other player rolls 2D6. Highest total chooses the scenario type and will be on the offensive side.

Raid/Reinforce

Assault/Support

Pitched Battle

Choose to repair active mechs completely with a Technician. Choose to repair disabled mechs with the component they need. Technicians and Components are removed once used.

Players choose 1 squad of 4 mechs and 4 pilots to deploy. Any active mech can be taken. Disabled mechs cannot be taken.

If an elite pilot is used then they leave your roster after the battle.

Then repair all active mechs that will not be used. Disabled mechs become active.

Deploy the battlefield

Roll objective

Roll for Reserves

Deployment

Begin Battle

## Post Battle

### Pilot injuries

Each pilot that ejected rolls 2D6. If either dice is a 1, the pilot is injured and must miss the next battle. If both dice are 1, the pilot is dead.

### Pilot Experience

Each pilot that did not die that was involved in the mission gains 1 XP. Each player gives 1 XP to one of their opponents Pilots.

### Pilot Level Up

If the next pilot XP threshold is reached, they gain 1 Skill or a Pilot Ability, depending on the level. Opponent must observe rolls.

### Mech recovery

Roll 2D6 for each destroyed mech. If at least 1 of the dice is a 1, then the mech is seriously damaged. The second dice determines which part needs to be replaced.

Reactor, Torso, Ammo, Arm, Electronics, Leg

### Pay

Receive pay from mission. Roll one D6 for each merc pilot that participated in the battle. Winner chooses one first, then Underdog, Then alternate between Winner and Loser until there are no dice remaining. Each team can only receive a number of dice equal to the number of pilots they fielded.

### Salvage

Roll 2D6 and add 2 for each downed Reserve mech.

Chart here: Mech parts, weapon upgrades, mech upgrades, Single use tactics. Campaign specific. Upgrades come as an opportunity, which needs to be paid for below. Opportunities always have the option to take a component or money instead.

### Sell components

You can sell any components you have so you can afford the Salvage opportunity. You can also trade mech components for Technicians.

### Buy upgrades

Pay for a Salvage Opportunity and select which mech to add it to.

Components can be bought for money. See campaign price list.

Elite mech pilots can be hired from the campaign list.

### Bank it

All remaining money goes into your company savings. This money cannot be spent in this campaign.

##### MOVEMENT TYPE

|            | **Minimum Spend** | **Maximum Spend** | **Special**                  |
|------------|-------------------|-------------------|------------------------------|
| Stationary | 0                 | 0                 |                              |
| Walk       | 1                 | walk              |                              |
| Run        | walk              | run               | Turn restrictions. Gain Heat |
| Jump       | 1                 | jump              | Turning is free. Gain 2 Heat |

##### MOVEMENT COST

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 49%" />
<col style="width: 17%" />
<col style="width: 17%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th>Forward 1 hex</th>
<th>1pt</th>
<th></th>
</tr>
<tr class="odd">
<th></th>
<th>Backward 1 hex</th>
<th>2pt</th>
<th></th>
</tr>
<tr class="header">
<th></th>
<th>Turn 1 facing</th>
<th>1pt</th>
<th></th>
</tr>
<tr class="odd">
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th></th>
<th><p>Target hex is Difficult</p>
<p>eg:// trees, light buildings</p></th>
<th>+1pt</th>
<th></th>
</tr>
<tr class="odd">
<th></th>
<th>Road</th>
<th>special*</th>
<th></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

##### RANGE TABLE

| 0 (same hex) | Melee range  |
|--------------|--------------|
| 1-4          | Short Range  |
| 5-9          | Medium Range |
| 10+          | Long Range   |

##### TO-HIT MODIFIERS

|     | Target is in Obstructed hex                                                         | +1  |     |
|-----|-------------------------------------------------------------------------------------|-----|-----|
|     | Per Obstructed hex between attacker and target that is not adjacent to the attacker | +1  |     |
|     | Per Vulnerable token on the target                                                  | -2  |     |
|     | Attacker has 2 or more Heat Tokens                                                  | +1  |     |
|     | Attacker has 3 or more Heat tokens                                                  | +2  |     |

##### CRITICAL HITS

<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 22%" />
<col style="width: 61%" />
</colgroup>
<thead>
<tr class="header">
<th>1</th>
<th>Internal Hit</th>
<th>Roll again (see below)</th>
</tr>
<tr class="odd">
<th>2-3</th>
<th>Leg Hit</th>
<th><p>First hit: Half speed</p>
<p>Second hit: no move.</p></th>
</tr>
<tr class="header">
<th>4-5</th>
<th>Arm Hit</th>
<th>-1 Damage all ranges</th>
</tr>
<tr class="odd">
<th>6</th>
<th>Nothing</th>
<th></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

##### INTERNAL HITS

| 1   | Cockpit hit | Unit Destroyed.                                                                     |
|-----|-------------|-------------------------------------------------------------------------------------|
| 2   | Ammo hit    | D6 Structure damage                                                                 |
| 3-6 | Engine      | Generate 1 heat when you activate this mech. A second engine hit destroys the mech. |

##### TURN SEQUENCE

- **Initiative Phase**

  - Roll 2D6 each. Highest wins.

- **Movement Phase**

  - Initiative loser goes first, then alternate.

  - Activate mech

  - Decide movement type

  - Move mech

- **Firing Phase**

  - Initiative loser completes all mechs

  - Activate mech or clear heat

  - Select target in LoS

  - Determine damage

  - Calculate hit change

  - Roll

  - Mark damage

  - Clear heat if you decided not to shoot

- **Cleanup Phase**

  - Remove vulnerable tokens

  - Roll Critical hits

  - Remove Critical markers

  - Remove destroyed mechs

  - Shutdown mechs which have 4 Heat.

Ideas

Break Obstructed hexes into Cover and Obstruction. Cover gives a bonus if you stand in it, Obstructed if you have to shoot through it.

Cooling hex. Remove one Heat before shooting.

Slippery: Pilot check if you enter this hex while running.

Ensnaring: End your movement when you enter this hex.

Sunken: Counts as Blocking if the attacker is at medium or long range.

Sensor based set up:

Each mech has a sensor rating. Deploy defender first. You can’t deploy a mech within sensor range of enemy mechs.

Weapon Types

Missile: Ignore Obstructed hexes (except Mechs) between the attacker and target, but not the one the target or the attacker is standing in. Increase target number by 1 for all attacks.

Ballistic: Split fire against another target in the same range.

Ballistic: +1 to hit targets that are in structure

Energy: Ignore Obstructed hex target is in

Mech Abilities:

AMS: Adjacent Hexes count as Heavy Obstruction against missile weapons

Reflective Armor: +2 to hit this mech with energy weapons

Reactive Armor: +2 to hit this mech with ballistic weapons

Ignore first Ammo hit

Ignore first Leg hit

Ignore first Weapon hit

Low Profile: +2 to be hit when standing in Obstructed terrain

Internal Cockpit. Harder to eject. +1 Structure.

Pilot Abilities:

Left/Right Handed

Missile/Ballistic/Energy weapon specialization

Skill increase when Mech has exactly X structure

Skill increase when Mech has exactly X movement

Increase sensor range by 1 level

Eagle Eye: Reroll one damage dice

Acrobat: Reroll one Pilot check

Can deploy one hex closer than allowed

Checklist Master: 6+ ignore shutdown (but still drop heat)

Road Warrior: +1 move when staying on a road the whole turn.

+1 move when its the first mech to move

Ignore to hit penalty for having 2 Heat

Spend turn points to ignore a hex of difficult terrain

Weather/Terrain effects

-1 sensor ranges

+1 target number at long range

-2 skill for Pilot tests

Obstructed counts double

Difficult counts double

Shutdown if Heat at 3

Shutdown if Heat at 5

Explosives: +2 movement to enter a given tile type

Mech Design upgrades

Costs:

- 1 point of damage in your lowest band

- 1 structure point

- Arc reduction

Purchase

- +1 sensor range

- \+ weapon special

- \+ mech special

- +1 melee damage

- +1 structure point
