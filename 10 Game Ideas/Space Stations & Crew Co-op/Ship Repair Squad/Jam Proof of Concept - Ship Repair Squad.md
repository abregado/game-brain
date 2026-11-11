---
title: "Jam Proof of Concept - Ship Repair Squad"
source: "Game Stuff/Game Ideas/Big Five/Survival Space Station/Ship Repair Squad/Jam Proof of Concept - Ship Repair Squad"
modified: 2021-11-22
type: design-doc
area: jam
status: "designed"
projects: ["[[Ship Repair Squad]]", "[[Game Jams]]"]
concepts: ["Ship Repair Squad", "Design: Power Network and Device State Events", "Design: Feedback and Juice in Diagnosis Gameplay", "Ludum Dare"]
words: 1283
summary: "Jam prototype plan for Ship Repair Squad: iteration 3 feedback/juice analysis, OnPowerUp/Down device events, quest object hierarchy (navigation, propulsion, power) and a list of epics (power network, cable tools, bots, line of sight, pipes, data network)."
tags: ["area/jam", "project/game-jams", "project/ship-repair-squad", "type/design-doc"]
---

**Loop**

Explore -\> Triage -\> Repair

**Iteration 3 Where is the gameplay, where is the juice?**

The first two iterations were lacking consideration of feedback and juice. How would the player know if they completed the puzzle successfully? What happens if they use an incorrect solution? How do we turn this into an actual game loop?

Just activating the systems is not going to be fun and does not add into the Information Gameplay that I want to display with this game. The player should move through the game loop from Explore -\> Triage -\> Repair -\> Explore several times as they figure out the solution.

Then we come to punishments and feedback. There is no time to add a set of bad conditions, health systems, or failure states. Not that those are fun anyway. Instead the “punishment” for using an incorrect solution should just be to go back to exploring.

The Iteration 3 solution to this is to use the OnPowerUpEvent and OnPowerDownEvents more heavily for gameplay effects.

**OnPowerUp/Down Events**

When a device changes from powered to unpowered (or vice versa) it can change its state without player intervention. Some examples:

When a fire door loses power, it closes and locks

When a fire door regains power, it unlocks (but does not open)

When a cabin door loses power, it opens

When a cabin door regains power, it closes.

When the heat sinks are powered, they deploy automatically (but can be retracted manually)

When the reactor is powered it starts warming up to the level it had before being shut down. If the heat sinks have not been deployed, then this will end up with the reactor overheating and shutting down (also breaking a component)

When the SOS beacon is powered, it begins sending out an SOS signal (makes the round timer count down faster while active)

When a data console regains power, it begins a 1 minute boot up sequence, even if it had only lost power for a second.

**The feedback problem**

To make the diagnosis/triage section feel interesting, the player needs to connect environmental signals that they see and hear to possible problems.

Each feedback could be indicative of several different problems, however this might increase the complexity of the game and subsequently the cognitive load of the player too much.

We can also try to create a sense of mastery for the player, by having the feedback very succinct. When the player sets up what they expect to be a successful solution, they will also expect a series of feedbacks to confirm a success. For example, the Reactor makes a sound as it begins working, and then make a single louder noise if something goes wrong and it shutdown. The Heat pumps have a blinking light to show they are functioning. So if the player turns on the reactor, they listen for the sound and look for the blinking light.

**Another problem that will occur**

How do we stop the player(s) from becoming stuck? With the power state able to change at any moment,

**Goal**

The player must reactivate 3 main systems in the ship.

**Shuttle spawn area**

Players spawn here

**Quest Object Hierarchy**

- Navigation system

  - Maneuvering Thrusters

  - Sensors

  - Helm console

- Propulsion system

  - Main drive system

  - Fuel pump

  - Control system

- Power system

  - Radiation shielding

  - Main reactor

  - Emergency power system

  - Engineering console

**Epic**

Players simply need to walk to the systems and reactivate them.

UI opening on Interact

Toggle machine on Interact

Walls added to make that non-trivial.

**Epic**

Access panels need to opened, and their components replaced to restart systems.

Repair consoles first, then repair systems, returning each time to activate them from the console.

Deployable part replicator.

Shuttle based part replicator. Also can make batteries for the deployable part replicator.

**Epic**

Power added. Three stage power: Emergency, Low and Full.

Shipwide state so it is the same for every object at any one time.

Three systems:

- Emergency power system: Provides Emergency power level. If it receives Low power, it deactivates. If Low power is lost, then it reactivates, unless it has a damaged component.

- Reactor: Provides Low power, or Full power if the radiation shielding is active. Changes to low power if the radiation shielding is deactivated.

- Radiation Shielding: Needs Low or Full power to toggle.

Every system triggers a “Power level change” event, which for the doors, resets them to their default.

Emergency power activates lights

Low power allows doors to be activated

Full power allows the quest systems to be activated

Doors are added between rooms. Each has a different default state (open/closed) when the power is out.

Doors can be cut open with a deployable welding bot. There is only one of these bots on the shuttle. It can be reused.

Doors can be forced open with a deployable wedge bot. This forces a door to be in the open state. The bot can be removed from either side of the open door. Can be used to be sure a door does not close when power cycles.

Inventory. Each player can carry as many robots as they want (although there is only one for now)

**Epic**

Power network. Each powered object is connected to the power generator via a series of access panels.

Powered objects change to their default state when the power returns.

Access panels gain one “cable” component per connection running along here.

If the component is broken, the powered object does not get powered, even if the power generator is on.

**This system needs to be generic as it will be used for pipes and data connections later.**

**Epic**

Cable laying tool, which can lay cables between access panels. Deploy the tool on the ground, then connect access panels and machines to it.

Doors closing can cut cables.

Cable snoop bot. Deploying it on an access panel highlights its connections to other access panels. This bot can be redeployed to change what is highlighted. Only one on the shuttle.

**Epic (Jam version theoretical finish)**

Activating the shuttle to end the round early

Time limit

Once the time limit is up players must activate the shuttle within 60 seconds.

Victory and failure popups

New game button.

New players can join mid round

Players can return to the shuttle to disconnect

At the start of the round, everything is working and then a random set of things are broken.

**Epic**

Line of Sight blocking.

Map is hidden to start with.

Reveal rooms as the doors are opened or cut.

Deployable camera robots to keep an area revealed. Two of these on the shuttle.

**Epic**

Pipe network using copies of the power connections system.

Pipes work the same as power cables, but connect thrusters to the fuel pumps.

Reinforced doors have a hydraulic connection

Hydraulic pump system

Reinforced doors are connected to the hydraulic system via access panels.

Reinforced doors need both power and hydraulic connection to function

Reinforced doors cannot be cut.

**Epic**

Data network using copy of the power connection system

Console object which displays variables and status of connected object

Helm, Control and Engineering consoles change to these

Data connections can go through access panels

Everything is connected to a console in the same room, and also to the Central computer

Helm, Control and Engineering consoles are connected to the central computer.

Deployable bot, which allows players to visualize a data network, and see variables/state for connected objects. Single one on shuttle. Fitting this to the Central computer and repairing all connections would theoretically allow all object states to be seen remotely.

You could also just build your own data network using the cable tool.
