---
title: "R-Pi WLan Skimmer"
source: "Game Stuff/R-Pi WLan Skimmer"
modified: 2021-11-19
type: idea
area: non-game
status: "unknown"
projects: ["[[Non-Game Projects]]"]
concepts: ["R-Pi WLan Skimmer"]
words: 89
summary: "Idea for a Raspberry Pi program that opens a public WLAN, collects data from devices that auto-join, and emails owners how insecure they are."
tags: ["area/non-game", "project/non-game-projects", "type/idea"]
---

A program that can run on an R-Pi that opens a public Wlan network and waits for people to automatically join.

It then scrapes as much public data as it can and sends an email or message to the person to tell them how unsecure their device is.

At a minimum, we can get:

- Device ID

- Location (from R-pi)

- Time

This would already be enough to scare someone, but I’m sure there is much more information that can be collected from a phone or passing device.
