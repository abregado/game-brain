---
title: "Concept - Dark Space Multiplayer Room"
source: "Game Stuff/Game Ideas/Concept Docs/Concept - Dark Space Multiplayer Room"
modified: 2015-06-22
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Elite-like Space Flight & Trading]]", "[[Player Market Hoardmode]]", "[[EVE-like Player Economy]]"]
concepts: ["Dark Space Multiplayer Room", "Design: Asteroid Mining System", "Player Market Hoardmode", "Design: Cryopod Player Cap", "EVE-like player economy", "Design: Passive Income Structures"]
words: 4536
summary: "Large concept for DSMR, a Meteor/web multiplayer take on A Dark Room in space: long and mini missions, job board, pre-flight checklists, cryopod permadeath, player market, mining, ship, fuel-rod consumables, task steps and passive income round 2."
tags: ["area/game-idea", "project/elite-like-space-flight-trading", "project/eve-like-player-economy", "project/player-market-hoardmode", "type/design-doc"]
---

# 

Dark Space Multiplayer Room

That Meteor game Idea I was talking about

By Ben Buckton

# 

# 

> [*Narrative Example*](#narrative-example)
>
> [*High Level Concept*](#high-level-concept)
>
> [*Initial Content*](#initial-content)
>
> [*Environment*](#environment)
>
> [*Framework Technologies*](#framework-technologies)
>
> [*Other Ideas and Notes*](#other-ideas-and-notes)

# 

# 

#  

## Narrative Example

You log in to see a few other pilots already plying the local asteroid belts. You check the job board. Looks like there is a pilot in trouble, he is being attacked by a few pirates. There is also another pilot requesting pickup of freshly mined ores, and he is paying more.

You run down to your ship, a jack-of-all-trades Privateer model. Your copilot is asleep in the cockpit and the others are nowhere to be seen. You wake him and tell him to start replacing the fuel cells. One of the other crew members is found nearby in the cargo lounge, you send him to find the others and head back to complete some other pre-flight checks.

Finally you are in space, flying towards the transport job. From here on its all up to fate.

## High Level Concept

DSMR is a multiplayer take on A Dark Room. Each player interacts with the game world through the simple interface, either completing tasks himself or by assigning his NPC crewmembers.

Some components of the game require short interval, interaction heavy gameplay followed by long periods of “autopilot” gameplay. During these periods where the player has no control your success will be based on the interactions of other players. The overarching idea being that players who prefer low interaction gameplay generate more gameplay opportunities for those that prefer high interaction gameplay.

An example. Player 1 sets up a mission to strip mine a nearby asteroid. Setting up the mission and launching is a short (10min) high interaction experience, but once the mission is underway the player cannot interact for 10-20 hours. During this period of low/no interaction, events occur which offer short, high interaction gameplay to other players. Some pirates might attack, or the mining ship might require emergency repairs. The mining player can set reactions to these events, including price offers for players to assist. Player 2 logs in and sees a list of available “mini-missions” and can choose to assist or to start his own long-term mission.

Long Term Missions are complex affairs, with many settings. Players who undertake these should try different configurations to see what works best for them. Once a LTM has begun, the only option available to the player is to return home, which does not immediately end the mission, but shortens the time until the player can select a new mission.

Mini Missions are mostly set up for the player when he/she selects it from the job list. There are still some simple options. Here the gameplay comes from completing the pre-flight checklist as quickly as possible, as tasks often pay a bonus for completing them early. Once the pre-flight gameplay is complete, these missions take 5-10 minutes of low interaction gameplay to complete but may be interspersed with one or more sessions of high interaction gameplay.

## Initial Content

As a proof of concept, the game would include an interactive Introduction movie, which would explain the prelude of the game. This will get the user acquainted with the UI, and demonstrate roughly what to expect from their gameplay experience.

As for initial multiplayer content, the players will be engaging in four main tasks. Scooping Gas from a nearby Gas Giant (medium length), Transporting refined fuel from the Gas Refinery (short length), Surveying objects of interest (long mission), and providing Military support for those completing other missions. The longer missions should be the most lucrative to incentivise players generating content for others. Scooping Gas is the entry level mission, which is always available.

## Environment

DSMR takes place in orbit around a moon, which is orbiting a Gas Giant. There are many other objects in orbit around the Gas Giant, and further out there is an asteroid belt orbiting the local sun. Each object has its own orbit, and everything moves in real time. The length of missions will be dynamic due to the movement of target objects. To begin with locations will be static, but once the basic gameplay is implemented, dynamic locations will be a high priority.

## Framework Technologies

There are many components that need to be built for this project to succeed, but I feel this is doable for one person.

- User Interface

  - Tab structure

  - Button

  - Timer

  - Login/Out elements

  - Mission Option Selection

  - Job Board

  - Preflight UI

  - Mission In progress

  - Station Control and Information (stats board)

  - Debriefing screen (saves last 3 missions)

  - Wallet and Crew

- Audio

  - Simple sounds for task completion

  - Alerts when input is required (combat, emergencies)

- Account/User Authentication

  - Username

  - Email

  - Password Recovery

- Data Structures

  - Jobs - Missions that are waiting to be accepted

    - var: timeout, how long the mission is available for

    - var: Ship Object, the type of ship this mission needs (players get the appropriate ship automatically)

    - array: Pre-Event Objects, These contain controls to modify Events, which are passed to the active Mission constructor.

    - var: positions, how many times this mission can be taken before being unavailable

    - var: owner, who owns this job

    - var: public, if this job can be taken by anyone

  - Sorties - missions that are in progress

    - array: Event Objects, which play in order

    - var: Ship Object, chosen by player and configured before the mission

    - var: public, if everyone can watch this mission/sortie

  - Event

    - var: Length, the time this Event takes to complete

    - array: Task Objects, where there is player interaction available

    - bool: notify, if the game should notify the player that the event has started

  - Task

    - var: uses, how many times this Task can be completed per Event

    - bool: startHot, if this Task starts available, or if it needs to cooldown

    - bool: playerControl, if false, this task is invisible and will auto complete (for enemy actions, and random events, or those without)

    - var: Timer, a timer until this task is complete

    - var: Cooldown, a timer until the task is available

    - var: onSuccess, what happens when the task is complete, including unlocking other tasks

    - array: skills, which skills are needed to complete this task. Determines which crew can complete this task

  - Timer

  - Result

  - Inventory

    - array: typesAllowed, which cargo types are allowed

    - var: volume, how much space is available

    - var: mass, how much the total cargo weight is

    - array: cargo, a list of the cargo items in this inventory

  - Ship

    - var: available, if this ship is available for player use, or if it is in use by a player

    - stats - lots of stats

    - array: Inventories, a list of the Inventory objects associated with this ship

- Server Methods

- Game Logic

  - Wallet Object

  - Ship Costs (Rental, Repairs, Fuel)

  - Flight Time (undock, sublight, FTL, adjustments, orbit curvature)

  - Buy/Sell Prices (must be adjustable by “Master Character”)

  - Orbit location based on server time

  - Modular design so new mission types can be created with ease

  - As more mission modules are created, exponentially more options become available for content creation.

- Pre-Flight Checks

  - Complexity and Progression design

  - Must open up

  - Variable length, smaller ships require less time and are simpler

  - Maze-like solution

  - randomise initial conditions

  - Each task has one or more prerequisite tasks and a list of crew that can complete them

  - Captain can always complete tasks

  - Task chains depend on multiple professions to promote forward thinking

  - Timeout on tasks (only available X seconds after Task Y was completed)

  - Display preflight checklist Final Items, with next step underneath

## view current mission

a separate screen to view your current mission in more detail. proper one mission only detection.

## replacing death

instead of ship destruction, which wuld effect the whole server and be open to griefing, players who gamble and lose instead are penalized with inconvienience.

A damaged ship limps home much slower than if it had completed its mission. the pilot must pay for the repairs. Messages of what happened to cause this are sent to the player, so thye know why thier mission isnt finished yet.

## pre-mission setup

client retrieves job data from server via method, and sets that mission to be unavailable until a timer has passed.

method returns job details and tells the client how long the job is reserved for

user modifies mission parameters on the client and then clicks 'launch mission'.

the client sends the modified job to the server for validation, and if validated converts it to a mission.

## event modification

each event has a number of variables which are passed to the client. these are given min/max values that can be modified and then returned for validation. The equations for actual effective stats are known by client AND server, only being used on the client for the modification ui. The actual numbers are recalculated on the server before the job is turned into a mission.

each modifiable variable knows if it is modifable with dropdown, slider or input. if dropdown, the server will tell which options are available for that dropdown.

for often used options, custom ui will be generated from the client. such as lists of ore to ignore, crew quantities, ect. these are sent using an array of keywords. If the client recieves a keyword it will show that ui and expect a response for validation.

## Cryopods - A spawncapping/permadeath system

There are limited cryopods on the station. Each represents a player space on the server. This is effectively a Player Cap. However, every player can see who is active on the server and how long those people have been inactive for.

If a player has not logged in since 3 weeks then everyone can see that their cryopod status is RED. other players can make a choice about RED cryopods.

Choice 1: Renew the cryofluid, which extends their storage for one week. The pods status is changed to GREEN and nobody can effect that player anymore (for another week). This takes ~5 minutes of idle gameplay.

Choice 2: Dispose of the body. This takes much longer (~2 hours). The player in cryo has their character and records deleted and will wake up in a new body when they log in next, if there is available spaces.

This game idea also goes with a new player experience wherein they must be active twice in the next 24 hours, followed by 3 days of inactivity.

## task generation

write task foward, but generate them backwards

- per use resource cost

- on complete resource use

- job restrictions

- 

## The player market

how to bring a player market to this game?

only one purchasing player, starting as a dev

that player is the only one who can set prices and have bulk cargo

this player also sets prices for cargo storage

players never own anything, just have money?

where does the demand come from?

- player consumables: fuel, repairs, ammunition, replacement parts

- artificial demand external needs: the station consumes lots of extra resources.

how are resources converted?

- the station converts at a fixed rate

- npc trade ships buy raw and sell advanced resources.

resource types

- resources that only the station needs, these create competitive gameplay

- resources required for player expenditure

- enabler resources which allow other resources to be converted

# players owning thier own ships

ongoing costs per ship (hanger rental)

owning your own is not useful unless you are very active

the house/station sets prices for all vehicles

if selling and then renting hangers can make more money than just renting the ship, why not

normal players access to ships?

always some public ships available?

maybe long term rental instead of buying?

what happens if player cant pay rent?

hanger rental period length?

## mining system

asteroids have a number of locations each an angle from centre

each has a radius and surface area

each location has an array of rocktype-depth pairs

rock closer to the surface gets collected first

depth is inversly proportional to collection speed

if all of a rock layer is removed, the others have thier effective depth moved higher

some drill types penetrate a depth before collecting

other strip more off the top layer

all have a wastage factor

preparing and asteroid for intensive collection should be viable

ores should have

- differing densities

- smallest unit (volume)

players should have options to ignore ore types - dump to space

players can rent containers to fill, allowing others to transport them back to station

players can log in to see a progress report of mining operations

drill concepts

- boredrilling. penetrates deep but doesnt collect very fast. very fine ore size. low wastage.

- strip mining. collects lots but doesnt penetrate at all

- heat leech. collects slowly and uses more power but gives very dense and fine ore. very low wastage.

- explosives. fast, super high wastage. large smallest unit. good to break through unwanted layers.

postprocessing concepts

- melter, lowers volume lots but weight only a little

- crusher, lowers smallest unit

- sifter. recovers wastage

## ship content ideas

Service Craft. a small multipurpose vessel that can be used to ollect gas from the nearby gasgiant, repair stranded vessels, or move other cargo. it can carry two cargo containers and has a low power, but efficent ftl drive system. The station has many of them aboard and they can be refitted or repaired easily. they can also be used for survey patrols, and to deploy core samplers.

Commercial Defence Craft. A larger craft that is designed for combat to ward off pirates and other attackers. It is not very fast or powerful but can take a beating. its ftl drive is very poerful to allow quick intercepts. a rack of missiles and several imballed mass drivers are used for damage applicatin.

Military Fighter. these are not player controllable. the esort carrier assigned to defend the station has several at its dispsal. they are fast, small and deadly. easily a match for a defence craft.

Hauler. this is a larger industeial haulercraft used to transport 8-10 cargo containerx, or to deploy mining and survey equipment to asteroids. it can fit an emergency launcher if nessesary to protect from agressors.

escort carrier. A corvette class ship sent to protect the station and the gas refinery. It has small munitions factories abord and will supply munitions to players if provided with raw resources. A wing of 5 Military fighters is docked with the carrier for intercept missions and to protect company assets in the field.

## Consumable system

station needs fuel rods replaced every 10 days. There are 9 rods. a mission becomes available for each one hat needs replacing.

The station also converts ore into parts at a rate based off the number of active fuel rods. If it runs out of ore then it must cool down for a day, and then takes another day to spool up again. This process occurs even when the station has no fully charged fuel rods, but is slow.

A trade ship comes at a long interval to collect rare ore 'Osmium' and gives Fuel Rods. It offers three packages, of which the largest is taken first and offers the best exchange.

The Refinry also uses Osmium and Fuel Rods. It holds three rods but only consumes them every 15 days, and only if there wss fuel generated during this period. When gas is added it takes 6 hours to warm up and efficency increases every 6 hours it is kept running. Fuel rod missions become available as needed.

The station can only hold so much fuel. Fuel is moved from the refinery to the staion by players, and a small trickle automatically is mved when the refinery is full.

Each ship consumes fuel during missions, whenever sublight trvel is used. The fuel is consumed when th ship to the station. if there is not enough fuel, the ship is offlined. When a ship drops gas off at the refinery, it is filled with fuel. This way gas scoop missions and fuel transport missions dont cost fuel and the system never reaches total entropy.

Each ship takes random damage during each mission. When returning there is a chance the ship will be offlned based on its damage. When ending an event there is a chance of something breaking and a new event being added to the queue.

Players can repair the ships using parts. These maintenace mission are between 10 minutes and one hour. They repair a varying amount of damage and cost parts.

Ships can also be inspected for damage, which has a chance to queue a repair job but takes a lot of time. Once cleared a ship cannot be inspected again until it comepletes a mission.

Players can inspect thier ship beforehand to reduce the chances of a failure. This adds 1 hour to a mission, but reduces the chances of a failure by 80%.

Ships also need fuel rods, once per 100 days. Ships with depleted rods travel at half speed during FTL travel.

## station market screen

this lists the buy price for each resource, the amount required and the cost for station services.

the station owner can also see inputs to change the pricing for each item and service, as well as see the conversion rates and times for production units

another screen shows the weekly profit/loss statement so a decent price desicion can be made.

## Other Ideas and Notes

Strengths of Meteor

- Easy access to MongoDB

- Authentication built in

- Javascript

- Access to HTML 5 and Javascript canvas’

- Cross Platform

- Live Update

Design Considerations

- Multiplayer or at least Massively Singleplayer (1.5 Player)

- Longer response time

- No slow buildup, except to tutorialize

- 20 minutes a day gameplay

- Discourage playing constantly

- complex objects are simple to do with Collections

- 

Inspiration

- A Dark Room

- Candybox

- Various timer games

- Gnomoria

- Outpost 1 and 2

- Town builders

- Colonization

Multiplayer concepts

- trade over time

- server goals

- player control of everything

- indirect pvp

Single player concepts

- activity as a multiplier on your inactive time

- setting up 20 hrs of automation takes about 20 minutes

- efficiency gained by setting up after exactly 20 hours

- better setups require more complex set up

- cancelling a 20 hr run means taking a hit on production for that run

- play - set - wait cycle

Other ideas

- one button jumper game with elite trading at the end of each level

- if you “die” in the minigame, you cant play another minigame for 20 minutes and some of your “cargo” gets desotryed

- stocks based off eve pi components

- players convert isk into game money

- non eve players can play

- eve players can play from outside eve

- players need eve parts to build things which dont produce eve parts

- exchange rate based on value of bank assets in eve vs the amount of currency in circulation

- cost to maintain the same level goes up with level, until equilibrium

- just get more?

- contracts to trigger bonuses in game "give me x and some isk" and the game picks up on it and gives in game items.

activities

- survey belts. this generates a number of asteroid results of which one can be kept. these can be used to generate new missions. Asteroids have a single positional value (radians). asteroids have complex information. and move over time (orbit). players put trackers on asteroids to claim them. short setp time, 20-60 minute run time.

- core sampling. drill a specific asteroid to discover its contents. 1- hr run time.

- mining. select asteroid, type of mining, on site refining, cargo capacity, mining speed, warp speed. Specialize your setup for a specific resource. an asteroid can be used many times. takes 5-20 hours to complete. genertes content for others. resquest escort (price per time, price per kill).

- patrol a region. asteroids in this region gain your protection, and if attacked you recieve a fee. you can select the range of coverage and fee.

- transport. set your fee for eah container type, range of coverage, request escort (cost per run, shiptype,) also collect spot requests.

progression

- wake up crew

- find missing crew

- each crew members gets a list of jobs they can do

- jobs become unlocked as you complete others

- if you click one job, all other jobs on that crew are disabled

- preflight checklist shown as a list of tasks

- each checklist item discribes the next step underneath it

- the top crew member is you, if you are doing something, you cant give orders to others, but you have more options

smaller ships have less crew and shorter preflight checks.

mission planning

- a screen of options

- timeline at top showing mission length, and how the time is broken up *example:// 1 hour mission, 5 minutes undock, 10 mins ftl, 10 mins setup, 10 mins survey, 5 mins packup, 10 mins ftl, 5 mins docking.*

- some options only become visible after others have been pressed.

- comes before the takeoff step

- select fuel amount, ammo stocks, destinstiin, combat strategy, reactor levels.

- select escort priority (shipsize, reaction time, cost)

- set escort min/max

- refuel, rearm offer price max

- transport max price

- cargo drop size

- readyness to run away. effects packup time, efficiency of work and setup time.

asteroid stats

- diameter/volume

- ore makeup (depth, rotation, volume)

- debris cloud/ftl entry distance

- drone presence

- internal pressure

- crust density

- regolith

- surface impacts

- radioactivity

- tectonics

- 

# Tasks

Step 1

redo account creation and login

players have a cash stat

change pilot name once

scoreboard sortable by columns

Step 2

surveyed asteroids happen rarely and have a distance value

survey missions have a fixed high fuel cost

mining and transport missions have cost based on distance

fuel missions have no cost

select mission brings player to mission confirmation screen

distance, ship config, fuel use all shown

breakdown of mission parts shown

Step 3

simple options for scanning mission: fields to scan, length at each field, max distance

ship module: ftl booster, life support tank, adv scan array

allow missin start if mission time is lower that life support time

Step 4

simple options for fuel missions: scooping time, number of scoops

ship module: life support, rapid unloader, heat shield

each scoop run can have its own length set

scooping time generates a heat. at the end of each scoop, the maximum heat allowed goes down based on how long the scoop went for. the max heat is shown as degrees.

show heat max before ablation, max heat for scoop and heat at current length

display ablation before each new scoop

heat shield increases ablation limit, and increases max heat

unloading time decreased if rapid module is taken

mission start is only allowed if mission length is less than life support

mission start is only alowed if all scoops are below max heat for thzt scoop

show total gas scooped for whole mission

Step 5

mining mission options: take 8 cans of equipment, bring 8 back

Drill Rigs: more mining equipment means cans fill faster

Hoppers: more empry cans means larger tonnage of ore

Life Support: extend maximum mission length

Crushers

can pack 7 extra cans in one can, but takes time to unpack

private or public display for extra transport jobs

transport job distance based on asteroid distance

Tidy up event message generation

When new missions are made

When a pilot accepts a mission

When a pilot returns

better event message descriptions

Help tab and tooltips

sign in and create account

message timestamps displayed

show last 10 messages only

place messages at bottom of screen

login box should close automatically

game stats before logged in to entice players

scoreboard at top

rename info to scoreboard

nav tabs stay active

Client checks every 10 seconds to see if the mission is complete

Each panel has a different background to differentite

server methods

verify a job is not already taken when adding a mission

id and admin check on admin commands

client

reduce reativity if existing data is the same

space scanner counts down locally and updates when something hits zero or every 30 seconds

messages update as now, but nly fetch last 10 messages

own mission in its own subscription updates every second

scoreboard as it is now, its not updated very often.

Tutorial Single player

- find crew mission with 5 steps

- at each step you get three choices of crew

- wait timer between is 2 minutes

- choice between a combat or noncombst mission

- noncombat mission goes for 2 hours, with attention required in 1 hour

- combat goes for 30 minutes, with inpit needed every 5 minutes

- rendeveus with ftl transport mission

- player hypersleep mission goes for 2 days

- when finished, multiplayer begins

Location variable and window

- each character gets assigned to a location

- a window at the top explains what the character can do here

- use an image to give an idea

- In hanger lounge, in ship bridge, in spacesuit doing X

- each location can have a hanger and mission list associated with it

**Round 2 Ideas**

**Capped Passive Income Streams**

Passively operated structures can be set up, which will generate not cash, but resources over time. The storage of finished goods is extremely limited, but the goods are automatically placed on the player market when complete. This means that if demand is high enough, and the player sets a decent price, the structures will make a profit.

Balance can be accomplished by upgrading the cargo capacity or production speed of these structures to suit the local market. The final production and sale quantities are based on the standard cargo container sizes. Other players must purchase and collect these containers, and cannot opt to purchase single units of resources. This also means that bigger containers are not necessarily better.

The sale of these resources is automatic, and can happen while a player is offline.

However the maintenance costs of these passive structures is constant, regardless of if they are producing goods or sitting idle. Whether or not they are profitable is up to the player who owns them.

Distance from the Main station also is a factor, as this will affect the delivery time of goods. As a structure moves farther away, it will become less profitable, and thus players will need to update their locations over time.
