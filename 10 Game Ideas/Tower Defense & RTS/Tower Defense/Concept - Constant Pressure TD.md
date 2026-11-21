---
title: "Concept - Constant Pressure TD"
source: "Game Stuff/Game Ideas/Concept Docs/Concept - Constant Pressure TD"
modified: 2018-07-09
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Tower Defense]]"]
concepts: ["Tower Defense"]
words: 625
summary: "Concept doc for a survival tower defence with continuous creep spawning, free mazing, turret swapping, time-based income and construction; annotated by Ben as deemed terrible in 2018."
tags: ["area/game-idea", "project/tower-defense", "type/design-doc"]
---

Deemed terrible in 2018 (Ben)

# Player Story

A crate of supplies arrives, and just in time. This time around its a Mk27 Artillery Emplacement. It is going to take a while to get going, but once active, it should hold back the invaders for another few minutes. The chopper pilot radios in, asking if there was anything else you need. “Roger, please swap Turret 847 and Turret 334”. You can see that the line is barely holding. A mound of alien corpses marks the enemies progress but every now and again one of the buggers gets through the line. Sure they quickly get taken down by a Hunter-Seeker missile, but those missiles are expensive, and HQ doesn’t like to waste them...

# Main Feature

Instead of coming in Waves, creeps are constantly spawning and marching towards the goal. The player builds his maze and places towers in a short period before the creeps arrive, but after that, they must decide on new strategy while under fire. A player can see how close the enemy are to breaking through to the goal area by where the last enemy dies. The strength of the wave fluctuates but trends very slowly upwards.

- **Freemaze in strategic environments:** There are only a limited number of tower locations, and some fixed terrain obstacles, but to start with the player can freely create a maze to direct creeps. Once the creeps arrive, the maze will have to be modified in-situ.

- **In Situ Planning:** The player can periodically swap Turrets to modify his strategy. This ability is then on a cooldown, so its important to use it both frequently, and at the correct time. When buying a new Tower the timer for this ability is set to zero.

- **Regeneration:** The goal is protected by a series of regenerating passive defenses. This means the player is not penalized for letting a few creeps through every now and again.

- **Time based Income:** Cash comes over time, instead of for creep kills. The player also is rewarded with interest on unspent cash.

- **Time based construction:** New Towers take a long time to get up and running, plan ahead! Don’t worry, once they are finished they are much more mobile.

- **Powerup!** Creeps gain in power while not being shot at, meaning that shooting them early is very important. Making excessively long mazes will not help unless they are covered by towers.

- **Multi-DZ:** There is always more than one location at which the creeps spawn. Maze them together as soon as possible.

# Genre

Constant Pressure will be a solid Tower Defence game, but with a focus on forcing the player to make choices while under pressure. A strategy will be built iteratively, but tower placement will be more reflex based.

As reflex has more focus, the game should reward high player skill and game familiarity.

As a Survival game, players should be expected to fail and try again several times, as all play sessions will end with the player failing.

# Technology

Being a Survival game with a long playthrough time, Constant Pressure will need to have a robust save/load feature. Playtime per session should be at least 30-60 minutes.

A series of hotkeys will be needed to allow fast tower placements and this requirement means it is best to target PC, Mac and Linux platforms.

Constant Pressure is a single player game. Some effort may be spent making the game optimized for a high entity count.

# Market

The target audience will be those who already enjoy the Tower Defense genre but want something a little different.

Being a Player skill focused Survival game ,the game should be marketed toward the hardcore crowd, possibly even to roguelike players.
