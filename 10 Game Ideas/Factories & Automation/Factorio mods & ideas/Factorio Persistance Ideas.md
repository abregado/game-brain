---
title: "Factorio Persistance Ideas"
source: "Game Stuff/Game Ideas/Factorio Persistance Ideas"
modified: 2017-02-21
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Factorio mods & ideas]]", "[[Living World PvE]]"]
concepts: ["Factorio mods / ideas", "Factorio Persistent World", "Living World PvE"]
words: 652
summary: "Design constraints and solutions for turning Factorio into a persistent multiplayer world: clone vats, tech archives, evolution decay, unlimited resources, trees regrowing, rocket launch as difficulty spike."
tags: ["area/game-idea", "project/factorio-mods-ideas", "project/living-world-pve", "type/design-doc"]
---

Constraints of a Persistent game world

- The map should never need to be regenerated

- All player impact must be removable

- No permanent bonuses should exist

- No fixed goals (do X) instead use temporal goals (do X for N length)

- Everything needs to be linked to an area of the gamestate than can be affected in both directions (creation/destruction).

- Play drivers must be created which are worth while in a persistent environment

- Players need to be incentivized to play

- Players need to be able to leave for 24 hours at least

List all of the Perma changes in Factorio

- Can't “unlaunch” a rocket ([*solution*](#make-rocket-launch-difficulty-increase-rather-than-end-game))

- Technologies are irreversible ([*solution*](#archives))

- Biter Evolution only goes up ([*solution*](#new-biter-evolution))

- Resources are depleted and never come back ([*solution*](#unlimited-resources))

- Trees are removed and never come back ([*solution-1*](#trees-are-not-a-resource-for-harvesting)) ([*solution-2*](#trees-grow-back))

- Landfill …

- Biter bases are not actively replenished

- Player structures are not targeted if left alone

Current Player drivers

- Research all technology

- Launch a Rocket

- Do one of those faster

- Achievements

Bens list of “Things my instinct tells me it should do”

- Return to clean state after 168 hours of inactivity

- Scatter new players across a large area

- When played actively, reach a state of equilibrium that can only be countered by hiring more players.

- Be impossible to stay at equilibrium without human intervention

- Include more “in world solutions” rather than more UI

Other foreseen problems

- Biters dont act, they react

- In multiplayer: There is no failstate, just setbacks

- Biter density reaching 100%

- Biter density reaching 0%

- Only one starting area

- Player griefing

- No way for players to reset their spawnpoints ([*solution*](#clone-vats))

- No way for players to choose to join one another

- 

# Solutions

### Clone Vats

Player built structures which a player can link to. These cannot be deconstructed once linked, but may be destroyed. Players return here when they die. If they are destroyed then players will be randomly placed in the world with no equipment.

### Archives

A structure to store finished tech. When a tech is finished, one of the Archive buildings becomes un-minable. This tech is now linked to the Archive. If the Archive is destroyed then the tech becomes unresearched.

### New Biter Evolution

Biter evolution only goes up when killing bases, and over time goes down is no bases have been killed recently.

- NEW PROBLEM: Need to make culling of bases selectively part of the gameplay again, otherwise players will just avoid all bases.

### Unlimited Resources

Resources never deplete and can be mined indefinatley

- NEW PROBLEM: Players do not have to expand very much to get massive throughput ([*solution*](#limited-minable-patches))

### Limited Minable patches

Using collision boxes, make the number of placeable miners, and theirfore the output of material, limited.

### Trees are not a resource for harvesting

Trees remain minable but do not give resources (damn unburnable alien trees). Now their only value is in letting them stay standing. Recipes that need wood need to be swapped to something else (iron or stone).

### Trees grow back

Using a chunk tile updater script, find a random tile in every chunk. If that tile is ‘alien grass’ then check how many tree entities are in range. If there are enough then place a new tree here. Use extra biomes to create “intermediate zones”.

### Make rocket launch ‘difficulty increase’ rather than ‘end game’

When launching a rocket, have this trigger a massive spike in pollution, aggression and evolution. Surviving after a rocket launch for as long as possible should be the goal of players. More rocket launches should mean more “cred” to those players. Attribute a launch to all players who were online at the launch, and remove the launch if all those players have lost their clone huts.
