---
title: "Pulse Coaster BS"
source: "Game Stuff/Game Ideas/Pulse Coaster BS"
modified: 2012-11-01
type: design-doc
area: game-idea
status: "designed"
projects: []
concepts: ["Pulse Coaster"]
words: 233
summary: "Brainstorm of a heat/speed simulation model for the Pulse Coaster game: variables for core, case and heatsink heat, pulse boosts, melting and cracking risk."
tags: ["area/game-idea", "type/design-doc"]
---

environmental stats

envTemp:int const

made up of

speed:int

drag:int const

pulseDrop

pulseSpeed

pulseHeat

coreHeat:int

caseHeat:int

caseFatigue:int

deltaCaseHeat:int

sinkHeat:int

hasSinksOut:Boolean

rateSinkDis (high):Number

rateCoreDis (High):Number

rateCaseDis (small):Number

charging a boost adds speed in a bulk lot (speed+pulsePerfect). It also adds heat to the coreHeat. Over time the coaster slows down due to drag, and heat is transferred to the sinkHeat and caseHeat variables at a fixed % of total heat in the hotter of the two (so they will equalise). The % of heat that can be transferred is based on the rate\*\*Dis variables.

So the heat from pulsing is placed on the core, which is quickly shunted to the case to equalise while being slowly shunted to the sinks, which is quickly shunted/equalised with the outside temp.

If the heat in the case gets too high, it begins to melt. This increases the chance of a pulse damaging the ships hull.

If the case gets very hot, but not hot enough to start melting, the heat can be used to power the Inertial dampening system, which allows the ship to gain much more speed in a pulse.

Also, if the deltaHeat of the case is too high in any frame, it can crack, also increasing the chance of a pulse explosion. So heating and cooling the case too fast is dangerous (example would be flying a hot ship into icewater with the heatsinks deployed.
