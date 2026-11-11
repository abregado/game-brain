---
title: "BS - Ship System Network Ideas"
source: "Game Stuff/Game Ideas/BS - Ship System Network Ideas"
modified: 2021-07-12
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Space Station 13-14|Space Station 13/14]]", "[[Spacetrauma]]"]
concepts: ["Ship Systems Network Simulation", "Design: Atmosphere Simulation", "Space Station 13/14", "Spacetrauma"]
words: 1299
summary: "Technical design for a networked ship-systems simulation (power, atmo, data) with machines, links, ticks, gas pressure equalization and SS13 panel references."
tags: ["area/game-idea", "project/space-station-13/14", "project/spacetrauma", "type/design-doc"]
---

Stories that can be told with the final system:

The AI can be told to change any parameter of the system that it is connected to.

Shipboard communication interrupted in localized areas, meaning some players cannot interct with the AI

Life support is localizaed, so that some areas require specialist equipment to traverse.

Power and Life support are undamaged but the connections between them are damaged. Re-route or repair the connections. In the meantime Lifesupport is running from backup power but wont last forever.

Crawlspaces and Corridors become cut off due to blast doors (closed by default) or lose life support due to being connected with breached sections (domestic doors open by default). Override consoles might be damaged, or the connections to other terminals might be severed.

Even after repairing and reconnecting systems, they take time to come online. Nothing should be instant.

Network Visability (Diagnostics) should be falible. You might not be able to see or get a reading on a system but it might be perfectly unharmed. Going and having a look for yourself is the only way.

The opposite should also be true. If diagnostic equipment is damaged then machines might read functional when they are actually dangerously damaged.

Abstraction

Entities

- Machine Objects

  - Array of Links

  - Location (cell or x/y)

  - n Needs per n Ticks

  - n Provides per n Tick

  - Storage

  - uptime

  - Request Priority

  - Enabled/Disabled

  - Damaged/Stable/Destroyed

  - [*Production/Consumption Functions*](#productionrequestconsumption-functions)

  - secondary settings (variables that not all machines have)

  - Need some way to track the networks a machine needs.

  - Required network list

  - 

- Links/Relationship

  - Location (cell or x,y)

  - Machine linked to

  - list of resources transferred/network name

- [*Resource/Network types*](#networks)

  - Atmo

  - Power

  - Control

  - Data

  - Proper network objects

  - If a network is searched which does not exist it is initialized.

Logic

- Machine

  - Needs available? Checks storage and then Linked

  - Accessible Resources (resource type): checks Linked for that resource type. Recursive. Returns amount of resources available.

  - Machine Type in System. Can this machine see a (type) via Links. Recursive. Return status

  - Check for networks

Each tick each object produces if it had the correct pre-requs last tick

First all Machines produce

Then based on priority, Machines consume if they have reached their Need Countdown

Damaged Machines produce a different amount to normal, perhaps consume more needs, or more readily

Delay between consuming needs and outputting Production

Needs split if more than one Machine at same Priority

Machine must be Enabled after being repaired

Allow hooks into the Machine Layer

Other game effects might be dependant on Machine status

Concepts

- Heaters/Coolers for Atmo effect temperature. Damaged ones might have negative effect and need to be disabled

- Breathable Atmo for rooms based on deck Life Support and local hull

- Blast Doors automatically closed when linked system fails

- Domestic Doors automatically open when linked system fails

Time to come online. Once systems are repaired, they should take a while to fully power up and start contributing.

Overloads and time cost for starting things that are not ready.

### Production/Request/Consumption Functions

Each machine has a function for what it produces, and how much it consumes. These request available supplies using different network names. Prouduced items are stored in this machine. Consumed items are always taken from internal storage of the local mahcine. So a third function determines how many resources this machine pulls from the network.

All of thesefuctions may produce different results based on internal variables. A power generator may have its production efficency effected by uptime, so that it burns a lot of fuel for the first 30 minutes of operation. A Life Support system might have a several minute cooldown after being disabled. A replicator unit might automatically shutdown if it is deprived of materials for a longenough time, requiring manual restart.

### Networks

Networks are simply a way of groupsing Links using identifier strings. Major machine groups might create asymetric gameplay when dealing with different types of networks, but undernearth they should all work the same.

When a machine Requests goods it searches other machines in a specific network. A list of all other machines connected on that network is returned and resources can be taken from them. For example: A power generator has a one way link to it from a Battery Bank. The battery bank requests power and sees the Power Generator, taking the power for itself. It also has outward facing power network links to other devices which may take the power from it.

Links contain a clamping function which limits the amount of resource that can be seen on the other side of the network. This can be used either as a “bandwidth” or in order to trigger something if too much/many resources are available as in a circuit breaker

Normal kind of network: Pure Network

Contains: an amount of resource, resource name

The resource is available everywhere in the network

Special kind of network: Gas/Liquid

Differences to regular networks: Pressure, content mixing, temperature

Pressure is based on contents and temperature

Contents need a pressure and temperature flash point

Life Support as many networks

Waste Gas (to be filtered), Mix (clean air from filter), Atmo (air in rooms)

Atmo blocks mix and level out over entire network

Atmo blocks linked together through doors, which if open effect the rate of change (size)

Atmo blocks also take mix from Vent blocks and add the contents to their mix.

Atmo blocks have a volume attribute

Pressure is calculated from volume and contents.

Vent Blocks only contain so much Mix which they pull from the mix network. The amount they contain can be modified which leads to pressure changes.

Scrubbers continuously take mix from the Atmos Blocks if they detect higher than required levels of different chems. They can also be set to “flush” in which case they will try to drain the room.

Pressure can be changed

Space Station 13 has a number of panels with the following functions

APC panels

- basic functions

  - turn power for enviro, light, systems on/off

  - accept charge from station mains

  - allow use of battery on system mains (discharge)

- wires exposed

  - 

Station Wide power consumption

Security and Crew Monitors

Door Controls

Atmosphere Panels

Fire control panels

MSFU Energy Storage

Tool Lathe

Supply Ordering

Equalization equations

Non-realistic approach 1

- No temperature

- Only gasses

- Gasses need to mix in a volume

- All gasses have the same size/weight/mass

- Update Loop

  - Movement Update

    1.  Iterate over all volumes

        - Iterate over all links to this volume

        - Gas only flows from high to low pressure

        - Group links by destination. Add areas together.

        - Amount that moves is based on total surface area

        - Cap amount by pressure difference

        - Tag a positive change for destination in New State object

        - Tag a negative change for this volume in New State Object

    2.  Apply New state object to old state.

  - Gas change Update

    1.  Iterate over all volumes

        - For the gas with the highest amount, iterate over all recipes with that gas

          - If volume recipe required pressure is correct, apply that recipe modified by the process % speed and the amount of the least available ingredient

- Pressure change cap

  - 25% of total pressure per tick MAX

  - \<1 difference means no change

Reactions can produce more or less units of gas than they consume.

Example reactions

- 2x Hot air + Cold Air = Breathable Air

- 2x Superheated Air + Cold Air = Hot Air

- Burnable + Superheated Air = Superheated Air + 1 Pollutant

- Burnable + Hot Air = 2 Superheated Air + 1 Pollutant

Equations
