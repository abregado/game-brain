---
title: "BS - Mechwarrior with Boids"
source: "Game Stuff/Game Ideas/BS_ Mechwarrior with Boids"
modified: 2024-12-13
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Mech Games (video)]]"]
concepts: ["Mechwarrior with Boids", "Design: Boid Unit AI"]
words: 278
summary: "Design for a mech squad game where pilots are boid-steered, with player-set target and zone rules and pilot personality weight modifiers."
tags: ["area/game-idea", "project/mech-games-video", "type/design-doc"]
---

BS: Mechwarrior with Boids

Player Interface

- Choose which targets are valid for a pilot to fire on

- Choose which weapons are active for a pilot

- Which targets to avoid

- Unit groups “Stay near eachother”

- Which speeds are allowed

- Operations zone. Draw an area that mechs must try to stay inside of.

Boid variables based on mech

- Optimization: Optimal range for currently charged and active weapons

- Safe movement: I want to avoid terrain that is slippery if I am moving at a unsafe speed

- Seek Cover: I keep obstacles between me and dangerous targets. More armor makes this weight weaker

- Indirect Fire: I keep obstacles between me and my allowed targets. More IF weapons makes this stronger

- Speed: Keep my mech moving at the fastest possible safe speed

Boid variables based on player interface

- Be Unseen: Push to get away from fire arcs for Avoidance Targets

- See my Target: Push to get my allowed targets into my firearcs

- Unit Cohesion: I need to stay near my squadmates, and move in the same direction.

Pilot Personality does not add new weights, increase adds a weight modifier to other weights

Boid variable modifiers based on pilot personality

- Seek Cover: I want to avoid taking damage

- Indirect Fire: I want to keep obstacles between me and my target

- Optimization: I want to get as close / far as possible from my targets

- Safe movement:I take risks with my mech

- Speed: I want to stay at top speed/safe speed

- Unit Cohesion: I’m a lone wolf / prefer to be near my team

-
