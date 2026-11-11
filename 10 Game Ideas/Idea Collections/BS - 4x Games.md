---
title: "BS - 4x Games"
source: "Game Stuff/Game Ideas/Big Five/FourEcks/BS_ 4x Games"
modified: 2020-10-24
type: design-doc
area: game-idea
status: "designed"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]", "[[City & Colony Builders]]", "[[Elite-like Space Flight & Trading]]", "[[EVE-like Player Economy]]", "[[Player Market Hoardmode]]"]
concepts: ["FourEcks / 4X Space Empire", "Design: Colony Scaling", "Design: 4X Maintenance Costs", "Design: Lazy Star System Generation", "Design: Fuel and Drive Types", "Design: 4X Technology Rules", "Elite-like space trading", "Industry Space Game", "Player Market Hoardmode", "4X War Exhaustion and Stalemate", "4X Pop Opinion", "4X Empire-specific Resources", "4X Explore Expand Exploit Exterminate", "4X Simulated Tactical Combat", "4X Infrastructure and Maintenance Decay", "Design: Lazy Procedural Generation", "Design: Tech Trees", "Neumon Industry Space Game", "Design: Economies"]
words: 5901
summary: "Long design notes for the FourEcks 4X: colony population/district/density mechanic (tries 1 and 2), simulated tactical combat, maintenance cost decay, lazy procgen of star systems, fuel and drive types, tech rules, plus an Elite clone idea and an industry space game with waste products, bond stores and Neumon threat."
merged_versions: ["Game Stuff/Game Ideas/BS - 4X Various Ideas"]
tags: ["area/game-idea", "project/city-colony-builders", "project/elite-like-space-flight-trading", "project/eve-like-player-economy", "project/fourecks-/-4x-space-empire", "project/player-market-hoardmode", "type/design-doc"]
---

## Aim

A colony mechanic which:

- Scales for colonies of 100,000 up to 100’s of billions

- Limits player micromanagement

- Offers player choices regularly

- Grows colony power over time smoothly

- Promotes slow changes

- Offers interesting trade offs between on-world and off-world upkeep

- Models overpopulation and unemployment

- Colony output as % of population drops as population increases

## Try 2

Planets have a number of notable regions.

Each region has a size, which dictates how much infrastructure it can have in the end.

Each region can have a district plan chosen for it, which determines maximum infrastructure for each of the 5 areas.

This means you can have large planets with 1 region (low options, but high potential) or smaller planets with many regions (finer control, lower potential).

When colonizing, the first region is where the colony starts.

When a colony reaches a certain size, another region becomes eligible for a district, which can change the direction of the colony.

The colony has a density multiplier, which multiplies the total infrastructure.

Density multiplier increases Service needs of population, and lowers birthrate.

The player chooses to expand land coverage or density.

Colony population is measured exactly (64bit integer)

Biosphere hostility applies a penalty to Population needs.

Atmosphere Hostility determines how expensive density increase is.

Terrain hostility determines how expensive land area increase is.

## Try 1

Resources

Material

Amenities: Created from Material via Service

Products: Created from Material via Manufacturing

Knowledge: Created from Material via Science

Districts

When you “buy” a district it costs Products

If there are no slots available, then you can replace an existing one.

This undoes the effect of the old one and adds the new one immediately.

Districts increase:

- max infrastructure

- max allocation percentages

- Population upkeep

Colony System

Properties

> Population value
>
> Workforce value
>
> Infrastructure values (per resource max, current points, max points)
>
> Workforce split (per resource current allocation)
>
> Growth Rate
>
> Absorption/Education/Assimilation Rate

Growth rate increases Population

Absorption rate increases Workforce to match Population

If population is higher than infrastructure, then the remaining population cannot work.

If population is lower than infrastructure, then the population works a balanced amount of jobs.

Infrastructure costs Materials and is created by Infrastructure allocation.

Infrastructure is increased in two ways.

- over time based on the % of production dedicated to increasing it.

- In fixed blocks called districts

Colonies also have a population density value, which is a power modifier on population value.

Density 3 = 100’s of pop

Density 4 = 1000’s of pop

Density 5 = 10,000’s of pop

Density 7 = millions of pop

Density 8 = tens of millions of pop

Density 10 = billions of pops

A planets density is upgraded by building particular types of district. These only become available when a minimum of 1^new density population is on the planet. The new population and infrastructure is calculated after the project is complete.

Production of population is allocated by sliders

- Extraction

- Services

- Science

- Manufacturing

- Infrastructure

The player sets these sliders and then they slowly adjust towards the set values. Sliders moving consumes the over-time infrastructure income.

Planet System

Planet habitability is displayed as Planet Hostility, which applies a modifier to two things

- Service production cost (Resource -\> Service conversion rate)

- Cost of infrastructure increase (both fixed cost and ongoing types)

Each planet has a different Hostility for each species.

Planets have a size value which determines how many districts you can build on it.

Aim: Write a abstract for 4 games in the 1x category. Explore, Expand, Exploit, Exterminate. Each should aim to be as detailed as Master of Orion II, with scalability options that dont require AI governors

Explore

Expand

Exploit

Exterminate

4x ideas

Complex universe generation. Simple Gameplay

Tactical combat without direct control. The player can simulate battles against ship designs he has encountered with medium acuracy, or if he has stolen those ship designs with high accuracy. Space battles are played out in one instance, the players only being able to watch a replay of the battle.

Ships follow a set of instructions pre-written by the player. These are written per opponent empire and can be tested in the battle simulator. Players mark priority ship designs, design fleet layouts/formations and other engagement/retreat strategies.

Players could opt to have their ships perform below maximum efficency in the first few engagements so that their opponent is lulled into a false sense of security.

Ships should always be able to disengage from battle. However when an empire has better interception technology the retreating force should always be put at a disadvantage for later action. Penalties for hasty retreat could be: stealth penalty, bonus to being tracked, capability leakage, mission intel leakage. Engagement strategies could be drawn up to promote damage to fleeing ships or to conserve ammuntion that wouldotherwise be wasted.

Infrastructure Development. In most 4x games the only options for attacking a players infrastructure come from attacking his planets, or his fleet. These are often the only two things that players spend resources on to develop.

I would propose to have a rigid developable logisitcs infrastructure that can be customised to the players empire. This could be hampered, damaged or destroyed like planets and fleets.

Players should spend resources to develop this infrastructure in different ways. Each upgrade or modification effects another element of the overall system negativley (even if this is only by increasing the maintenance costs). Every opportunityu to upgrade is a real choice, one which cannot be taken back easily, and that becomes an assest that can be attacked/damaged/destroyed.

Maintenace Cost idea. Everything has a maintenance cost. This not only balances players of different power levels, but means players have to weigh the ongooing cost with the immediate cost.

I propose that maintenace costs for each fixed asset reduce over time as long as that assest is not modified or mothballed. If anything with the assest is modified, the maintenace jumps back up to a percent of the original value. For Example// a ship design is used over a long time. Its maintenace costs slowly reduces as the parts become commonly available. If the design is modified and all ships refitted with the new changes, the maintenance goes back to its original value (maybe higher). Perhaps the rate of maintenace decay can be related to how many of those ships are produced (simulating spares being produced along side the actual commisioned ships).

New technolgoies could also work this way. As a technology is released to the public over time its maintenace is slowly reduced. The most systems it is utilized in, the faster it is reduced. Options to commercialise the technology or to release it as free knowledge to the public could also reduce the maintenace at different rates while giving a penalty to protecting this technology from espionage. Doing this with a ship design could allow you to support a massive fleet, but enemies could analyse the design for weaknesses and produce countering fleet very easily.

Macro or Micro control  
Should the player control the actual development of the empire or just be abke to guide it along? Should he have u;ltimate control over the population or can they rebel against his wishes? Can every tiny detail be controled every turn or will the player have limited "action points"?

More things to spend money on: Empire, System, planet, city wide policies. These should be represented by a physical point of conflict. Example:// the player impliments a system wide cargo hualer saftey inspection program. This gives a penalty and a benefit to all trade and logistics in the system (including alien traders not part fo this empire). Over time Saftey offices build up at all orbital installations which can be attacked to reduce the efficency of this policy.

Priority Proceedure Generation

Proceedurally generated Star systems could potentially use up a LOT of space/memory. To generate a sizable universe could be disasterous. I would propose to generate system data as it is required, spreading this load over a long time. Many systems will never have anyone visit them, and many more will never suffer close scrutiny.

At universe generation only star mass (and subsequently color, temperature, lifespan) are generated.Posistions are randomized and set using a spiral/cluster/belt system.

When a player has "sight" of a system the amount of free mass that is availble for planetary bodies is calculated. This is further developed into what kinds of bodies are present. The first check is to see if there is a rocky planet within the "habitable" zone of the star. The number of other rocky planets, gas giants, asteroid/Ice/dust belts, protoplanetary discs and other things are calculcated but only as quantities.

As players can get this much data it qwould be rear to see them try to visit every solar system in range. As they will discover, defending and colonizing many worlds can be untenable. The best way should always be to colonize the best available systems.

When aany ship arrives in the solar system, planet placement is completed. Orbit distance and period is discovered. Moon quantities are also generated.

When a planet is visited, or a LR survey ship comes into the system, Planetary atmospheres, radius, densisties, ect are calculated.

When an extensive survey of a world is completed, mineral compositions, weather patterns, tectonics, lifecycle all become known. This should be the most expensive survey possible (time AND resources)

Fuel Opportunities

Radioactives, Ice Harvesting, Gas collection, Solar mining, solar power, Exotic matter, anti-matter, biological nutrients. Different species/empires have different methods of generating fuel for space travel. Some require mining of rocky worlds, some need gas giants present. This will make each system have a different value to each empire. Often it would not be benifical to capture a system that is viatal to an enemy as it holds no real value to your own empire. Without fuel generation built in systems a craft would have to carry enough fuel for its entire trip and any subsequent combat it gets involved in. Some systems could be set up to be mearly transit/fuelling systems. These could be srtategically important but not have a lot of expensive infrastructure.

Different Drive requirements

Perhaps each differing space drive can have limitations. a simple powerful reaction drive could go anywhere, but cannot exceed the speed of light. Hyperspace might not be uniform and such sertain systems could lie in turbulant areas of hyperspce. This would make certain locations in realspace accessable more easily to different races.Certain drives might not operate in nebulae, or can only jump to stars of certain mass. Perhaps some can exit a craft near a planet, while others leave the craft to complete a long sublight flight form the oort cloud. Systems with very distant boundaries would be less useful for a species with this kind of drive technology. Energy/Mass transfer drives would require complex starlanes mapped out previously, while point to point wormholes might require large infrastructure in both systems. Combine this with the different fuel types and the universe becomes a very interesting and complex place.

Points of conflict move throughout the game (through nmew technology needs, conflict orother means)

Resources and technology linked. EG// Researching gravity at some point needs a black hole.

no tech redundancy. Technologies should always be useful on some level.

technology theories. These are the hurdles required to be overcome to enter new tech areas

technology dependant on infrastucture. If all the facilites using a tech are destroyed then the technology required to build them takes a setback. If a civilization has its technology infrastructure destroyed it may lose theories as well.

Technology needs to be attackable.

Levels should fluctuate throughout a game, not continously go up and down. EG// during wartime technology should shift towards combat technologies, then back again. Theories discovered during these times can be used for peacetime technologies as well.

most empires should be in the same "technology level". Keeping empires from dedicating resources to advanced theories should be a viable strategy.

Cities and Colonies should be two sepearate things. Players cannot micromanage colonies, only make sure their demands are met. Cities can be manipulated into developing how the player likes, since very high grade planets are so rare.

Combinations of celestial bodies and thier placement in a solar system should be important. EG// A habitable world is nice, but one in system with Gas Giant or Asteroid Belt (or both) is worth much more)

Access to rare phenomena should give an empire unparalelled bargaining power, but also attract more powerful empires to attack. Most should be useless at the start of the game. Players can see what is available and select appropriate technology paths based on whats nearby.

Systems with no value should not be generated.

Other ideas for ELite "clone"

Like DopeWARs, players can change location in the game instantly. Destinations are selected before undocking and ETAs are calculated. Starship flight is not modelled at all.

Other ideas for Industry Space game

WASTE PRODUCTS! Important. These can have some value when refined, and even a process to extract the maximum "waste" material from an ore if it is the waste material the player wants. These should always be produced in large enough quantities to be a concern. Players might even be paid to dump them elsewhere. Of course showing up with a waste refinery looking to make some quick cash, while bumping up the threat value of the fleet (concequently costing the primary producer more in defence contracts) may be frowned upon.

Waste products also open up the possibility that another industrial player will start another defence contract (low paying of course). This promotes more gameplay and eventually there may even be competition for the waste goods.

Waste products should be refinable into commonly used ingredients. These ingredients should ALWAYS be available for manufacture more efficently some other way. Those more efficent processes should produce other waste products, keeping the cycle going and causing price interdependancy.

Bond Stores. Got this idea from how Rum is made. Some chemical reactions happen instantly, some require catalysts and some, like rum soaking up tannins, must be started then left untouched for some time.

Bond Stores could be used for some processes. Industrial players will need to factor in the price of starting the process, then also defending the storage vats until the reaction is complete. Some of these reactions could take days or even weeks, but generate very low threat. Better yet, the process might not take a fixed amount of time, meaning the industry player needs to come check (or pay someone) if the reaction is complete.

Bond Stores also help to keep the economy from slingshotting back and forth. Players cannot stockpile some resources and wait for a patch to one ship or weapon when they have to keep ingredents stored for days at a time. This would work very well to promote speculation as well, since the industry player has to think about when to start the reation, and to cancel it would spoil the lot. If they guess wrong, it is still worth selling the goods instead of refining it into its base materials.

ONE WAY REACTIONS. It is nessesary that SOME processes cannot be reversed. This should stop the industrial players from "getting a refund on bad choices". A certain portion of the economy should be liquid, and a portion "viscous". Perhaps keeping the top end amnufacturing recoverable but with a high cost for recycling.

Recycling final equipment (Ships, Consumables) should yeild 50%

Recycling Equipment (Hulls, Ship systems, weapons, drive units, reactors) should yeild 40%

Recycling construction components (processors, beams, plates, routers) should yeild 30%

Materials below this in the chain should be divided into recyclable and non-recyclable. Metallic compounds will of course be recyclable, but some alloys should not. Non-recyclable materials can be recycled through other processes, but these should yeild a lot of waste materials.

Industry Space Game system layout

sun, rocky world, gas giant, ice world, outer planet, asteroid belt

Sun

Neumon Solar Plant

Hothouse rocky world (venus like)

Barren rocky world (no atmosphere)

Barren Moon

Dust ring

Hot core moon

Neumon Deepcore mining operation

Asteroid Belt

Gas Giant

Icering

Higher threat neumon activity

Several Rocky Moons

Protoplanetary chunks (sparse asteroid belt)

Low threat neumon activity

Lagrange Point Station

Larger moon (twinned planet)

Ice planet at far reaches (long, eccentric orbit)

Neumon stealth probe base

Threat should increase faster in parts of the ring more easily accessed by nemon bases.

Threat should increase faster the closer you are to the sun.  
Slightly eccentric orbits on all worlds will make Threat multipliers fluctuate.

Neumon Bases/Outposts get developed over time. There are many types of these:

At Asteroids:

Surface blisters serving to repair/rearm Neumon devices

Subsurface mining outposts. Transports will arrive to ferry materials away

Ambush bases. Devices bury deep in the asteroid waiting for miners to venture past

Full conversion. The asteroid is mined out and transformed into a free floating neumon manufacturing outpost

At rocky worlds without atmosphere:

Deep core mining operations, undetectable and unremovable

Surface blisters build up for Heat Sinks, Docking ledges, waste ports, repair and rearm stations, point defence weapons.

Different blisters have different effects on the surrounding Threat Multipler

At Ice/dust rings and Gas Giant atmo:

Scoop stations colleting particles

Docking platforms for tankers which go out to collect from the collectors

Refuelling pods for passing devices to refuel at

At the Sun:

Solar plants creating super capacitors and other high energy components

Researching higher technology items

Eventually players will want more advanced equipment. New designs for equipment and ship hulls will came on the regular supply caravans from Earth. Other refinements can be made by collecting large amounts of undamaged Neumon components. Neumon components are found in all Neumon devices but undamaged ones are only found on transport devices. Of course the only places to intercept these transports is when they are leaving or arriving at Neumon bases. This could give combat players good reason to risk their equipment to attack fortified bases, appart form just keeping threat multipliers down.

---

## Differences from other versions

_This document existed in several versions. The text above is the most complete one, unchanged. Below are the lines that appear only in the other versions._

### Only in “BS - 4X Various Ideas” (Game Ideas, modified 2021-10-10)

War needs to fall into stalemate after a while.
- Fleet distance from a colony determines its cost to move
- Both sides suffer exhaustion until they can not take a starbase
- Exhaustion reduces damage dealt to opponent but also damage taken from opponent.
- Cost to give aggressive orders increase over time.
- Ships return to home system point when their order is finished/cancelled.
- Defend system is an order, separate from the home system.
- Ships need a line of supply to their home system otherwise they suffer malus.
- Changing home system takes time and other resources.
- While at war, military upkeep is higher.
- While at peace, aggressive orders cannot be given.
- Threatening empires are always at war with everyone, and so can always make aggressive moves against neighbors.
- Defenders against such threatening empires do not suffer war exhaustion until they declare war.
- Once war had been declared, the threatening empire starts to accumulate exhaustion
- While nobody is at war with a threatening empire, exhaustion goes down.
- 
Pops have opinion of other pop species.
- Compatibility traits
- Opinion of Empires with leaders of that species are different.
- Having pops that don't like each other on the same planet causes happiness problems
- Wars effect opinion
- Ground battles and bombardment effect opinion
- Differing living conditions effect opinion
- Neighbouring system governor's and trade have an effect of happiness based on species
**Empire specific strategic resources**
Tech has breakthrough nodes which unlock empire specific resources. Knowledge of these resources and their locations is only available to that empire.
Expand gameplay abstract
Exploit gameplay abstract
Explore gameplay abstract
In general, controllable space should have different value for each empire. The highest value available is your own homeworld.
This could be that some empires don't use some resources.
Military or authoritarian citizens get upset if you compromise of making the best choices.
Pacifist citizens get upset if you choose options which involve combat or annexing.
Planet size is broken into biomes. Each species can settle different biomes. To 100% utilize a planet you need multiple species, or genetic diversity. Species should have their own demands, so that producing a new variant of your base species results in more problems.
Aim: Write an abstract for 4 games in the 1x category. Explore, Expand, Exploit, Exterminate. Each should aim to be as detailed as Master of Orion II, with scalability options that dont require AI governors
Each player only controls the exploration ships of each empire. Finds are catalogued and resources are marked for pickup by empire traders.
During war, science ships act as recon. Stealth gameplay is used where the player can mark enemy ships to assist with Intel and combat operations.
Your empire expands behind you, exploiting the resources you found, although this is not simulated in a detailed way.
