---
title: "Game Concept Doc - Quarks"
source: "Game Stuff/Game Ideas/Game Concept Doc - Quarks"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "designed"
projects: []
concepts: ["Quarks"]
words: 453
summary: "Concept doc for 'Quarks', a 2D physics puzzle demo where colonies on orbiting nodes harvest energy from pools via links, intended to show off reverse path finding."
tags: ["area/game-idea", "type/design-doc"]
---

Game Concept Document

*“Quarks” (Working Title)*

Ben Buckton

### **Introduction**

Quarks is set in a small world where tiny creatures live only to consume and reproduce. Competition for resources is fierce between rival colonies of these critters. The players have only limited control over the environment and must keep all of the colonies thriving.

### **Background**

This concept is designed as a demo game to show some of the ideas behind using reverse path finding to create in game behaviors and procedurally generated environments more interesting.

### **Description**

The game universe consists of many elements that all orbit around Nodes. Creatures called Quarks live on these Nodes constantly working to increase their own population and gathering resources. Everything in Quarkdom moves, constantly. The smaller nodes orbit around the larger ones, much like planets in a solar system. As colonies of Quarks increase in size, they must gain access to a wider variety of resources called Pools which move exactly like nodes but are finite in quantity.

The Player has only two tools available to him. It may move Mass from one node to another by siphoning it over time. Alternatively it may tear a chunk of Mass from a node and let it drift into orbit.

### **Key Features**

- Dynamic Environments. No two games will ever be the same as the universe is constantly changing based on the players actions.

- Problem Solving. The challenging puzzle formed by the Quarks interactions is sure to test the minds of even the sharpest player

- Fast paced: Players with sharp reflexes will be able to capitalize on key opportunities as they arise during the game

- Based on simple principles: The games mechanics are very simple to develop

- Easy to learn: New players should have no trouble getting into the game

### **Genre**

Quarks is quite clearly a physics puzzle game. However by utilizing path finding in the decision making processes rather than as an outcome, the creatures within the game should be very interesting to interact with.

### **Platform**

Quarks would be developed using a commercial 2d engine, such as Torque. 3d graphics would not bring anything to this particular project except to increase the development time.

More Information

Pools are generated whenever Nodes are separated or joined.

Pools contain a limited supply of energy

Quark Colonies harvest energy from Pools by using Links

Links can move a number of units of energy from the Pool to the colony per second

Longer Links transfer slower than Shorter Links

The only thing that blocks Link paths is Nodes

Links are always straight lines

When Links cross over each other, the Quarks fight

When Links are both harvesting the same Pool, the Quarks fight
