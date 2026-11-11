---
title: "Project - Living World PvE"
source: "Game Stuff/Game Ideas/Big Five/Living World PvE/Project - Living World PvE"
modified: 2019-11-29
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Living World PvE]]"]
concepts: ["Living World PvE", "Design: Combat Stamina and Gradient Falloff", "Design: Evolutionary Enemy AI", "Design: Weight Classes", "Design: AI Self Preservation"]
words: 3260
summary: "Design doc for a cooperative PvE game where a single evolving AI (Von Neumann machines guarding a planet) runs bases, camps, patrols and state-machine behaviours that mutate based on how long bases survive. Includes combat concepts (everything limited, gradient falloff, weight classes, AI self-preservation) and an entity list for a prototype."
tags: ["area/game-idea", "project/living-world-pve", "type/design-doc"]
---

## 

## 

Living World PvE

A concept by Ben Buckton

“I would prefer to have a game with 100 people playing together, than 10 million people ignoring each other” - Ben Buckton, 2014

> [*High Level Concept*](#high-level-concept)
>
> [*PvE spawns Ideas - Living World, a rough concept*](#pve-spawns-ideas---living-world-a-rough-concept)
>
> [*Notes*](#notes)
>
> [*NPC Base Behavior States*](#npc-base-behavior-states)
>
> [*Exploration*](#exploration)
>
> [*Expansion*](#expansion)
>
> [*Outer Defence*](#outer-defence)
>
> [*Local Offense*](#local-offense)
>
> [*Inner Defence*](#inner-defence)
>
> [*Digital Torpor*](#digital-torpor)
>
> [*Destruction of a Base*](#destruction-of-a-base)
>
> [*AI Variables (possible)*](#ai-variables-possible)
>
> [*Player Weapon systems*](#player-weapon-systems)
>
> [*To make the above content system*](#to-make-the-above-content-system)

[*Combat Notes (how to make the combat strategic AND tactical*](#combat-notes-how-to-make-the-combat-strategic-and-tactical)

> [*Combat Concept: Everything Limited*](#combat-concept-everything-limited)
>
> [*Combat Concept: Gradient Functionality Falloff*](#combat-concept-gradient-functionality-falloff)
>
> [*Combat Concept: Short Engagements*](#combat-concept-short-engagements)
>
> [*Combat Concept: AI Self Preservation*](#combat-concept-ai-self-preservation)
>
> [*Combat Concept: Weight Classes*](#combat-concept-weight-classes)
>
> [*Bloat Features and other crazy ideas*](#bloat-features-and-other-crazy-ideas)

##  

## 

## High Level Concept

Humanity sent out Von Neumann machines into the interstellar void with one directive. If you find a suitable planet for humanity, protect it for us. A planet was found and now we have arrived. The Machines recognize us as humans and will not harm us, but they also refuse to allow us to exploit the surface of the planet. Now we must take the planet back from those we programmed to protect it, and it is not going to be easy!

## PvE spawns Ideas - Living World, a rough concept

To make a good PvE game, where all the players want to cooperate we need to create an enemy that everyone can work against that reacts to the players, is interesting to fight AND that is difficult.

The whole game world is controlled by a single AI that will literally evolve different strategies and implement the ones that are most effective against the players.

Base spawners on map generate NPC mobs. These mobs move out to occupy other areas of the map.

Once they arrive they set up a “camp”. These camp areas are marked on the map. Players entering that area will be aggressed.

Camps in newbie areas should be far enough apart that players can avoid them.

Once cleared, a camp will be removed but a new spawn will be created (after a short interval) at a nearby base spawner and begin moving back to the camp.

Some enemies are also on patrol, and will agress anyone they encounter (moving camp areas shown). These will complete circuits of the map and return to the base.

If outgunned, enemies should retreat to their base. This should force players to attempt spawns of their own level.

Attacking the base spawners will make them spawn much faster for a period of time after the attack. The more damage inflicted to the base, the longer the period of time and the more aggressive the spawns. If destroyed then there will be no spawns for a period of time.

Keeping an area free of NPCs to make it safe for non-combat operations will require repeat combat incursions and also combat sweeps.

With several based covering the most lucrative resource fields, a lot will be invested by the players to keep areas clear.

Players could also mark areas for NPC bounties. Other players making kills in these areas will be rewarded with the bounties.

make sure camp locations match up with rich resource areas

NPCs might also send out transports to these camps to collect resources. They might be guarded or undefended, and players could attack them to get the rewards (and it would aggravate the spawn level).

Bases of different levels exist so that groups consisting of different player levels could take part in this content.

Anti-big guy weaponry could be used to make bases that only newer players can attack, or older players with specialist small equipment

## Notes

All Complex AI is controlled by Base entities. NPC units get given orders to complete at creation, and continue to repeat them until they return to base.

NPC units are formed into Squads which control their “Combat Behavior” when engaged with the player. Squads are the smallest entity with Behaviors. This should limit the amount of server time spent on pathfinding and ai.

Squads get their “Combat Behavior” from their base “AI Template” when they are spawned. It does not change until they return to the base.

## 

## 

## 

##  

## NPC Base Behavior States

### Exploration

This state is in play when the Base has less camps set up than its desired amount. The Base will spawn NPC Patrol Squads and assign them routes to take throughout the game world. As they move around these squads will collect data on the area such as Resource Wealth, other base activities and player activities. When the squads return to the base, the base information profile (what it can see) is updated. These squads will not agress players but will move in close to unguarded Non-Combat players and scan the area for resources. If there are players there, there is probably also resources. The Patrols are fast, light NPCs that will fight a fleeing battle if engaged. Their Primary mission is to collect data and return to the Base. If damaged they will cut their patrol short and return to base.

100% of spawns will be Patrol Squads

### Expansion

Once the base has detected some quality locations for camps to be set up, It will begin spawning Camp Squads. These squads are aggressive only if attacked and will move out to set occupy areas of high resource value. Once set up, they will attack any players moving within a set range, and will return fire. The longer they stay, the more reinforcements they will request from the base.

Bases will still spawn Patrols during this time, but the ratio should drop to 30% Patrols, 60% Camp Squads and 30% Reinforcement (once a single camp is set up)

A Base will revert to Expansion when its number of Bases drops below its Minimum Bases Variable.

### Outer Defence

This state is in play when the Base has filled its camp quota or can detect no more camps within range (generally it will fill up the slots with crappy spots). Patrol Squads will no longer spawn, instead Combat Squads will spawn and begin patrolling between camps. Camp aggression areas will increase in size and spawns will be split between Reinforcements and Patrols 50/50. If a camp comes under attack, then nearby combat patrols will close in to reinforce the area, moving to the closest camp if there are multiple under attack. When a camp is under attack, 100% of spawns are dedicated to reinforcing that camp.

Combat Patrols will not stray too far from their routes to engage players, opting more to chase them away than to destroy them.

If a camp is depopulated of NPCs and stays depopulated for 1 hour, then the camp is considered destroyed.

### Local Offense

If no camps are under attack and player activity is recorded in an area, then a base will switch to this state. This state is only accessible from Outer Defence and will trigger after no player aggression has been detected for a set time (Patience Variable). Combat Patrols will track players for longer periods of time and agro from longer range.

When attacking player groups, NPCs will attempt to pull back when damaged, and will only continue to agro if a percentage of their squad is still fighting. Any squad that successfully withdraws will collect more squad members before attacking again.

### Inner Defence

If the base itself comes under attack, then it will override ALL states with this one. It will spawn only defensive NPCs. These will be slow but powerful. Also its current Threat Variable will rise over time while players are in the vicinity AND also exponentially based on how much damage is suffered. A portion of nearby Combat Patrols will be recalled to assist with the defense. Combat Patrols already in combat, but not near to the base will retreat to either the nearest camp or the base itself.

This state will continue until all players have left the area (or been removed) and then for a period of time afterwards (Paranoia Variable). The base will then revert to normal states but its Threat Variable will slowly go down over the period of 24 hours. This means that the other states will be much more active than usual and if Local Offense is triggered, players may find the area difficult to survive in.

The slow moving NPCs are either assigned to nearby camps or recycled into other NPC types.

### Digital Torpor

The AI construct in the game only wishes to survive forever. So, if it detects no threats for longer than a week it will shut down its operations. It will construct detector posts at all of its Camps, then withdraw units to the base. These detector posts are alarm bells that will trigger the reawakening of the AI if players move within range.

New bases that are discovered begin in this state. Once players move within a certain (large) range then the AI will wake up and proceed with its normal programming.

This means players can explore new areas, and if they are very careful can survey for resources without bothering the local AI. If an AI base is attacked while in this state it will obviously immediately switch to Inner Defence mode, but will be at a significant disadvantage. This also means that it is easier for players to clear building space behind enemy lines, at the obvious disadvantage of safe supply lines.

## Destruction of a Base

If a base is successfully destroyed then it will be inactive for a period of time. Also its variable AI parameters are stored in a list, along with how long the base stayed alive, how many NPCs it lost and how many players it killed. At the point when it itself respawns, a new set of AI parameters is selected, weighted toward AI sets that survived the longest. Then random “mutation” of the parameters takes place. Eventually the AI will adjust to whichever causes the players not to destroy the base, aka “living in harmony”. If there were different AI “factions” then each could have a different variable for “success”. One might be interested in efficency (NPCs used per Player kill), one might be interested in blocking resources (Player resources aquired per time), or perhaps simply “Most area covered”.

When a base is created is also when the AI is set for every NPC it spawns, the common patrol paths and which resources it values most. These all get stored in the AI profile and can come back again with the next reroll.

This behavior may cause AI that causes the least trouble for the players to become more prevalent. If the players can somehow stop other players from destroying bases then they could also allow weak AI to survive longer to stunt its evolution.

## AI Variables (possible)

Each AI has many many variables that control how it behaves. The more variables the better, as the system of AI respawning and mutation should sort out which ones are more valuable. Examples could include: Reaction Time to (attacks/player proximity/active scanning/mining/combat), Focus on NPC stat (speed, toughness, terrain immunity, effects, damage), squad min/max size, Combat/Industrial focus, Spawn % (scout/reinforce/combat/patrol/def/industry), Patience (time before it gets bored and attacks), Agression radius modifer, Camp quantities, Preferred camp reinforcement level, min/max distance between camps. The list can go on forever. Any system should be written so that new variables can be added in at the devs whim, and so that new values can be seeded out to all AIs at a base level.

## Player Weapon systems

See the [*document located here.*](https://docs.google.com/document/d/1fVL2H7b0TJteyTQpduF4KJSULw75jtixsRaen8FDwrQ/edit?usp=sharing)

###  

## To make the above content system

We will need to following entities, variables and behaviors

- Base Spawner

  - spawn types

  - max number of spawns

  - desired locations

  - spawn cooldown

  - base health

  - which spawns come at which stages of damage

  - radius of aggression

  - resources available for collection

  - Behavior - check camps for collection

  - Behavior - check camps for reinforcements

  - Behavior - check desired locations for action

  - Behavior - sent squad to location

  - Behavior - spawn new squad

- Spawn (NPC squad)

  - array of NPCs

  - base spawner it belongs to

  - destinations

  - aggressive or not (will always return fire)

  - Behavior - move towards destination

- NPC Camp (squad becomes camp once it reaches destination)

  - reinforcement timer

  - base spawner to call reinforcements from

  - desired NPCs

  - radius of aggression

  - resources available for collection

- Important Locations

  - generated static or dynamic

  - based on what?

- Pathing nodes

  - generated static or dynamic

  - tile based or discrete fine resolution?

- NPC entity

  - speed, range, team, ect

- Terrain system - nothing to begin with then:

  - player cannot cross (exterior mission area zone)

  - NPC cannot cross (player zone)

  - both cannot cross or shoot (forest)

  - both can shoot across, but not move (chasm)

  - both can move across but not shoot (shrubland)

  - both can move with large units across and shoot with all across (light forest)

  - both can move with small units across and shoot with all across (marsh)

- Player interaction

  - click to place “players” on the map

  - players will damage NPCs around them

  - players will be damaged by NPCs around them

  - simple test cases to see how the AI reacts

  - 

# Combat Notes (how to make the combat strategic AND tactical

Players want to shoot and destroy targets. The long term goal of this game would be for the players to build up enough resources to be able to take out “all” the enemy bases. To make it into a persistent game, simply add more and more enemy bases in increasingly higher densities.

We should also offer the players a range of “weight classes” to pilot. Every player is different, some like fast nimble craft, others like slow plodding death dealers.

The overall gameplay should not be about destruction, but forcing the enemy to retreat. Holding ground should be more important than total destruction. How can we achieve this?

Speed is directly related to damaging dealing capacity. If something is fast, it should not be able to defeat something that cant run away from it. Faster targets should always get the ability to withdraw to be saved for another day. Larger targets will withdraw earlier if they are outnumbered, not blindly throw themselves into battle.

Eventually player groups will be large enough that a squadron of faster craft could chasedown fleeing heavier targets. To counter this, the game would have to have limited ammunition/combat duration. Players should not blindly chase down every target, when holding the valuable ground is more important (or if they do, it should not be optimal).

To keep combat interesting and heated, the enemies should deploy mobile repair/rearm bases nearer to the player occupied area. Then their attackers can perform hit and run attacks and eventually whittle the players down, unless they are supported by other players.

Larger craft should have more firepower, but exponentially more staying power(ammunition/combat duration).

Attacking bases should make things WORSE for the players unless they are successful, and then it will be better only for a short period of time.

## Combat Concept: Everything Limited

Every weapon and ability has a limited number of charges before the craft needs to return to refuel/rearm/reload. The period when functionality starts to drop off should be long so the player can decide when to turn back. Different types of craft with more or less “Combat Stamina” should be available to suit different players with different Play Session Times. Someone who is looking for a 20 minute bash would select something that runs hot, fast and runs out of ammunition quickly.

## Combat Concept: Gradient Functionality Falloff

The efficiency of a player craft should diminish slowly over time. As weapons start to run out of ammunition they should also diminish in efficiency. This is so that the agency of the player is not a boolean state. The longer a player plays, the more he should have to think before engaging in a combat. The speed of this effect can be balanced with what we find to be the normal Play Session length. Different craft should have different rates of functionality falloff. Damage should also have an gradient effect on functionality, rather than eventually just disabling one system entirely.

## Combat Concept: Short Engagements

Combat engagements should never be “until the death”. Players should always be considering “could I use this ammunition later/elsewhere” and when their quarry begins to flee they should have a really good reason for chasing the enemy down. Also, considering when to withdraw temporarily to rearm should be an important element.

## Combat Concept: AI Self Preservation

Enemies in most games are stupid. The throw themselves against the player with no thought of their own survival. In this game, it is different. Enemy units build up at a fixed rate. They attempt to flee combat when they are too damaged or ineffective. If enough of them survive, the return with greater number in the next wave.

As they retreat, other friendly forces move up to cover them. Damaged units are shepherded back to be repaired. Players who foolishly attempt to chase down fleeing units might get caught by more enemies.

## Combat Concept: Weight Classes

Not a new idea, but a good one. Each craft falls into one of several weight classes. Smaller, Lighter craft would have less staying power but could continue to harrass fleeing targets. Heavier craft would be slower, and therefore unable to escape smaller craft but would be able to outlast them in terms of toughness and “Combat Stamina”

### Bloat Features and other crazy ideas

When bases are under attack, Devs can log in and designate target priority manually, to give the feeling that the AI is generating new strategies. They cannot tell the AI exactly what to attack, or how to do it however.

New AI bases are constructed from nearby bases and use their “AI Parameter seed” to generate the new seed. This means that new AI is always a mutation of currently successful AI, and may lead to the players “Domesticating” the AI planetwide but destroying problematic AI and allowing weak, easy to avoid AI to take over.

AI could share knowledge of “success” and breed new AI Parameter Sets by combining their variables. Each AI faction could have variables it deems as Dominant that are always passed on.

Primary and Secondary variables. The Primary variables change but the Secondary Variables are based on the Primary ones.

AI consider their success level based on a minium of two critera. An agressive environmentalist AI might consider success to be most players killed per resource consumed. An efficent disruptor AI might consider the number of resources players harvested against the number of NPCs used.

Scout behavior.

Select a point in sight that can be reached directly, test that it is farther from the start than the current location.

Repeat until travel distance is higher than the return value.

Repeat the same except the point must be closer to the start, prefer points not near existing points.

Once returned, this path is added to known paths and locations
