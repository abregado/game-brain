---
title: "Concept - PulseCoaster"
source: "Game Stuff/Game Ideas/Concept - PulseCoaster"
modified: 2015-06-24
type: design-doc
area: game-idea
status: "designed"
projects: []
concepts: ["Pulse Coaster"]
words: 458
summary: "Outline of PulseCoaster, an inertial racing game moved by timed engine pulses with heat management, mazes, time trials and a 1D shooter variant; mechanics to try."
tags: ["area/game-idea", "type/design-doc"]
---

Concept Outline - PulseCoaster

The player is in control of a craft which is moved by pulsing its engines every few seconds. This counteracts the effect of friction which slows the craft down. The Player completes a quicktime event to determine how strong each pulse is. (Alternatively, the player can have one button when is held down to charge the pulse).

The game uses an inertial movement system in which the player can only apply new momentum in a forwards direction. The player can twist the ship between pulses to choose the direction he will move towards.

Each level is an increasingly complex maze or racetrack. The Players ship can rebound off walls but will eventually be destroyed from too many collisions.

The time between pulses is based on how large the most recent pulse was. If the player chooses a low power pulse, the drive will come back online much sooner than if a very large pulse is used. However the velocity gain from a large pulse gives more velocity change than several pulses over the same period of time.

Each pulse also generates an amount of heat in the ships engines. This heat level does not dissipate, instead being based on the last pulse size. The player must warm up and cool down the pulse drive by choosing pulse sizes not too dissimilar to the last. If a player has accelerated heavily for the last few turns, then they cannot perform a very small pulse without damaging the engine. This works in reverse as well. If the player wants to perform a high energy pulse, first they must perform a number of increasingly larger pulses to build up to the largest one. Remember that to slow down, the player must simply do nothing, or pulse when facing backwards. This means a player can always stop by turning around and performing the same level of pulse as he did last time.

Conflict in PulseCoaster comes from both time trials and competitive racing between players on the same keyboard.

1d concept would imitate a top down lane shooter. The player ship can dodge left and right but its dorward progress is bases on the inertial system.

If the ship is run hot enough (close

To the point of explosion) then an inertial damping field comes online reducing drag.

When the ship collides with ibstaclea it fires a laser to break through but this generates heat.

Mechanic to try

Different drag based on crossection of hull facing direction of travel.

Add accelation instead of speed. Accel drops back to zero quickly. Means you have to steer straight for a short time after pulsing.

Accuracy of boost based on damage. Inaccuracy decided when boost is applied. Severity based on heat
