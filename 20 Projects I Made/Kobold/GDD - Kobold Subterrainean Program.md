---
title: "GDD - Kobold Subterrainean Program"
source: "Game Stuff/GDD_ Kobold Subterrainean Program"
modified: 2023-03-10
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Kobold]]", "[[Game Business & Funding]]"]
concepts: ["Kobold", "Game business & funding"]
words: 946
summary: "Game design document for Kobold Subterranean Program: a 2D co-op rocket/vehicle building game for parents and children, with funding basis, pillars, mechanics, level types and controls."
tags: ["area/game-idea", "project/game-business-funding", "project/kobold", "type/design-doc"]
---

# Funding Basis

Serious game: Promotion of parents playing WITH their children as a method to generate teachable moments.

Get kids interested in STEM.

# Oneliner

“A building game that is cooperative, not just when designing vehicles, but when driving them.”

“As if KSP and Lander had a baby, and it was multiplayer”

# Pillars

Co-pilot control concept for parent-child play

Faster design-\>test-\>design cycle than ksp

Simpler physics. 2d. No atmosphere. Simpler design goals.

PC/Console, gamepad, young audience (6+)

## PC, gamepad, young audience (6+)

Why?

- Minimal market coverage

- Keyboards and touch screens are not designed for multiple people to use them

- Promote putting the gaming pc in the common space

## Faster design-\>test-\>design cycle than ksp

Why?

- Children has lower attention spans

- Instant feedback to show what went wrong

- Promote the engineering cycle

How?

- Simpler simulation: gravity only, instant thrust

- Limited considerations (no money or prices, no fuel weight)

- Quick restart/retry

- Build and Pilot mode are in the same scene

- Simulator mode where you can try without consequence.

## Simpler physics. Simpler design goals.

Why?

- KSP has only long term goals

- Promote breaking the problem down into small parts

- Lowers control complexity as well as design complexity

How?

- No fuel weight, everything runs on batteries.

- No atmospherics, vehicles operate in a vacuum.

- Limited connection points

- Forced craft symmetry

- Controls to automatically stabilise (training wheels).

- Objectives are small but the game incentivises you to complete multiple in one run and return to the start.

## Co-pilot control concept for parent-child play

Why?

- Putting the parent in the passenger seat promotes a good learning environment

- Improve agency of the child

- “Let them try, Let them fail”

- Improve grit, resilience and self confidence.

How?

- Child can “offer partial or full control” and the parent can take over only what is offered.

- Simulator mode where you can try without consequences.

- Split screen so both players can demonstrate an idea and discuss it.

- 

Concepts

Used

Fixed Gravity

Centre of Gravity

Not used

Rocket equation: Fuel is weightless

Game loops

Design -\> Drop -\> Design -\> Drop -\> Finalise Design

-\> Choose proven vehicle -\> Attempt real Drop -\> Unlock new start position -\> Design -\> drop

Progression

Completing multiple missions with the same craft unlocks more parts.

Completed missions become your infrastructure

Reducing cost per kg of cargo.

Reaching new locations where you can open up new shafts, construction sites and drop zones.

One Line Pitch

“An engineering game designed to tackle a less complex problem than spaceflight.”

“A building game with UX that works on controllers, in split screen.”

“A building game that is cooperative, not just when designing vehicles, but when driving them.”

“As if KSP and Lander had a baby, and it was multiplayer”

“Coop vehicle building game where how well you drive and design affects your progression.”



In flight Mechanics

**Forgiving damage system**: For some reason the Kobolds build the capacitors on the outside of their ships. When these bump into something they lose some of their charge (fuel). Parts of your ship never stop working due to damage so you can recover from a small mishap.

**Stabilise button:** There is one button you can hold to remove velocity and hold position. This of course uses up energy, and generates heat, so you can’t hold it forever.

**Heat:** You can’t use the engines constantly as they generate heat. Every ship has a heat sweet spot. The further you are from that spot, the less efficient your capacitors are, increasing fuel consumption. Heat builds up slower than it dissipates.

Types of Level

Shaft exploration.  
Go as deep as possible and return to the top. Each time you go down and reach a checkpoint a recharge station gets built for next time that you can use to go deeper and return from deeper.

If you reach the bottom of the shaft, you unlock Route Optimization for that shaft and unlock Tunnels at that depth.

Route optimization.

Repeat the same shaft but land on all platforms in both directions. Try to optimise the cost per weight of cargo you move. This value will affect the price of new ships deeper in your system

Tunnels.

Horizontal levels used to discover new shaft locations. These require different kinds of ship, and also require that no cargo be carried. This allows the levels to be much faster, tighter and difficult. Some Tunnels also require coop play, where one player must land on a pad to open the way for the other.

Gamemodes

One of the more difficult things to implement is that building an flying should be doable simultaneously. The iteration length when testing out a vehicle should be very short. So the level you select should be running in the background while in the editor. Testing the vehicle should cost no resource, however when you are ready to fly for real, the editor should be inaccessible.

Simulation build game mode

Controls

Select a connection node on your design with right stick

Scroll up and down the piece selection with left/right bumper

X: rotate which connection node of the to be placed piece is to be attached.

A: attach piece

Y: toggle mirror

The following ship statistics should also be visible on this screen without opening a dialog or special view mode:

- Centre of gravity

- Centre of thrust

- Weight

- Optimal Heat

- Maximum heat accumulation speed

- Energy max

Coop/Splitscreen

The actual most difficult thing about this design is getting this all to work seamlessly with drop in/drop out splitscreen
