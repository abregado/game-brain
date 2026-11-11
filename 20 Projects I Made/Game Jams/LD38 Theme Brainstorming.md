---
title: "LD38 Theme Brainstorming"
source: "Game Stuff/LD38 Theme Brainstorming"
modified: 2017-04-22
type: brainstorm
area: jam
status: "idea"
projects: ["[[Game Jams]]", "[[RTS Ideas]]"]
concepts: ["Ludum Dare", "Planet Eating Fish", "Fog of War Maze", "Spectrometer Planet Puzzle", "Tiny Planet Gravity Jumper"]
words: 666
summary: "Brainstorm for Ludum Dare 38 theme Small Worlds: interpretations, gameplay styles, one-liners, and a developed planet-eating fish exploration game idea with code and asset lists."
tags: ["area/jam", "project/game-jams", "project/rts-ideas", "type/brainstorm"]
---

## Theme: Small Worlds.

## Interpretations:

- Tiny planets

- Small World ([*the book*](https://www.thalia.de/shop/home/rubrikartikel/ID2927320.html?ProvID=11000522)). About a man who has Alzheimer's whose world is getting smaller because his experiences are vanishing.

- Close borders

- Worlds of small creatures (Ant farms, insects)

- Animal Kingdom (Chibii style)

- Supernatural “Otherworldly”

- Worlds are small because it is a space game and you look at the from really far away (Like trying to detect the planets from telescope on earth)

- Small world can simply mean uncomfortably small game levels

- Big world viewed through a small hole

- The worlds are small because you are big.

- World under a microscrope

## Suitable Gameplay styles:

- Gravity based games

- Forgetting items and abilities

- Everything you do affects your neighbours

- Camera tricks with zooming in and out (ala Captain Toad)

- 

## One Liner Designs:

- A gravity driven game about jumping between tiny planets (been done i know)

- Navigate a maze which is covered in a “fog of war”. When you step on a tile you have been to before the hidden parts of the map are recreated. As you find special locations, those parts of the map are fixed.

- The puzzle game where you have to analyse data from spectrometer trying to identify atmosphere of faraway planets. This will require a lot of trial and error from the player.

- Similar as above, identify planets by firing particles which are attracted in a gravity like way to different types of planets, or that change color based on the type of planet they pass through. (I already have access to a gravity simulator :D)

- You control a planet eating fish, every time you eat a planet you change your appearance. Requires smart system for changing fish and some procedural generation. Not a lot of gameplay, this is more about visual exploration.

  - **B:** So you can only eat a blue planet if you are a blue fish (for example)?

  - **V:** No, you can eat anything you want, and depending on what you ate, you will change in a different way. It is all about exploring what kind of fish you can create and trying to predict how each planet will change you.

## The Fish Idea

Extended Description

Features/Ideas

- Gravity based movement(?)

  - does that take away from the exploration feel?

  - Slingshot mechanics

  - Button to halt momentum

  - Button to match Orbital Speed with closest physics body

- Other movement ideas?

- Collecting planets modify your fish type/ modular parts

  - How many parts/sections do we need to make the idea interesting?

- Procedural planet images using layers?

  - How many different layers needed?

- What else is in the world?

- 2d Top View Perspective

- The goal is just to explore the combinations of fish

- Fish properties affect how environment looks

  - If you have certain fish parts then some types of planet might glow or animate

- Message area to explain narrative to the player

  - Console style?

  - Speech bubble style from portrait?

  - Particle Text

Code:

- Import HUMP tools, camera api.

- Set up camera on Player.

- Solar System thingo system with planets moving around a sun using a Tweening library (simple, medium time)

- 4 way placeholder player movement (simple, quick)

- PLAYABLE HERE - play testing

- Collisions for collecting and bumping (simple, quick)

- Change to vector based movement (constant acceleration, no gravity). Mouse and WASD

- PLAYABLE HERE - play testing

- Import Anim8 Library if we want to use 4-8 frame animation

  - Or if we just animate with color change and rotation then use the tweening lib

- Multilayer drawing for planets and fish portrait (mid-complex, quick)

Asset list:

- Space background

- Gravity sources

  - Suns (1-4)

  - Black hole (Maybe)

  - Pulsar (Maybe)

- Planets

  - Layers (10-20)

  - Glow variations (?)

- Asteroids

  - Variations (1-5)

  - Glow variations (?)
