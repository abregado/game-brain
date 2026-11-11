---
title: "Project Moon and Living World"
source: "Game Stuff/Game Ideas/Big Five/Living World PvE/Project Moon and Living World"
modified: 2016-04-14
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Player Market Hoardmode]]", "[[EVE-like Player Economy]]", "[[Living World PvE]]", "[[Industry & Production Games]]"]
concepts: ["Player Market Hoardmode", "EVE-like player economy", "Living World PvE", "Project Moon", "Design: Industrial Craft Gameplay", "Design: Combat Mechanics (heat, ammo, repair)", "Design: Anti-botting Resource Gathering", "Design: Environmental Effects", "Design: Base Module Specialization"]
words: 6715
summary: "Long notes on a player-run-economy mech/spaceship MMO (EVE/Perpetuum inspired): 2016 revision where the server owns everything, Project Moon phase-1 prototype (rovers sampling moon regolith), economy principles (faucets/sinks, decay, localised supply, no botting), PvE for small groups, industrial craft waypoint gameplay, combat mechanics, environment and level design."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/industry-production-games", "project/living-world-pve", "project/player-market-hoardmode", "type/design-doc"]
---

> [*Project Moon: AKA Phase 1*](#project-moon-aka-phase-1)
>
> [*Necessary Elements - and explaintaions of each one*](#necessary-elements---and-explaintaions-of-each-one)
>
> [*localised supply of materials (everything is not available from everywhere)*](#localised-supply-of-materials-everything-is-not-available-from-everywhere)
>
> [*players assets at risk when they are making wealth*](#players-assets-at-risk-when-they-are-making-wealth)
>
> [*several options for wealth increase*](#several-options-for-wealth-increase)
>
> [*Gameplay value add by players playing the game*](#gameplay-value-add-by-players-playing-the-game)
>
> [*Gameplay value add by players creating game content*](#gameplay-value-add-by-players-creating-game-content)
>
> [*Safezones are not useful for anything else*](#safezones-are-not-useful-for-anything-else)
>
> [*nothing is perminant*](#nothing-is-perminant)
>
> [*controlled faucets and balanced sinks*](#controlled-faucets-and-balanced-sinks)
>
> [*each process interacts with others*](#each-process-interacts-with-others)
>
> [*VERY LIMITED npc market - nothing should be infinite*](#very-limited-npc-market---nothing-should-be-infinite)
>
> [*flat quality curve - everything is useful for one reason or another*](#flat-quality-curve---everything-is-useful-for-one-reason-or-another)
>
> [*ease of notifying others what you want*](#ease-of-notifying-others-what-you-want)
>
> [*price information is not global to encourage exploration*](#price-information-is-not-global-to-encourage-exploration)
>
> [*discourage player hoarding - tax on storage space over a certain limit?*](#discourage-player-hoarding---tax-on-storage-space-over-a-certain-limit)
>
> [*visualizations of who is holding goods in a station/service*](#visualizations-of-who-is-holding-goods-in-a-stationservice)
>
> [*goods cannot be placed into storage forever, eventually they should be released back into the game world (if a player stops playing)*](#goods-cannot-be-placed-into-storage-forever-eventually-they-should-be-released-back-into-the-game-world-if-a-player-stops-playing)
>
> [*Pve content that creates market drive on lower market tiers*](#pve-content-that-creates-market-drive-on-lower-market-tiers)
>
> [*infrastructure designed for small groups*](#infrastructure-designed-for-small-groups)
>
> [*Notes*](#notes)
>
> [*PvE content for multiple players*](#pve-content-for-multiple-players)
>
> [*Ideas to make industrial craft interesting to drive*](#ideas-to-make-industrial-craft-interesting-to-drive)
>
> [*Mechanics that could be better than current gen*](#mechanics-that-could-be-better-than-current-gen)
>
> [*Combat Mechanics*](#combat-mechanics)
>
> [*Environmental Effects*](#environmental-effects)
>
> [*Landscapes and Level Design*](#landscapes-and-level-design)

## 2016 Idea Revision - Players don’t hold items

### Server owns everything

In this version the server would own everything. Players would work to increase the “server wealth”. Players are rewarded with more power to change the game world. Currency is changed with dynamic relations, which determine both the level of items available to the player, and the amount of “voting power” on changes to the systems.

### Cash vs Relations

Here when cash is referenced it is a currency used either to loan server objects, or to be spent to upgrade relations with the server. Players can decide how this cash is spent. Relations drop constantly over inactive time. Cash stays attached to player accounts, but of course the costs for items may change over time.

### Reverse Specialization

Each Base Area starts with one of each module, giving full functionality. Modules are:

- Combat Mech Hanger (Holds 10 Combat Craft)

- Industrial Mech Hanger (Holds 2 Industrial Craft)

- Turret System - destroys enemies within range, if a base does not have one of these it cannot defend itself.

- Storage Module - Stores a decent amount of stuff for each player, amounts of each can be adjusted.

- Reactor Module - Allows players to convert enemy loot into cash

- Scanner Module - Allows players to convert enemy loot into terrain/resource scans

The starting server base cannot be modified.

Each module can be changed into any other for an increasing cost. The cost to change one module is based on the highest number of a single type.

- Base with 6 of the same module cost is very high to change the last module

- Base with 5 of the same module is high

- Base with 3 is moderately expensive, regardless if it has two different lots of 3 modules

This way was a base is specialized it becomes expensive to change.

### Construction Gameplay

When a player decided to rent an Industrial Craft it is flown into location. The player decided on the rough location of the initial craft deployment and then the craft is set underway. It takes about 10 minutes for the craft to arrive. Before launching the player has to chose which items he will attempt to construct by choosing a Blueprint.

While in transit the player can configure his factory design. The blueprint shows inputs and outputs and what the last setup managed to build in a given timeframe. The values from last time must be exceeded to level up the blueprint.

### Instant Sale only

Only items that can be sold at bases can be sold and is done so instantly. Excess is purchased at FAR lower prices so it is basically always a total loss. The amounts of items that can be stored in a base is based on the number of storage modules available.

### Instant Buy only

Combat Players cannot buy items and keep them stored. Mechs and Combat Craft are “leased” and materials are purchased at a fixed price before being deployed. Left over equipment is bought back at the same fixed price.

###  

After so much EVE and lately Perpetuum I decided to write down my ideas for a player run economy game. Its a waaaay to big of a project for one guy to complete in a reasonable time frame, but none the less, its my dream project :D

Mechs or Spaceships, take your pic

### Project Moon: AKA Phase 1

So Phase 1 for this design would be to create a multiscale, procedural level generator that can produce a believable representation of the moon. During this phase a heightmap and random diffuse map (resource strength) are generated

There is only one structure on the moon. This is the Rover Base. Here the players spawn, and here is where they can “safely” log off. I say “safely” because there will be no threats on the moon.

Players can log in, or the game can create a guest account based on their IP address (is this even legal). Each player gains control of a Rover that can only do two things. One is move about the surface of the Moon (limited capabilities). The other is to collect a sample of moon regolith.

Do complete this task, the player moves his Rover (WASD) or by creating waypoints with the mouse. Once he finds a spot he wishes to sample, he simply clicks on his rover. The sampling task takes 1 minute to complete and then the Rover has a Moon Rock item added to its inventory.

Each Rover can only carry one item at a time.

If the Rover returns to the Rover Base, then the result of the sampling is added to the collective map.

Players can zoom out to see a map of the area. Spacebar jumps from the map to the zoomed in mode (Homeworld map).

Each Rover has enough power to move continuously (to collect samples) for 1 hour. Then it must power down to recharge with its Solar Panels. If returning to the Rover Base then a Rover can be recharged in only one minute. If using Solar Panels then the Rover will take 8 hour to recharge.

The day/night cycle of the Moon should be realistic ~27 RLdays of day/27 RLdays of night

If your Rover is trapped out at night time and cannot return, then it is stuck for 27 days.

When at the Rover Base, the map can be zoomed out farther and all Rovers are marked on the map.

It is important at this stage to make all the code re-usable.

map graphics will be a grey heightmap with green markers for ROvers. When zooming in the terrain will be visible as a grey heightmap (3d), the rover will be a simple lowpoly model.

### Necessary Elements - and explaintaions of each one

#### localised supply of materials (everything is not available from everywhere)

each task/gameplay element has a single unique resource type. In addition, geographical placement also effects which resources are available from “passive” resource accumulation (mining).

The layout and availability of services/facilities and the shifting denisty of players will effect the flow of resources.

Not only geographical availability would work. Times based availability could create boom and bust cycles. Also having harvesting limited to a limited number or type of players. Having the right players in your area would be attractive simply so that you have access to the resources in said area.

#### players assets at risk when they are making wealth

Any time that wealth is generated from the game world, someone is taking a risk, AND it is costing them something. PvE content always consumes resources, and every item will eventually break and need to be replaced. In a way, everything is consumable.

Players should realise that making wealth from value add and player demand is the only way to make risk free wealth. These PvP wealth players will need others to be active and taking in game risks in order to make wealth.

#### several options for wealth increase

There should be more than one way to generate wealth from the game world. Each method should have differing amounts of risk, reflex vs planning, and player skill. Those that require the most of these will automatically become the most well paid positions.

#### Gameplay value add by players playing the game

Since everything is consumable, wealth can be gained simply by transmuting non-useful items into more useful ones. Every player who is active and taking risks should be given tools to create more motivation for others to play. Sharing resources with other players should be as simple as ticking a box. Asking for help should be simple, and paying for that help (incentives) should be intuitive to set up.

There should be demand for new players as soon as they spawn. Something new players can do that others cannot?

The game should get better as more people play. There should never be a drive to move away from other players completely.

#### Gameplay value add by players creating game content

Those that want to take a risk free path will need to set up missions, contracts and objectives for those that are happy to take risks. The value added to the risk takers gameplay experience in this case is paid for through the non-risk taker. Thus there is a cost to going down this path but it also provides a service.

#### Safezones are not useful for anything else

Parking your vehicle is only for the sake of parking. You cannot do anything while safely parked in a facility. This would be mostly for logging out, and switching vehicle. Even logging out can be done from the game world.

#### nothing is perminant

Everything degrades while it is being used. This could cause some database issues and a technical solution needs to be found. No items that get used should last forever, and items in storage should incur costs that must be paid by a player. If the server becomes empty for long enough, it will empty of all items eventually.

#### controlled faucets and balanced sinks

The toughest thing to control is inflation. It is nessesary so that all players can continue to be rewarded for their efforts. Since everyone needs to be “getting richer” all the time, there will always be inflation. However, expanding too quickly for no reason will incur costs (storage, replacement, repairs) so this should work itself out if planned correctly.

In economic emergencies, there needs to be some planned remedies for both rapid inflation and deflation. One solution would be to dynamically alter the cost of imported resources that are necessary for player vehicle construction. This also allows the devs to control the number of vehicles that are available in the game world.

Offering NPC market buy orders at very low prices in certain situations means that players will have to look for windows of opportunity to rid themselves of excess items. The exchange rate of these can be adjusted as the devs see fit.

#### 

#### each process interacts with others

Every resource and process should be nessesary to facilitate a health game world. The demand from one process should promote players doing another process. Some processes will interfere with one another, but are nessesary none the less. This push and pull of industrial concerns should create a political environment that is interesting, as every group of industrial players will want to make their slice of the total pie larger, at the cost of others.

This is the sort of PvP I would envisage for this game. Market and Political PvP.

#### VERY LIMITED npc market - nothing should be infinite

Resources can move in and out of the system. Unlike in other player economy games, this is not a constant truth, as these opportunities will be limited in time and availablity. NPC buy orders will be in high demand, and function more like an auction system. Every player who wants to take advantage of the situation will need to make a bid, and the lowest price wins the contract. However, if the contract is then not filled, that player is banned from making bids for a long time.

converting “bounty items” to liquid money takes time in the game world. Your avatar must stay in one area and is vulnerable during this time. Enemy NPCs spawn continuously to attack you. Bring a friend when you want to cash in.

Opportunities to buy also work this way, players can bid to pay the most for the whole batch.

A number of the top bidders win the contract at the same time. This can also be set by the devs to create anti-competition situations. Occasionally a single winner contract could be available that will be in high demand as it will create a monopoly.

#### flat quality curve - everything is useful for one reason or another

Grinding the get the better equipment is common in most games. However what players in this game should strive for is to collect the CORRECT equipment to specialise in a situation. Then the goal becomes collecting the best equipment for each different situation.

Enough combinations of gameplay situation need to exist so that cookie cutter requirements do not become the norm.

#### ease of notifying others what you want

Getting players to do what you want should be easy for the requester to set up and very visible to other players who are looking for something to do. A lot of work must go into getting this right from the start, as it is a fundamental component of the “player creating content” style.

#### price information is not global to encourage exploration

SOLUTION NEEDED - better or worse to have perfect information? perhaps simply better visualisation is all we need to fix global market knowledge?

#### discourage player hoarding - tax on storage space over a certain limit?

storage space costs a fixed amount per space per day, paid weekly. Each week the price moves up or down based on demand. Storage service price min/max and the curve can be modified by the community voting on changes. See below for a more in depth look.

#### visualizations of who is holding goods in a station/service

It is important to see who is holding goods (but not what kind of goods) at any location, so that you can tell who to pester about it. Players can also make available information about the type of goods as well.

#### goods cannot be placed into storage forever, eventually they should be released back into the game world (if a player stops playing)

SOLUTION NEEDED - what happens when a player doesn’t pay his bill? Is the total of his items seized? If it is still protected and can be stored indefinitely without the user paying his fee (but is obviously not available to him) then is that the same as simply deleting the goods?

NPC sales? The items are offered for sale at a fraction of the value plus the fine? Could create interesting dynamic specials from players who don’t pay their bills.

Dealing with waste storage? Automatically contracted to be moved to the refinery?

Creating content for players from players who dont pay their bills (or have quit the game) is a great idea but HOW?

#### Pve content that creates market drive on lower market tiers

Higher up/ harder content that requires more organised groups should not simply provide the same materials at a greater rate. The lower end, easier gameplay should still be required for the whole economy to run smoothly.

What happens is the entire playerbase is doing high end PvE content? They will drive the price down on the items they are creating, as they are not required. Perhaps this could create interesting “waves” in supply and demand, if completing a large PvE raid would result in 3 months of supply of a particular material. Once they price starts to creep up, other players would automatically be incentivized to redo the raid.

#### infrastructure designed for small groups

The requirement for more players to be active in a situation must be arbitraty. Each task needs to be designed with a number of players in mind, and rarely for solo play.

Solo play should be more about “pubs” or public opportunity grouping. If you are alone, you will work other players you do not know, and eventually this might lead to players joining up with each other, or some players being known as trustworthy freelancers.

PvE content thus should be designed for groups of 2-5. To avoid the benefit of “followbots” or multibox clones, the content itself should require enough attention to make multiboxing difficult.

Player groups larger than 5 players should be given multiple tasks that need to be achieved simultaneously. There should be opportunities for large scale tasks at all levels of gameplay. AKA 40 man raids are not something that only the top end do.

### Notes

- players will grind if its in their interest

- travel times to enable value add should work well

- risk should come from NPCs ~~if in a No PvP zone~~

- ~~when in PvP zones, most of the risk should come from other players~~

- promote group play

- players should need to be active in the world to gain wealth

- re-specialization of materials takes real world time (refitting craft for other purposes)

### PvE content for multiple players

content should always be more productive and fun with more players.

Mission content should effect the world, eventually players will offer incentives for mission runners.

Npc Transport contracts should look the same as player ones!

Any player can make a protection contract, asking for others to stay near them and offer payment for kills.

Mission participants need to be interacting, don't support the multi box

Concurrent objective requirements that must be completed at the same time

Objectives: Hold, disrupt, antagonize, harvest,mine, collect, load

Rats spawn at one location and attack another. Second point is where non-combat players need to be.

Only non-combat players can get missions but require other combat players to help them.

Ongoing patrol missions, difficulty fluctuates based on number of accepted players. Bonus points for resource scanning at each waypoint. The more npc,'s killed on patrol, the less NPCs spawn and attack local non-combat players. Local non-coms can incentivise more players going on patrol by donating to a structure.

Linking NPC spawns with mission success. Players who want to destabilize an area might work against mission runners.

NPCs should raid fuel supplies and eventually shut down services. Players should feel like NPCs are the enemy, not farm animals.

Most NPCs should be worth very little to kill, only the occasional special one should have important resources.

"Farming" NPCs instead is accomplished by attacking NPC facilities. Players can raid these locations for the resources, but must bring non-combat craft to carry it. The loading is lengthy, and the goods come randomly. If the attacking team wants a full load of resources of a particular type, they will have to wait a while.

The difficulty of these raids escalates exponentially over time. Eventually the players must leave the area.

Attacking also aggravates local NPC spawns and attacks on non-coms.

Destroying a NPC facility allows players to have new services built.

NPC facilities spawn in clusters but never right next to one another.

The goods gained in this way are needed for manufacturing, but it obviously effects those players who are collecting raw materials.

It also will generate secondary job markets for consumables, patrols, and escorts.

Destroyed NPC bases will be reclaimed if the players do not claim them.

The density of bases could decrease as the terrain generates from the centre out but the speed at which the NPCs escalate could go up. The more players, the further out they could push.

Islands of player facilities could form, surrounded by NPCs. These would just fold back into NPC land if left unattended.

This seems to be leading to an infinite team based PvE sandbox world. Maybe that could work.

Start with one of each service facility (bare minimum) players can develop the rest of the areas.

Perhaps each facility could hold two-three services, but the fuel consumption is quadipled for two services, and times sixteen for three. If it is worth a corporations while, these services will stay powered.

Services so far: sell NPC loot for cash(star port or export centre), mission board, cargo/craft storage, refitting, fuel construction, manufacturing(different kinds), research, recycling, refining, PvP zone flag, control facility(political tower), highway connection (builds player roads between points)

For gameplay reasons these could be limited in placement for quantity. Facilities further out will already be more expensive to fuel because they need fuel from the starting area.

Some components should only come from off planet imports to the starting area.

Static spawns come from small structures. Shoot them to generate spawns, spawns get harder as the structure gets low, structure regens over time (filly once per day). Destroying it makes it take longer to regenerate

### Ideas to make industrial craft interesting to drive

Industrial craft drive automatically by waypoints.

Players build waypoint sets that are saved in a history list and can be saved as bookmarks.

Driving using the same bookmarked path will improve its efficiency over time.

making paths on highways will be more time, heat and fuel efficient.

industrial craft cost wealth per time that they are running, but can run much longer than combat craft.

there is a warmup and cool off time at the end of each path.

the player must commit to a path, and if cancelling, must cool down double as long before moving off again.

Industrial craft can interact with objects farther away than combat craft

for extremely long paths, pauses need to be made to cool off.

Planning paths is a core part of Indy gameplay.

Indy players can plan research, manufacruring and other tasks while in a craft. These plans can be saved and implemented later quickly.

For example, while mining, a player might be configuring a refining plan to have his ore smelted so that when he returns it can be put into action quickly. He might also be organising a protection contract for his trip home.

Collecting static resources should involve coordinating several craft. The base raw materials should be very inefficent to move, so another craft might be nearby to refine/compress the goods.

Collecting and moving items should not be instant, instead the Indy player assigns his minions to fetch the items over time. These can be controlled while driving on a path.

Configuring input and output bins for the Indy cargo will also take some attention. Moving items between internal storages takes time. Having ammunition and coolant available for your escort in output bins.

### Mechanics that could be better than current gen

Buy/Sell orders simplified to “Mark Item stacks in inventory as for sale or wanted to buy”. A price is added. Hover information shows current best price locally, regionally, and hi/lo record. Buttons to quickly increase/lower your price to beat the local best.

Separate areas for each task. One structure with all services is not as interesting as each service having its own structure. Access to services only when in the game world

Player must maintain the land they use, or move to somewhere more populated. Services and structures require constant fuel. This fuel need is in the form of automated buy orders up the a quantity enough to keep the structure running for a set time period. Services tax goes toward making these buy orders. Players can cast votes to modify the prices of services, and the quantitiy of stored material. Player corps can vote on behalf of their players, making these groups stronger politically. Votes are tallied after 48 hours so only players who frequent these areas will end up voting.

Players wanting to reactivate a station/service will need to fill its fueltanks even tho the offered price may be lower than other stations.

Services require more time, players to interact personally in game, and also cost more. It should be realistic that while a process is going, the service runs out of fuel. This means organised groups will be more time/resource efficient and solo players will seek out stations run by well organised players.

Converting items into pure wealth requires moving goods large distances with good escort coordination. Liquid currency inflation is self regulated by the playerbase. Those with a high % of the wealth might seek to halt the flow of materials to these locations.

First tier activities (those that generate resources/wealth from nothing) should attract risk from both PvE and PvP threats. “Mining” should cause npc creatures to attack/aggres the players group. Also, unarmed transport/engineering vehicles driven by players should come under attack when seen by NPCs, unless there are other armed players nearby (in which case there should be a chance they will attack anyway)

Player set missions should be easy to set up. NPC bounty while in squad, pay on arrival/acceptance, contract value min/max should be displayed.

Movement speed based on load of cargo! The difference between combat and engineering craft in terms of speed should be very large. Engineering equipment should also be MUCH more buff, structurally, but military hardware should have higher resistance to damage.

Depots can be deployed by engineering craft that act as temporary storage areas. These are code locked but goods may be flagged as for sale/wanted to buy just like storage in stations.

Storage in fixed locations is limited. The price per unit of space per time goes up the fuller the storage becomes. Players who have junk will get rid of it or sell it when the price becomes too great. Those that are making good money from the stored items will keep them there.

Services have limited numbers of concurrent jobs, but the queue for work can be as long as is needed. Users pay to store items in the service storage as normal (perhaps at a higher rate). “Until complete” jobs can be run, then as long as the user keeps his incoming storage filled the jobs will never expire. The cost pressure from waiting in the queue will go up the longer the queue is as your items must wait longer, and the storage may become fuller with more queue users, forcing people to drop from the queue.

corporations can buy access rights to station services, in which case they can freely modify the values of the station. This process has a minimum bid value. Other corporations are notified of this bid and must exceed the bid by double to instead gain the rights. Rights are for a set period of time (30-60 days?). Excess wealth cannot be taken from the station, however fuel can, so it is possible to take everything when your contract is over. At the end of each period, the next highest bidding corporation takes over control, or you pay the same amount as you did last period to retain the claim.

fees can be set for public users and for corporate members.

being a service owner means your corporation forfeits its right to vote on other public stations

The starting area should not be claimable, instead run by the game devs, or only by public voting.

cargo has many types, to encourage specialization

each craft has a cargo damage tolerance. Taking damage will destroy on board cargo. Transport vehicles have very high damage tolerance on their cargo bays. Military vehicles have limited/no generic storage with low damage tolerance, and high tolerance ammo storage. Hybrid engineering/military craft have a mix but are not better at either role.

craft collecting resources in an area cause all other craft in the area to generate resources slower. EG// Two craft working at the same time will generate 99% of the normal amount each. Each craft also takes up a substantial amount of space, so there is limited concurrent access the best veins/areas. This means if you want the most \$perHour, you need to show up early, get the best spot AND force everyone else to leave when they come to take the second best spot.

Resource collection reaches a peak units per time after being set up for a while. Investment in time means more people know where you area, which means more risk. more risk should mean more cash. Being set up at the right place, for the right time, for the right amount of time should be what you aim for.

No task should be bottable. This means that there should be no task that generates wealth that the player could do with his eyes closed. “Mining” in EVE for example. This prototype could still have tasks that need minimal interaction, but in order to get peak output, a player must be attentive.

One idea would be to have a mining craft set up in an area but the player needs to pinpoint the best spot to actually mine. This point moves over time in different directions. Wealth will still be gained, but the rate will be effected. Also giving players other tasks that they can accomplish while doing this will help (scanning for the next patch for instance).

Setting up for maximum \$ per hour will also means your craft has higher sensor signature, attracting more NPCs to your location.

An exclusion zone, in which you cannot mine, but also others cannot, based on your craft signature/wastage might be good. Players who create these solo behemoths will not be popular with the public players. They would however be good for organised group players who want the most \$ per hour per player not in a military craft.

Perhaps even liquid cash cannot be transferred instantly to anywhere. Perhaps you must leave cash in facilities (banks?) for others to collect. This could create localized cash markets.

~~Corporation credits could be produced and traded as well, but that might be ripe for griefing. Perhaps banks require some collateral of real currency to “mint” corporation credits.~~

Specializing your cargo hold should have large benefits. Knowing what it is you want to be collecting, and forfeiting the opportunity to collect other things should result in you being better at collecting those items. For example a salvager might bring a container for scrap metal and a container for reactor plasma, so he can carry the most of these. Now he leaves behind scrap ammo and electronics. This might create secondary industry where players specialize in collecting the left overs.

### Combat Mechanics

military craft should not be able to carry enough equipment to refit themselves.

destruction of craft should not be as common as withdrawal of forces.

Equipment and craft that take damage can be repaired but it consumes an item in the process. Repairs costs are directly related to the cost of this commodity. Taking big hits also causes a very small amount of permanent damage to equipment meaning it needs to be retired eventually. Craft with lots of perm damage will generate heat faster (see below)

ammunition and repairs are not as simple as just pressing a button and heading out again. These are completed quickly but not instantly. Heavier damage takes exponentially longer to repair. The sooner you withdraw from combat for repairs, the sooner you will be back (travel time not included of course)

destroyed craft retain a portion of their wealth as salvageable components. Another part of their wealth is added to the terrain, that can be collected later.

instead of “docking” players can park in “weapons off” areas. These areas are free of hostile NPCs and players cannot activate their weapon systems. Targets in these ranges are also protected by the station area themselves (the station will fire on aggressors and soak damage dealt to players). Players aggressing others inside the zones will be unable to gain protection for a long period of time.

Combat effectiveness should decrease over time after the craft has started combat. This means that players cannot stay engaged forever, nor can stalemates occur.

The amount of ammunition in weapons should be a real choice. Taking less should give some tangible benefit. Fitting your craft correctly for long/short term engagements should be just as important as fitting correctly for long/short range.

Specialization should be key to success.

Refitting should cost something AND take real world time to complete. Forward planning and having an armory of equipment ready to go should be critical for all activities.

Tactical Raids will be possible since military vehicles are fast enough to get in and out, but engineering and transport craft will not be able to. This will limit supply raids to hybrid craft that cannot carry large amounts for great distances.

Military craft should be expensive to repair per hit point, but not lose as many during combat.

Disabling your weapons will cause your craft to move faster. Re-enabling them takes a period of time in which you are slower than normal. This is so that craft can disengage, so travelling is faster, and so that ambushes are possible.

Information Warfare is greater than Electronic Warfare. IW components allow you to be unseen at range while playing. The are also very situational, being more effective in certain terrain types. Since travelling craft tend to disable their weapons, the element of surprise can be enough for these stealth specialized players to take the advantage.

Your sensor strength determines the longest range in which you can be targetted. Switching to passive sensors will force your opponents to move in closer, but also lower your targetting range. Long range artillery craft will only be able to target larger targets that are also trying to target at longer range creating several combats that are overlayed simultaneously. Long range weaponry will also need to have a minimum range mechanic, however this should be a soft minimum.

Smaller, nimbler craft will be seeking to close the gap and attack long range craft up close where they are less capable.

Craft firing will cause their signature size to get larger, and the sensor strength of other nearby craft to get smaller. Large weapons platforms will have to spread out to be effective.

This will also mean that you can detect craft at long range when they are in combat.

Craft will still be visible at all times, and can be targetted at all times. If you want to launch a missile at the target on the ridge 4kms away that you can’t identify, then you should go ahead. Not being able to tell the difference between NPCs and players could also be interesting.

Information about a craft when you cannot detect/target them will be limited. Visual recognition in important.

Heat is used to limit the time that a craft can operate. It builds up constantly over time and affects the efficiency of craft systems. Coolant tanks can be installed and filled, to extend the lifespan, but these are also consumable (increasing the cost of artificially extending a crafts combat lifetime). The price/availablity of this coolant will modify the player market drie to build heat efficient equipment.

Scanning the terrain to find good harvesting locations should be time consuming unless you are already sure you are in the right area.

Transport and engineering vehicles use a different control system. The player sets waypoints in a point and click fashion. Once the go is give , the craft chargrs up then starts to move. When it reaches its destination it parks which takes time as well. So engineering/transport craft are not good at reacting to situations.

Comabt craft on the other hand are manually controlled. They react immediatly.

Protection contracts are advertised above the player who is offering it and also on a job board in the facilities. Players can offer thier services to the player with the contract. The player looking for protection can also select to automatically accept help. Also if the protectee is an industrial craft, the protectors can see its planned movement.

Searching for an item for sale will show available items on the map and highlight them in the game world. Items can be purchased remotely and are added to the players inventory.

Inventory areas are visualized with boxes filling an area. Information regarding individual items is not available.

Fees for storage are taken automatically. If there is not enough cash available the players goods are locked until the fees are paid. While locked, good suffer fr storage damage.

### Environmental Effects

Different areas of the map should have different effects. Some areas will generate more heat in craft, others will cause them to go slower. There could be many options for this. A dynamic version of this could be represented as weather. Other ideas

- increase cargo volatility (radiation/acid rain)

- decrease vision/radar range

- limit damage to craft so that combat becomes about ammunition storage/quantity

### Landscapes and Level Design

The important things are:

- enough areas to generate localized markets

- scalable to more/less players

- travel times matter

Epic infinite terrain might be cool for an upwards scaling mechanic, but it is important to keep a solid player density AND create mechanics to support that.

Terrain might go on forever, but perhaps there are very few “good spots”. This coupled with the limited runtime of craft, and limited ammo storage, means there is a soft limit to the distance you can travel without risk. New installations would not be available to players, however longer journeys could be supplemented with engineering/transport/support craft.

The starting area, and surrounding play area, should be hand crafted to generate the best play experience for an optimal number of players. The area closest to the “spawn” should be especially well designed for a small number of players.

As the player-base shrinks, the remaining players will be encouraged to stay near the same facility.

If the centre most facility goes offline, then the players must log in from there. So in the end, players should be congregating around the centre point.

The further from facilities that a resource patch/NPC area is, the better its yield should be. It should also be more pinpoint. So the stronger the yield, the more concentrated the area. Areas near the facilities should be more diffuse but low yield. There should be a decent exclusion zone around the facilities that lowers the yield.

The yield amount of areas should fluctuate over time. These could be procedural and on a cycle so that one area is always very rich during the start of a month.

structures that allow players to convert resources into liquid cash (NPC market faucets) should be geographically far away, or limited to a single location per resource that can be converted. An example would be that bounty tags can only be traded for isk in Jita. This creates more opportunities for player involvement and profit.

NPC strength should fluctuate in outlying areas and not be totally linked to yield. This way players can discover quiet safe havens or bustling danger zones. Having players exploring for good patches will mean better yield for less risk.

NPCs should encroach on the player territory. They should not spawn behind your lines. The players who are furthest out should stand to take the most heat. Also this creates opportunities "in the shadow of giants"

NPCs should not spawn right next to players. If you are hunting for them, you need to be moving , not waiting.

Perhaps there are areas where players can go to aggravate the NPC’s causing them to spawn nearby. This should increase the rates of npc attack across the whole play area.
