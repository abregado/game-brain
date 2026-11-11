---
title: "BS - Sci-fi Dungeon Crawler"
source: "Game Stuff/Game Ideas/BS - Sci-fi Dungeon Crawler"
modified: 2024-09-09
type: design-doc
area: wargame
status: "idea"
projects: ["[[Dungeon Crawlers]]"]
concepts: ["Sci-fi Dungeon Crawler", "Design: Activation Dice", "Design: Campaign Lists Progression"]
words: 1620
summary: "Design notes for a cooperative sci-fi tabletop skirmish/dungeon crawler: problems with wargames, desired features, mission tables, reactions and fatigue, post-battle locations, saturation tokens, unit traits and setup cards."
tags: ["area/wargame", "project/dungeon-crawlers", "type/design-doc"]
---

## What is the problem?

Rules should not be about selling books. Rules updates should happen when the game needs them, not when money needs to be made.

Tabletop Wargames are not cooperative.

Tabletop Wargames are not narrative.

All armies in a tabletop wargame function very similarly. Controlling Tyranids does not feel mechanically different from controlling Space Marines.

No progression, or unbounded progression. The sweet spot needs to be found.

Player downtime during monster round.

One-two round slow start in most games.

## What do I want?

Increasing danger as time goes on

Hot start

Party build strategy

Players incentivised to play fast

Tight mapping (small amount of area, only the important bits)

Shootouts down corridors or across rooms

Players power up by playing adversaries and challenges

Terrain effects

Reasons to split the party

Content packs add on top

Players should feel heroic

Enemies should feel deadly

Combat cannot be deadly

## Rolls to design mission

Players rolls on a number of tables to determine what the mission will be. Rolling the same as last time allows them to choose which they want to do this time.

| Roll | Mission Type    | Owner     | Opponent   | Complication     |
|------|-----------------|-----------|------------|------------------|
| 1    | Salvage         | Us!       | Xenomorphs | Time limit       |
| 2    | Repair          | Marines   | Marines    | Limited Access   |
| 3    | Rescue          | Syndicate | Syndicate  | Uncooperative AI |
| 4    | Black Box       | Robots    | Robots     | Life Support     |
| 5    | Demolish        | Psychics  | Psychics   | Gravity          |
| 6    | Boarding Action | Hightechs | Hightechs  | Radiation        |

Then the players choose which items they will take with them, and where they will begin. Generally the mission begins with everyone already in place to complete the mission.

## Players react and interrupt

Enemies and Challenges take their turns one after the other. As each appears, players can say they will react to them. Every time they react, they gain a Fatigue token. At the end of the turn they lose a number of Fatigue tokens. Having too many is bad.

Example reactions:

Move

Reaction Fire

Engage

Counter

Attempt Solution

## Post Battle location

After a mission, the team decides which location it will visit. It cannot visit the same location as it did last time. Certain locations are better to visit after others. Each location has facilities.

Example Facilities: Shops, Bars, Quest Locations, Shipyard, Drydock, Commodities Market, Underworld locations, Laboratories, Hotels, Resorts.

Not all locations have all facilities. Which facilities you need might change during a mission, altering your plans.

Each player gets two post battle actions. They must choose both actions before rolling for any outcomes.

## Activation dice

This is a reasonable solution. It:

- Signals to the player how many actions they have

- Signals how much risk they should take this turn

- Allows the players to plan together

- Provides unexpected difficulties (they know what they want to do but can't this round)

- Gives another axis for balancing actions.

## Solving the slow start.

Replace the first two turns with a setup round, where players see the entire challenge and then modify things to make it easier. Players start where they need to be to solve the problem. The enemies that spawn add chaos to that process.

## Solving the progression accountability

Lists exist in one campaign. The campaign is written on the list. Every player is responsible for checking the progress of their opponent.

Lists do not get transferred between campaigns. Lists can only be created in a campaign.

## Solving the temporal unfairness within a campaign 

All missions involve using less than maximum units or points. Only units put at risk can advance.

## Quest and Story Tables

D6 tables. The more players that Explore the post battle location the better. Each rolls a D6. Any player that rolls a number the same as another player can choose their result instead. Each result can only happen once.

| Roll | First Visit (always gives Key) | Second Visit            | Third Visit               | Fourth Visit                    |
|------|--------------------------------|-------------------------|---------------------------|---------------------------------|
| 1    | Trap                           | Scam                    | Robbed                    | Trade keys to avoid bad Outcome |
| 2    | Possible Trap                  | Trade key to avoid Scam | Trade key to avoid Robbed | Trade key to avoid Attacked     |
| 3    | Possible Trap or Bonus         | Possible gain key       | Gain Key                  | Sell Keys                       |
| 4    | Possible Bonus                 | Gain Key                | Trade key for Bonus       | Trade keys for OK Outcome       |
| 5    | Paid Good Bonus                | Trade key for Bonus     | Trade key for Bonus       | Trade keys for Good Outcome     |
| 6    | Bonus                          | Trade key for Bonus     | Trade key for Bonus       | Trade keys for Best Outcome     |

Possible outcomes

Trap, Scam, Robbed or Attacked

Banned from location for 1 extra mission

Limit actions next time you return here

Random bonuses for next mission

Mission setup rerolls

Forced setup options on next mission

Rerolls

Opportunities for cheap item

Consumable supplies

Permanent stat buffs

New downtime locations open up

New downtime actions become available

Cover: Roll an extra dice then discard your highest dice

6’s cause critical damage (no defence)

Saturated Token. Enemies do not move through saturated areas. 1 extra red dice per Saturated Token. Remove at end of turn. Units in a Saturated area at the end of the turn take 1 defence roll. If a unit leaves an area with a Saturation token, it takes a defence roll.

When to place Saturated markers? Every hit? Every kill? Every shooting attack?

Heroes

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr class="header">
<th>4 activation dice</th>
<th>4 activation dice</th>
<th>4 activation dice</th>
<th>4 activation dice</th>
</tr>
<tr class="odd">
<th><p>Reactions:</p>
<p>1+ Melee Strike (1 blue)</p>
<p>2+ Shooting Strike</p>
<p>(1 grey)</p></th>
<th><p>Reactions:</p>
<p>2+ Claw (2 grey)</p>
<p>6+ Saturation Fire (blue) Add extra Saturation Token</p></th>
<th></th>
<th></th>
</tr>
<tr class="header">
<th><p>Actions</p>
<p>3+ Sniper (1 pink)</p>
<p>6+ Sniper (2 blue)</p>
<p>3+ Move 3</p>
<p>5+ Blink 2 Ignore Saturated and Enemies</p></th>
<th><p>Actions</p>
<p>5+ Gatling (pink x2)</p>
<p>4+ Power smash (blue) Hit last</p>
<p>4+ Power Grab (pink) Restrain enemy if not dead</p></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

Wack-a-mole: After taking damage a unit can ignore the damage by moving one area away, unless it is in a saturated area.

Self Preservation Override: This unit ignores Saturation Tokens for the purposes of movement.

Regeneration: If this unit does not change areas, and there is no Saturation Token present, one wound is removed.

Acid Blood: When this unit dies an acid token is placed in the area. These act like Saturation tokens and are removed last.

Chitinous Exoskeleton: This unit is immune to Acid tokens.

Dying Scream: When this unit dies, another of the same type spawns at the end of the round.

Normal Actions

1+ Move 1

1+ Fallback 1 (reaction)

5+ Commit to Hex progress

Big Shooty Bad Def 3+, Qual 3+, M 2, A3, W2

1+ Cover and Shoot

2+ Charge and Shoot

6+ Charge double

**Self Preservation Override:** This unit ignores Saturation Tokens for the purposes of movement.

**Regeneration:** If this unit does not change areas, and there is no Saturation Token present, one wound is removed.

Shooty Bads, Def 5+, Def 5+, M3, A1

1+ Cover and Shoot

5+ Advance

6+ Overwatch

**Take Cover!:** After taking damage a unit can ignore the damage by moving one area away, unless it is in a saturated area.

Choppy Bads.m

1+ Hide

3+ Charge

Area Effects

Cluttered: Units here always count as being in cover. Movement stops when entering or exiting this area

Blocked: Something heavy is in this space. Units may not enter the space.

Exposed Equipment: Adding any number of Saturation Markers here adds an extra one.

Shipwide Effects:

No Gravity

No Atmosphere

Debris Clouds

Setup cards

Forced entry: a character with this card can begin in a room that is inaccessible, but the room gains the Vacuum trait.

Welder: one sealed door can be made unsealed or one unsealed door can become sealed.

Cleaning disintegration: one area with Cluttered loses the state.

Seal Plate: remove one Hull Breach or Open Vent marker.

Weld wedge: one door is permanently open

Shaped Charge: Add a Hull Breach token.

Portagen: the room where this is placed is considered powered.

**Maybe each equipment card has a setup and/or a game use part. Powerful in game cards like weapons and armor could have no setup bonus. Different characters could have different amounts of equipment at mission begin, or gain the ability to use some abilities multiple times.**

Repair mission could be harder because you need to use more equipment slots on setup items.

If a mission has the same ship type as it has aggressor, then there are different events. The aggressors are trying to recover the ship without damaging it. If the aggressor and ship type are different then the aggressors are a pirate crew from that faction or military that does not care about the ship.

When ship gravity is disabled:

Cluttered tokens become Debris tokens

When ship gravity is enabled:

Fragile cargo tokens become cluttered tokens

Explosive cargo explodes

Debris tokens become cluttered tokens

Unsealed Doors can be activated for free if there is power. Otherwise they require an activation die to change state.

Rooms are powered or not. Each room has a power network token to show which network it is on.

Generators have tokens to show which networks they are powering. Each generator has a number of slots for network tokens.

Apart from setup cards, players can change the state of something just by spawning next to it. So if you want to change the state of the reactor in setup, you can do so with a card or by starting in it's area.
