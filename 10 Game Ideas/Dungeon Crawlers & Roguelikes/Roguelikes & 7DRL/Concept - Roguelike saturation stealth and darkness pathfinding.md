---
title: "Concept - Roguelike saturation stealth and darkness pathfinding"
source: "Game Stuff/Game Ideas/Concept - Roguelike saturation stealth and darkness pathfinding"
modified: 2014-10-04
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Roguelikes & 7DRL]]"]
concepts: ["Lantern Saturation Roguelike", "Design: Stealth and Darkness AI"]
words: 551
summary: "Design notes for a small-room lantern-based roguelike where light gives colour saturation to enemies; details player kit, shield/javelin combat rules and six enemy types using darkness pathfinding."
tags: ["area/game-idea", "project/roguelikes-7drl", "type/design-doc"]
---

Small rooms, 10x10. Lantern lights up a 5x5 area.

Tactical choice combat

Each item(can carry 5) has a once per room active use and a passive bonus for carrying it.

When reaching the mid point of the players fuel, a large popup appears offering safe return to the surface.

Items taken back can be used on later runs, but a dead hero loses everything.

Saving a full rack of good gear to make the final boss run is the end game strategy

Player carries a lantern, sword and shield, and a javilin

When sword and shield are drawn the lantern is put down

lit area is static while the character fights, as the lantern must be put down

simple bump combat for melee

shield has very high chance to block attacks

80% when moving with shield drawn

95% when stationary with shield drawn

damage juice popout markers when hitting

no way to heal damage

shield takes one damage each time it is hit or it is unavailable for turns equal to damage

larger hits give more warning so the player can move out of the way

enemies with ranged attacks get a yellow “!” above them when they aim, it turns to red the turn before they fire.

takes 3 turns to fire at the player

javelin takes one turn to throw

can be retrieved by moving on top and pressing wait

the world is very grey

the lantern gives a yellow glow to the world

the lantern gives saturation to enemies

enemies with high stealth have a resistance to the saturation effect of the lantern

enemy 1- shadow djinn

used djiksta to move towards the edge of shadows and stay there

if the player moves into medium range these throw projectiles

will only melee the player if they can stay within the darkness

will move around in the darkness to make it harder to be attacked

eyes will glow for one turn after firing at the player

enemy 2 - stone camo spider

has high resistance to the saturation effect

will not move until the player moves into medium range

may pounce or wait until closer

enemy 3 - basic skeleton archer

takes 3 turns to aim/fire then 3 turns to reload (will move away from the player during this time)

immune to javilin

moving into darkness will make them miss

will move toward guardian plinths if available

enemy 4 - temple guardian

unkillable golem

has a “plinth”

will move slowly and attack the player when within range of the plinth

will stay on the outer edge of range until the player moves out of sight

knocks the player backwards, and cannot be blocked

takes 1 turn to attack the player, “!” appears turn before hit

initial activation occurs when player moves close to the plinth

enemy 5 - scarab beetle

swarm creature

easy to kill

leaves a goo pile when dead

player slips over, moving in a line and losing a turn if they step on the goo

attacks in groups

enemy 6 - basic skeleton warrior

simple hits doone damage to the player on bump, no shield stun

heavy hits have one turn warning, and do 1 turn of shield stun of blocked, 2 if unblocked

has no camo and moves toward the player at a normal rate
