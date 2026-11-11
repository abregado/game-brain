---
title: "LD49 Round 2 Brainstorming"
source: "Game Stuff/Game Ideas/LD49 Round 2 Brainstorming"
modified: 2021-10-06
type: brainstorm
area: jam
status: "designed"
projects: ["[[Game Jams]]", "[[Catastrophic Journey]]", "[[Shooters & FPS]]"]
concepts: ["Ludum Dare", "Catastrophe Journey", "Vectored Thrust", "Ballast", "Vacuum Decay Escape", "Horse Teleport Stables", "Zombieworld Equilibrium", "Orbit Rocket Logistics", "Paper Plane Shooter"]
words: 641
summary: "Ludum Dare 49 round 2 game idea list (vectored thrust, ballast, vacuum decay, horse teleport, disaster roguelike) with a detailed spec for the hex-grid Catastrophe Travel game."
tags: ["area/jam", "project/catastrophic-journey", "project/game-jams", "project/shooters-fps", "type/brainstorm"]
---

**Round 2: What even game to make**

Vectored Thrust: Lander with cargo, player adds thrusters. Each thruster is bound to a key.

Ballast. Submarine that is sinking, push cargo around to make it land flat. Marker for centre of gravity. Currents and bubbles.

Escape vacuum decay. Expanding from points. Different rules inside each area (speed, turning, acceleration). Each decay has a level which overrides other decays. Fire/Cause particular decays to occur.

Select a horse - a destination position changes to random spots every second. When you press the button it teleports to the selected location and its position becomes more certain. When you button the teleport radius gets smaller and you need to teleport all the horses/animals into the stables without teleporting them on top of another one. All the horses have names of famous physicists.

Paper aeroplane side scrolling shooter. Wind coming across the screen effects your movement speed and shooting angle. Dont hit the ground.

Disaster scenario. Survival Game. Rougueliky. Tile based. Crappy 2012 movie. Alerts arrive that tiles will change. Weather disasters, chasms, volcanoes. Traversal gameplay to reach the goal. Procedural. Into the Breach style warnings that give you lots of time to plan. Resource harvesting to fill a food clock. Player chooses fastest path, or longer path to keep resources high.

Zombieworld 4 you win when you reach equilibrium with the number of zombies on the map for x time. Zombies come out of spawners and attack your base. Interact with 3d map, walls, turrets etc. You get tides of zombies the rate of zombie spawning goes up and down. Goal counter only ticks at the peak. Resources limited? Control small area, need to move to new areas to get more resources. Move heavy thing to other side of level. Tanks kill zombies.

Tricky Towers style - stack objects as they fall down. Build 3 separate towers on a scale mechanism.

Beaker of Chemicals. Add things to it to keep it unstable. Not really a game.

Sensory games. Driving a dizzy character.

Launch rockets from one orbit to another - then launch them back. Build up a collection of rockets that follow the orbits you have created for them. Don’t let them collide. Move resources around.

**Catastrophe Travel** **Thingo**

- Grid system (Hex first, then grid)

- Mouse selection

- TurnEndUpdate Function

  - Tile effect handler

  - Map generator

- Turn based, turn ends when you move

  - Move 1, 2 or 3 spaces each turn

- Terrain options - Removed by Disasters

  - Generic Tile Entity

  - Road - faster speed if you have a car

  - Forest - lower food usage

  - Mountain - slower speed

  - River - faster if you have a boat

  - Boat - Faster speed for X turns

  - Farm/Campsites/Supplies - collect supplies

  - Military base/dangerous location - lose people/ collect supplies

  - Town - collect people

  - **Bandit camp - every X turns it spawns bandits nearby roads**

  - Car - Faster speed for X turns

- Disasters

  - Volcano - makes lava every turn - creates 3-5 lava tiles every X turns.

  - Lava - lose people

  - Meteor - causes instant destruction around it

  - Chasm - opens up and expands each turn to an adjacent tile.

  - Swarm - moves every time

  - Locusts - spreads to eats forests and turns them into desert

  - **Bandit - steals resources if you pass**

- Resources

  - People

  - Supplies

- Food clocks

  - Use 1 supplies per turn

  - Max supplies so the player cannot indefinitely build up

- Disaster line moves across the map

  - Disaster spawning system

  - Disasters happen more frequently behind the disaster line

Sounds

- Walk

- Drive

- Volcano

- Lava

- Meteor Arrives

- Chasm appears

- Locust swarm eats something

- Collection Sound

- Ambient tense sound theme

-
