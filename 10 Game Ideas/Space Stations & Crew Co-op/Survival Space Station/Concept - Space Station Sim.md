---
title: "Concept - Space Station Sim"
source: "Game Stuff/Game Ideas/Concept - Space Station Sim"
modified: 2020-12-11
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Survival Space Station]]"]
concepts: ["Space Station AI Overmind Sim", "Survival Space Station", "Design: Station Task and Job System", "Design: Dual Timescale Disasters"]
words: 1868
summary: "Staged development plan and prototype description for a space station management sim where the player is an AI overmind, built on polar coordinate module placement, pathfinding crew, tasks, life support and ship docking; ends with bloat-feature notes on power, fires and districts."
tags: ["area/game-idea", "project/survival-space-station", "type/design-doc"]
---

### Basically an excuse to learn/use polar coordinates

### 

### Marketing Concept

To create a basic prototype on top of which to build a much more deep and interesting game.

### High Level Concept

The player is an AI overmind whose job it is to run a new space station efficiently. Substandard staff and equipment are provided and the AI must do his best to keep the station running. The fail conditions are either human revolt, all human lives lost or the station being destroyed. The Ai must also respect the free will of the humans allowing them time for their own inefficiencies.

### Gameplay and Goals

Ships come to dock at the station and the player must complete tasks for these to generate resources. These resources are used to persuade top staff to stay on at your station, and to build new sections.

### Rough development pathway

1.  **basic systems**

    1.  module object - radius and location

    2.  gantry object - contains linked modules, and if it is active/inactive

    3.  external addon slots entity

    4.  when module selected, hover and click UI elements for external addons

    5.  first addon is “Create new module

    6.  hover and click select UI elements for gantries and modules

    7.  ~~click must allow renaming of modules, and choosing a “zone”~~

    8.  hover shows name and zone type

    9.  zones do nothing yet

    10. clock UI element

    11. ability to pause the simulation with UI overlay effect - SPACEBAR and UI button

    12. hover glow and selection effect

    13. output module and gantry list to terminal on keypress

    14. initially just one module always the same

2.  **Module creation: Using polar coords**

    1.  freely placable new modules: set distance and size

    2.  checking collision

    3.  modules get a minimum safe distance

    4.  randomly placed external addons

    5.  gantries only can be built from empty external connections

    6.  module creation UI element showing size, cost and number of internal addon modules. external addons are added later.

    7.  placement UI also must show other external addon lines, and the minimum placement of all modules.

    8.  module hover and click UI must show % complete and tasks remaining

    9.  hold CTRL to snap to minimum distance and overlapping points

    10. play can now build a series of modules that are connected by gantries forever

3.  **population entities**

    1.  stored in modules and gantries

    2.  random name/gender/charateristic generator

    3.  Staff selection UI element - name and other variables

    4.  Staff hover UI element - name

    5.  staff list output to terminal on keypress

4.  **pathfinding between modules - fixed movement speed**

    1.  pop ents being passed between module and gantry

    2.  Debug pathfinding UI when a staff is selected

    3.  hover UI to show time remaining until staff move

5.  **tasks handler (points of interest) and skills (initally boolean)**

    1.  essentially a job list which is added and subtracted from

    2.  pop can request a job list that relates to them

    3.  higher priority intertupts

    4.  task POI UI element

    5.  add skills to pop ents

    6.  first skill: maintenace technician (crew randomly have this or not)

    7.  task list outut to terminal on keypress

6.  **add slots to module ents for internal Addons**

    1.  functions to search all modules for a type of Addon

    2.  Addon entity: These are added to slots in a module

    3.  new addon: Machinery - generated maintenance tasks and disaster events

    4.  hover and click UI when a module is selected for internal addons

    5.  deconstruction option in UI.

7.  **events handler: for recurring and random task creation**

    1.  receive requests to create new events from Addons and Pop

    2.  maintenance tasks for gantries

    3.  events continue until all deactivation tasks are complete

    4.  ability to provide messages to the player

    5.  messages UI element

    6.  ability to pause the game and ask for verification

    7.  verification UI element

    8.  events UI list with hover and detailed info showing requirements

8.  **player created positions (allowed skill list)**

    1.  setting wait areas (home module)

    2.  setting areas of operation

    3.  appointing staff to a position

    4.  position creation UI element

    5.  list all current positions UI element

    6.  delete a position with verification popup

9.  **Numeric Skill systems and Task update**

    1.  set up and packup times based on skill level (skill is now numeric)

    2.  skill checks for completing tasks

    3.  tasks can have finish and start locations: module,addon (start in module X, go to Y to complete task, finish is module Y): this adds a travel component

    4.  functions to find nearest suitable module/addon combo to a point

    5.  required Addon attribute for tasks at work location

    6.  new job: office/lab work(creates score)

    7.  new Module: Communications

    8.  new module: Office

    9.  new module: Archives

10. **life support (global effect)**

    1.  oxygen usage (per module, per population)

    2.  new module: Engineering

    3.  new addon: Airscrubber - generates atmosphere

    4.  new addon: Workshop - start spot of maint jobs

    5.  non-linked life support: excess air from modules fills other modules automatically

    6.  modules below 50% atmosphere will be disabled

11. **More construction stuff**

    1.  task creation to complete contruction

    2.  event handler checks if all tasks are complete

    3.  level creation changed to single AI module at beginning

    4.  player gets a fixed number of resources at beginning of game

    5.  new modules come with random staff (until staff come on ships)

    6.  player selects the zoning of the module at contruction.

    7.  new job and skill “Contruction

12. **ship arrival events**

    1.  new module: cargo bay

    2.  new internal addon: Refuelling station

    3.  new internal addon: Repair station

    4.  new external addon:docking bay

    5.  docking bays require docking lanes (straight lines from them to the map edge)

    6.  docking bays have an airlock size (size 1 or 2)

    7.  ship docking at docking bays

    8.  ship based task creation (refuelling, repairs, cargo unloading, cleaning, maintenace)

    9.  ships can be leaking atmosphere and therefore be a burden on your stations life support

    10. ship based tasks generate wealth

13. **crew changeovers**

    1.  crew stay for a fixed contract: length stored in crew object

    2.  once complete they will leave on the next crew ship that arrives

    3.  a replacement for them will arrive on the ship after that one, automatically taking over their job position if it is still available

    4.  when a contract is over, the player has a chocie to re-hire them for the shift after next, which costs resources.

    5.  off-station crew list, which is checked for replacements if you re-hire staff

14. **Save system**

    1.  just one station per player

    2.  self destruct to get a new station

15. **Prototype 1 release - see description below**

### Prototype 1 Gameplay Description

The player begins with a single module, the AI core, and a small amount of wealth to spend. The AI core has a random set of connections on it, one of which is a Docking Bay. This module also generates a small amount of Life Support by itself. Once the first modules are placed, a small ship arrives to unload your first staff members. Construction begins.

Small ships can come and go by docking with the AI core. These only have simple requirements and generate a very small amount of wealth. The player will need to set up a lab or cargo bay to begin generating more wealth. A larger docking port will allow larger ships to be serviced, but these also have more requirements.

Early construction will be limited by the docking port connected to the AI core. Once another docking port is set up, the player can begin expanding in a different direction by removing the starting port.

Difficulty will come from maintenance getting out of hand, a constant increase in staff size, and from difficult ships docking for a long time. Also as the crew develop and then go off station the player will have to deal with drops in efficiency.

STOP READING HERE THE REST IS JUST NOTES

Bloat Features

1.  module cargo system (capacity, inventory, movement)

    1.  cargo movement system between modules

    2.  tasks that create objects

    3.  new job: manufactoring

    4.  new module: cargo bay

    5.  loading of manufactured items onto ships for score

    6.  import/export of items on ships

2.  airlock system

    1.  EVA movement and pathfinding (slow, long set up time for entering/exiting an airlock)

    2.  tasks switched to internal and external

    3.  spacesuits moved as cargo between airlocks

3.  power system

    1.  each module has a power drain based on area

    2.  each addon, external and internal has power use,cycle time,cooloff,generation per cycle attributes

    3.  power storage modules/batteries to create cycles of charge and discharge

    4.  gantries have power transfer maximums and power is split evenly over all connections

    5.  gantries have circuit breakers which pop when they transfer too much power, and generate a task

    6.  circuit breakers can also malfunction or burn out each time they trip this can create fires

4.  fires

    1.  consume oxygen/atmo when active

    2.  can be in gantries or modules

    3.  modules can seal off affected parts (disabling some slots)

    4.  fire fighting systems

    5.  addons used to keep staff/equipment safe

5.  Dual timescale system

    1.  when an event begins, time slows to realtime/close to realtime.

    2.  they player can interact with the disaster/event without worrying about so much other micromanagement.

    3.  during this timescale individual crew can be commanded (imperfect)

    4.  this would build up to the combat system

Nodes represent modules on a space station

area of a node = how much workspace there is but also effects how much maintenace is needed

Players create roles on thier space station, selecting how much % of work time is used on each task and in which nodes/modules

Employees come in shifts or can be invited to live in the station

live in staff use % of their time for recreation and eating

Live in staff require more infrastructre

shift workers are randomised each shift but some will return repeatadley

changing the pod internals is much cheaper than building new nodes

nodes can only be built between shifts

new pods must be brought online by maintenance staff

efficency of work comes from each task having a set up time

a staffer doing work has an efficency decrease when starting a job, and builds up to 100% efficency after a period of time

travel times are effected by distance between pods and quality of the connections

workers will always stop waht they are doing to attend a higher priority job

districts

office

maint

power

life support

security

cargo

rec

sleep

comms

biodome

sci-lab

hotlab

structures

airlocks

docking locks

struts

walkway tunnels

space gantry

capsuletrain

cargo chute

gas transfer

Station design incorporates space utilization, life support usage, gas/liquid transport using a pressure and flow rate system, cargo management. The player must make choices that will negativly effect some areas while giving benifit in others. Choices should always be non-trivial.

Examples: Having airlocks on every module means it is faster to access space for repairs, but it is more difficult to defend against attacks.

relying on a single main pipeline to move air around the station is cheaper but what if it fails.
