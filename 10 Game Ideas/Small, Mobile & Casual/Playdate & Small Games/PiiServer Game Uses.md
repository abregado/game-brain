---
title: "PiiServer Game Uses"
source: "Game Stuff/Game Ideas/PiiServer Game Uses"
modified: 2014-04-14
type: brainstorm
area: game-idea
status: "idea"
projects: ["[[Playdate & Small Games]]", "[[Player Market Hoardmode]]"]
concepts: ["Pii Server Games", "Massively Single Player Market", "Design: Tick Distribution", "Stored Ship Designs"]
words: 233
summary: "Ideas for free web/android games using a Raspberry Pi as a lightweight server: massively single player market, scoreboards, chat, hints, ship design store, level distributor, tick distribution."
tags: ["area/game-idea", "project/playdate-small-games", "project/player-market-hoardmode", "type/brainstorm"]
---

Free games for web or android that could use the Pii as a server

Limitations

- Latency mustn't be an issue

- should not generate heavy traffic for a single user

- no logins or identification apart from IP address, maybe unique key stored locally

Massively Single Player market

- Store items that players are offering for trade

- limit store updates to once per day

Scoreboard recording

- send player name, score and other details to the server when a game is finished

- send players a list of the current high scores to compare with their local ones

- record seed of the game as well, so that scores can be compared per seed

IRC ingame chat

- allow players to chat with one another during the game

- players could leave messages behind

Players leaving hints for each other

- hints are shown in the game world

- i think dark souls has something like this

Store ship designs

- in any game with customizable craft or characters, store these on the server for everyone to use

- players get a commission if their design gets used

Level Distributor

- to ensure every player gets the same level, it is served from the server each day/hour

Tick distribution

- players only get so many ticks per day/hour/time

- their client must connect with the server to receive tick updates

-
