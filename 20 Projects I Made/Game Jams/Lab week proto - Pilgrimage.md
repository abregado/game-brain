---
title: "Lab week proto - Pilgrimage"
source: "Game Stuff/Lab week proto - Pilgrimage"
modified: 2023-12-04
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Game Jams]]"]
concepts: ["Pilgrimage", "Design: Multiplayer Netcode"]
words: 755
summary: "Design for Pilgrimage, a minimalist multiplayer stone-voting game in Unity with dedicated servers, UUID-seeded characters, goals, token decay, scoring and data structures."
tags: ["area/game-idea", "project/game-jams", "type/design-doc"]
---

## Multiplayer stones game: Pilgrimage

### Game description

A minimalist multiplayer voting game. I just want to try something simple with Netcode for Gameobjects and dedicated servers in Unity. It would also be nice to say that I made an MMO once in my life, so I can put that aside.

Once every epoch the people make the long track to the stone circle. Every night for 100 nights they cast their vote on the future of the stone circle.

### Play mechanics

Players join the world.

Their character is proc gen based on their hardware UUID.

A circular stone altar with ~10 standing stones around the edge can be seen.

The player can move their character and interact with the stones.

Clicking a stone cycles its color between a set of colors and adds a player token to the stone.

Each player has a unique goal, represented as a goal color for some stones. This goal set is seeded by their UUID.

Every 15 minutes scores are calculated.

Player voting Tokens deteriorate over time.

Person score (Success) and global average score (Harmony) is shown.

### Implementation

Clients send their position to dedicated server

Clients send their stone votes to dedicated server

Server sends player positions to Clients

Server sends stone values to the clients

Server calculates votes and resolves scoring

### Camera and UX

The camera is fixed looking at the center of the ring of stones. The player can rotate the camera around the stones by holding the right mouse button or pressing A/D. The camera locks to the nearest stone if no input is detected for 2 seconds.

Left clicking on a stone or pressing W will zoom to that stone and the player’s character will walk to it.

While zoomed on a stone, the player can select which color they would like the stone to be with the A/D keys or the mouse. Right clicking or pressing S will zoom out again.

When a player is not logged in, their character moves away from the ring and stands in a circle around it. This means when you log in, you can see how many unique players have logged in since the game began, and on which stone people logged out the most often.

### Player characters

Characters are represented as meeple style figures, just a cone shaped body and a spherical head. The head has one color, and the body has two colors. The head and the body each can be +/- 10% in size from the norm. The colors and size are determined by a pseudorandom generation seeded by the client’s UUID.



### UI and Scoring

Two numbers are shown to the player: Personal success and Harmony

Personal success is the total of how many stones were colored in your favor over the last 10 in game days.

Harmony is the average Personal Success of all players that have at least one stone placed.

### Voting

When a player selects a color for a stone, their token is placed in front of the stone with the color they wish the stone to be. All other votes can be seen as a stack of tokens next to the stone, so the player can calculate what color the stone will be after the next voting period.

### Token degradation

When a player interacts with a stone, when a player changes their color vote or when a player removes their token, the change is sent to the server. The server also keeps track of how long it has been since a player interacted with a stone. If it has been longer than 3 days since a player has placed a token, the token will degrade and be removed.

### Stone visualization



### Goal types

Goals can be one of several types

- A number of stones must be X color

- The nth stone must be X color

- A stone of color X must be next to a stone of color Y

### Graphics

Simple low poly, asset packs.

Day/night cycle to show the passing of time. Sync to system time at one cycle per 15 minutes (or x96 speed).

VFX to show when you are gaining points.

### Data structure

GameManager

- Scores Dictionary\<UUID, int\>

- GlobalScores int\[\]

&nbsp;

- Stones Stone\[\]

- Tick int

Stone

- Color enum

- PlayerVote enum

- Votes Dictionary\<UUID, enum\>

Pilgrim

- Position Vector3

- targetStoneIndex int

### Synced things

Characters position and facing, if logged in.

Stones color

### Unsynced things

Player animation state
