---
title: "GDD - Mission Engineer game"
source: "Game Stuff/Game Ideas/GDD - Mission_Engineer game"
modified: 2020-06-26
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Coop Station]]", "[[Ship Repair Squad]]"]
concepts: ["Mission Engineer Coop", "Ship Repair Squad"]
words: 488
summary: "Short GDD for a 2-4 player coop game where crew prepare a spaceship for rocket burns, hunting hidden faults in components with Papers Please style checking; handhold movement phases."
tags: ["area/game-idea", "project/coop-station", "project/ship-repair-squad", "type/design-doc"]
---

GDD -Coop Mission

Phase 1

Several 3d ship components that can stack together.

- Framework with hand holds

- Perpendicular Support beams with runner

- Solid cylinder with openable service lockers

- Solid Cylinder with hatch

- RCS Disc

- Fuel Tank with pump access

Internal components

- Control panel with grid of switches, indicators and screens

- Area with service lockers

Movement system Phase 1

Each area has handholds. The player moves between these handholds by hovering and clicking on the next handhold. Handholds are linked in the editor to determine which ones are reachable.

Movement system phase 2

When in a space suit, the player needs to click a second time to complete a quicktime event in order to make the move successfully. They also have two wires with carabiners, similar to Via Ferrata equipment. They cannot attempt a move without one line being attached. The player needs to attach and detach these lines to move around. If they fail a move, then they reel themselves back to one of the clipped points.

Gameplay

The 2-4 players start a mission together. They select a ship type and a mission type (In Phase 1 there is only 1 of each). A mission is a series of 3-5 rocket burns.

The game generates some issues with the ship that will happen before each burn.

Play starts 5 minutes before the first burn. The players need to test the ship systems and prepare for the burn to take place. There is always a problem before each burn, but the players do not know what it will be. Sometimes the fault will be not a functional fault, but an instrumentation fault.

The players have a hardcopy of the mission parameters ,including all of the burn specifics.

The first thing they do is to check with the navigation computer to make sure all the data is correctly input. The players do not complete the burn, instead they just ask the computer to do it for them. Assuming all systems are working, the computer can handle this.

This creates some Papers Please style gameplay where the players need to double check the ship for things that dont match.

Components need be checked but many can be checked from the control module area via linked indicator lights. These indicators can also be faulty.

Components

- Flight Computer (unbooted, unpowered)

- Flight computer screen (unpowered, glitching)

- Memory Units (flashed, unpowered)

- FuelPumps (unpowered, blocked)

- Liquid lines (iced, leaking, blocked)

- Igniters (unpowered)

- Pressure gauge (jammed, unpowered)

- Tank Pressure Regulators (jammed, unpowered)

- Pressure sensor (uncalibrated, unpowered)

- Tank Heater (unpowered)

- Temp sensor (uncalibrated, unpowered)

- Solar angle (jammed)

- Battery Banks (disconnected)

- RCS nozzles (iced, jammed)

- RCS nozzle heaters (unpowered)

- Control linkages (iced)

- Heat sink deployment (jammed, iced)

- Power fuses/breakers (tripped)

Before burn is started, all crew need to be back in their seats.
