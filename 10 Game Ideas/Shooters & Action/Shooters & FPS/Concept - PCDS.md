---
title: "Concept - PCDS"
source: "Game Stuff/Game Ideas/Concept Docs/Concept - PCDS"
modified: 2018-07-09
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Shooters & FPS]]"]
concepts: ["Persistent Character Deathmatch Shooter", "Design: Persistent World Economy"]
words: 1676
summary: "Concept doc for Persistent Character Deathmatch Shooter: wagering respawns/ammo/charges, permadeath characters on player-run servers, post-match reward packs, complex damage model, server options."
tags: ["area/game-idea", "project/shooters-fps", "type/design-doc"]
---

Concept

Persistent Character Deathmatch Shooter

Drafted by Ben Buckton

### Description

This is an attempt to create a multiplayer deathmatch shooter with persistent characters that relies on player skill, prematch tactics, wagering of resources, has no experience leveling and has a complex non-realistic damage system.

As players start a match they select which of their equipment they would like to use in battle as well as how much ammunition to bring. Each loadout is limited to two weapons, several miscelaneous equipment items and a set of armor. Each item with an active ability has limited uses (charges) similar to weapon ammunition. Ammunition has effects just as the weapons do, so bringing the correct types is as important as anything else. Players must also select how many “respawns” to bring to the match. Excess ammunition, respawns and charges are discarded at the end of the match, and if a player runs out of respawns he loses every item that was brought to the match.

Characters are stored on the FPS dedicated server. These servers are run by players, or can be rented from common server rental companies. Since matches and post-battle are happening on the same server, players will most likely wait in a queue to fight and then complete postbattle while others are fighting.

### Goal

- To create a fast paced deathmatch combat system

- To have many viable options for loadouts with minimal overall items

- Create an environment where information is as effective a weapon as a rifle

- Players must bring just the right amount of gear for each encounter

- Charcter advancement is separate from victory

- Players who disadvantage themselves advance faster

- All players in a match spend/advance together afterwards (post-battle)

- Limited supply forces players to think twice before bringing their best gear

### Features

The in match component of this game has some unique features:

- Respawn wagering

- Ammunition and Charge wagering

- Active defence items

- No weapon/armor pickups during the match

- Loose locked targetting

- Three levels of weapon heavyness (pistol, carbine and heavy)

- Three levels of movement related to the weapon classes

- dodging, aerial manuvers using vectored thrust

- Complex damage model (size, resistance, reduction, penetration, splash, contact area)

- interactive level elements (traps, doors, platforms, jumppads)

- collecting information on your opponents loadouts has priority

- Suit cameras and sensors shown in PIP windows

- players select loadouts before fighting

- Guild/Killteam shared equipment

- equipment and ammunition combinations create different game effects

- Loot rewards for completing in-match challenges

- Loot rewards for particular killshots

- Recycling of unwanted equipment into ammunition for desired items

- no minefield of crap items. Only effective items

User Experience

Server Browser

After loading the game, players join a server using the browser. The server identifies the users name and password, providing their client with the saved character data for that account. Since characters are not transferrable between servers, a Favorites list should be made available to players.

Pre-match

Once connected to the server, players can:

- watch the current match

- view a friends list

- modify loadouts and view their equipment

- purchase new equipment

- recycle old equipment into ammunition

- see a list of upcoming matches

- request a certain type of match

- mark themselves as available for a match

When no matches are queued the players options for requesting a new one include:

- Respawn multipler (x10, x5, x3, x1, x0) (smaller multiplier gives more reward)

- Round Length (longer rounds give more reward)

- Team size (or Free-for-all)

- Number of teams

- Killteam match?

- Map

If there are upcoming matches with free places, the player can simply mark himself as available and when the next available match begins they will be prompted to join. Players are locked into the match just half way through the previous match. Joinging a match also means they will not be available for the immediate next match as they will be in the Post Battle segment of the their game.

Once the match is full, or all players vote to begin anyway, the loadout screen appears. Players can select from the following options:

- Which pre-configured loadout they will use

- How many respawn tokens to take into the battle

- How many charges for each item they will have for the whole match

- How much ammunition they will have for the whole round, per weapon

- Which types of ammunition and charges their items will be loaded with

After all players have locked in their setups, the match begins.

Match

The match begins and all locked in players can participate. The match itself plays much like a classic deathmatch shooter. Players deal damage to eachother until they “die”. The player (or team) with the most “frags” at the end of the round timer, wins.

That is where the similarities end. Each player can only respawn a fixed number of times. This number is equal to the amount of respawn tokens brought times by the “respawn multiplier” of the match.

Ammunition and charges are used throughout the match. Respawning does not cause ammunition or charges to be discarded. However, at the end of the match, all unused ammunition, charges and respawns are discarded completely.

If a player runs out of respawns and is killed again, his character is killed. This effectively deletes the character from the server (except for his placements in the high score charts). The player must begin with a fresh character on this server.

Players also earn extra rewards for utilizaing special locations in the map, and for killing their opponents in unique ways. Some of these include

- Fraggin someone in sight of a camera, or in special killzones

- Fraggin with melee attacks

- bring the first to frag with a certain weapon

- permadeathing a character

- camping on undefensible positions (resource locations)

- never using advantagous positions

- headshots

- wall running

- use of dodging

- use of jetpacks

- making frags while the target is effected by de-buffs

- sneak attacks

- using jumppads

- modifying the level

- placing traps, effectors, zones

- staying stationary for a long time

- ammunition efficency

- pushing characters into damaging zones

Post-match

Once the timer is over, the remaining characters may chose their rewards. A number of different rewards are generated for each field of acheivement. Players who performed best in each field get to pick first from rewards in that field. The winner gets to select from one of two prize packs.

The amount in each of these reward categories is based on how active the players were in that category. The total reward is divided into a number of Reward Packs equal to the number of remaining players. The first pack contains 25% of the total reward pool for that category, then the next has 25% of the remaining pool.

The total Reward Pool is based on:

- Total equipment brought into the match

- Amount of equipment lost to permadeath

- Amount of ammunition, charges and respawns wagered

- Respawn Multiplier of the match

- Match length

Players who have short matches with many respawns will get very little reward. In these matches, players will have to wager very little to make ends meet and because the Reward Poll is calculated from the total used, wagering a lot increases the rewards your opponents get as much as they increase yours.

Matches with the opposite generate much greater reward, for those who survive. Long matches, even those where the respawn multipler is high, run the risk of working players down to zero ammunition.

Reward Packs should include a mixture of items, ammunition and respawns so that there is always an element of choice between packs even when each pack contains more “wealth” than the next.

Once all packs have been chosen (surviving players should get a choice in each category). Players are taken to their loadout screens to select which items to replace with the new gear, and which ones to break down into ammunition. Players can only store two loadouts at a time, so must decide carefully which items to keep. Items may be moved between loadouts before any match.

Backend

The dedicated server must be able to run the current match, reward generation and post-battle for a large group of players. Limiting the game to a maximum of 16 players gives a good spread of team variants (16FFA, 3v3v3v3v3, 4v4v4v4, 5v5v5, 8v8). Larger maps could be made to support more players, but it shouldnt be nessesary. With the maximum I game set at 16, and a one match downtime for each player, there could be up to 48 players connected to the dedicated server at any time. By modern standards this is not a great deal. Creating a server that can support a scaling number of concurrent client connections should not be too difficult, as idling players will not make many calls.

Several tools should be made available to server admins. Character information should include timestamps so that admins know when a player has logged in last, as well and creation date and when the last match was played. Keeping an active player base will be essential, and we as the developers should help the admins achieve it.

2018: I don't know if this is a good idea anymore. Refer Eco and how server operators create games with massive xp multiplier.

The server options should include several relating to the game economy. Some servers may want a slow buildup for their characters, or maybe they want to increase the risk that players must take. Customization options should exist for:

- Respawn multipler

- maximum and minimum match length

- minimum/maximum ammunition and charge wagers

- minimum/maximum respawns usable per match

- Overall Reward multiplier

- maximum economy wealth

- self regulation of item rareness (items with no iterations are spawned first)

- doubling reduction (so players cannot have two of the same item)

Engine

Platform

Server
