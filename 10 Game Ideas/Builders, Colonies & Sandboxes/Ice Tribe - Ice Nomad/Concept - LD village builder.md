---
title: "Concept - LD village builder"
source: "Game Stuff/Game Ideas/Concept - LD village builder"
modified: 2013-11-16
type: design-doc
area: jam
status: "designed"
projects: ["[[Game Jams]]", "[[Ice Tribe - Ice Nomad|Ice Tribe / Ice Nomad]]", "[[City & Colony Builders]]"]
concepts: ["Ludum Dare", "Ice Tribe / Ice Nomad", "LD Village Builder"]
words: 713
summary: "Design for a Ludum Dare village builder based on Ice Tribe: job bins, tick-based days, mealtime phase, hunger system, journeys, survive 100 days, plus component/task breakdown."
tags: ["area/jam", "project/city-colony-builders", "project/game-jams", "project/ice-tribe-/-ice-nomad", "type/design-doc"]
---

Draws on icetribe

simple build up and victor condition

villagers can be put into “job bins”

tick based gameplay

at the end of so many ticks the game pauses for “mealtime”

player chooses what to cook/eat and if there is no food can cook a villager

jobs can only be changed after each meal

hunters are gone for several days and then return

when villagers have completed a job they will wiggle and the player can click on them to see what they did

injuries can reduce the options for villagers

job bins start out as builder job bins until the job is finished then it becomes a different bin

visuals

as the sun rises and sets, the background shade changes

inventory is shown on the village screen, with items piling up around the huts

job bins

building: constructs new job bins

cook: converts food supplies into better food

scavenger: collects random items in batches

hunter: is removed from the village and returns after a random number of days with a large haul

crafter: moves non-food objects through the process chain

victory conditions

survive 100 days

components

three types of job bin

changeable each day

type 1: disabled while busy (hunters).

type 2: completion adds to a total

type 3: completion vends an event

villager

draggable after mealtime

clickable once a job is finished

boolean abilities for each job (can hunt, can gather)

1.  Job bin entity

    1.  Type static class for bin varieties

    2.  Rendering to screen

    3.  number of slots for villagers (max array length)

    4.  work completion variable

    5.  max completion threshold

    6.  callbacks when completion value reaches max

2.  Villiger entity

    1.  Container variables in job bin ent

    2.  Rendering to screen

3.  World Clock

    1.  global variables for time

    2.  callbacks at 2 points in day

    3.  sky color change to tell the time

4.  Villager timers

    1.  game pausing with input blocking

    2.  time modification (speed up)

    3.  ui display for villager timers

    4.  Callbacks on completion

    5.  villagers wiggle when ready

5.  Villager boolean skills

    1.  Job bin skill requirements

    2.  Villager gets events from job bin on completion

6.  Events class that generates events from xml

    1.  Event functions include modifying values inside job bins and villagers

7.  Inventory system

    1.  Commodity entity

    2.  Display resources on screen

    3.  Events modify resources

    4.  Events modify villager skills

8.  Content package for jobs

    1.  Scout Hut - adds random resources

    2.  Sawmill - collects trees

    3.  Hunting Lodge - adds food resources, chance to lose hunting skill

    4.  Building Site - turns job bin into another job bin. uses resources

    5.  Kitchen - converts raw food into edible food for mealtime

    6.  Toolmaker - converts resources into tools

    7.  Campfire - generates moral for other villager at the fire. Fast cycle time

9.  Mealtime Phase

    1.  phase ui display

    2.  food inventory display

    3.  drag food to pot to cook

    4.  drag and drop villagers to bins

    5.  upgrade slots in bins using tools (click on empty slots to buy)

10. Hunger system

    1.  Villagers have nutrition, healthiness and fullness

    2.  Villagers die if healthiness drops to zero

    3.  nutrition above 90 heals

    4.  nutrition below 20 kills

    5.  fullness above 90 and below 50 kills

    6.  villagers always eat the whole feast you select

11. Journey Job Type

    1.  boolean state for job hut type

    2.  this type of job makes all villagers in the hut invisible

    3.  this job takes an indeterminate time to complete

    4.  all villagers return at once and yield a collective result

    5.  one event is generated from the event list

    6.  result is based on collective skills

12. Victory Condition and difficulty

    1.  survive 100 days

    2.  difficulty from your villagers getting injured

    3.  

Gameplay example

Player will start the day by allocating jobs while paused. This is the only time you can interact with the game while paused. Then the day starts and the player can interact with everything. As the sun sets, vilaer are moved to the campfire to recharge moral.

Hunting and logging parties are sent out and can take several days to return. They bring back large amounts f resources.

Juries and work lower the morale o-f villagers. Death costs villagers a lot of morale.
