---
title: "Extraction Ideas"
source: "Game Stuff/Game Ideas/Extraction Ideas"
modified: 2011-03-09
type: design-doc
area: game-idea
status: "designed"
projects: ["[[EVE-like Player Economy]]", "[[Player Market Hoardmode]]", "[[Living World PvE]]"]
concepts: ["Extraction Game", "Impact System", "Design: Layered Damage Model", "Design: Money Sinks and Faucets", "Player Market Hoardmode", "Living World PvE"]
words: 2307
summary: "Design document for a multiplayer extraction game: explorers find claims, strategy players buy them and hire mercenaries, with an Impact aggro system, money sinks/faucets and layered damage model."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/living-world-pve", "project/player-market-hoardmode", "type/design-doc"]
---

> [*INTERFACE*](#interface)
>
> [*PLAY PROCESS (EXPLORER)*](#play-process-explorer)
>
> [*IMPACT*](#impact)
>
> [*OTHER IDEAS*](#other-ideas)
>
> [*WHEN SHIT HITS THE FAN*](#when-shit-hits-the-fan)
>
> [*MONEY SINKS*](#money-sinks)
>
> [*MONEY FAUCETS*](#money-faucets)
>
> [*DAMAGE MODEL*](#damage-model)

# **INTERFACE**

Players can wander around the main settlement in avatar form to chat and organise extractions. They can also stay in “Lobby Mode” and wait for extractions to begin.

Lobby mode is just like a multiplayer game browser. Instead of just a list of games available there are a number of tabs. Explorers who have found good claims list their claims in a tab. Here Strategy players can review and purchase claims to begin an extraction. Extractions that havent yet begun are listed in the “Pre-planning tab”. The strategy player sets up which equipment he will take to the extraction, and how much space he wants to dedicate to mercenary groups to come with. A budget sheet is shown here for shipping, fuel, weight and the cost of renting the aircraft to move all the equipment out to the site. Mercenaries can get shipped to the location at the Strategy players cost during this phase.

The last tab is for Extractions in progress. During extraction the strategy player can open up more positions/contracts to be filled. Mercenaries can pay to be flown to extractions and begin fighting. They can also review contracts, payments and how the extraction is going. Most players will use this tab.

# **PLAY PROCESS (EXPLORER)**

Solo content is a must as at the start there will not be very many people online at any one time. The initial players will spend their time getting acquainted with the game world, the weapons, damage system and how to stay alive outside the spaceport.

The option to explore the entire game world will be available. obviously there will be limited content at release/beta so systems must be in place to keep the player from venturing too far from the starting area. These will include some of the earliest large enemies. There will not be weapons available to kill these enemies and such will create a “ceiling” in the available gameplay for the time being. Even so the actual explorable area should be quite large at release.

As players explore the planet, they can detect basic areas of high value resources. Once they have ventured out to these areas, a simple system of prospecting should take place. The prospecting system should involve some player skill, and over investing in one area should be penalised. Once a decent amount of resources have been prospected, a player or group of players can lay a claim marker down and sell the area to be exploited by industrial players. Explorers can set the fixed price of a claim, the share of extracted material they want, sell the claim by auction, write a description of the surrounding area (including tactical/strategic assests), or mark the claim for use by their own group of industrial players.

When an explorer group requests a pickup, they must defend the LZ for a short time while the pickup flys in and lands. The time until pickup is based on the distance from the spaceport, and the speed of the craft they require. The speed of craft and landing time is based on the size of the craft (more explorers require a larger craft)

explorers can also bring back samples of plantlife and creatures they have captured for study (research). These are often very heavy and require much larger craft, making pickups quite dangerous. The explorers must also load the cargo onto the craft making the whole ordeal take longer. Mercenaries may also be hired to fly in and be deployed to help defend the LZ while cargo is loaded and unloaded.

Most solo play involves controlling explorers and mercenaries. However industrial players can also complete some early challenges without assistance. The area immediatly surrounding the spaceport can be exploited by industrial players without mercenary assistance but the profits are very very low. My simply purchasing a nearby claim and offering a decent price to mercenaries, industrialists should be able to extract much more than by completing solo extractions. These solo extractions should use all the same rules as multiplayer extractions so that new industrialists can learn how to play safely.

# **IMPACT**

IMPACT is the measurement of how strongly the environment reacts to the players actions. There are a few different types of impact:

Initial Impact is how much Impact is generated when the object enters the area. Moving objects such as skimmers, aircraft or vehicles only add this number to the area while they are inside the extraction area.

Ongoing Impact is how much the local Total Impact the object adds over time. This impact effect stays even after the object leaves the area.

Sudden Impact is an amount that is added to the local impact AFTER an effect has taken place. Many structures and weapons deliver local impact in bursts (for example exploding a mining explosive) but do not generate impact over time or when they are placed.

Depth is a modifier to Impact ratings based on how deep into the environment the players are. During the early release this would be higher the farther the player ventures from the spaceport.

Threshold is a modifier to each Impact based on the largest Impact source at the time. The impact ratings of players walking around should eventually not add to Total Impact if there is a 1000 tonne digging machine churning up the neighbourhood!

Every player has an Initial Impact based on his equipment. Heavily armored mercenaries have a much higher initial impact than a lightly equipped explorer. Ongoing impact is generally from passive effects and communications devices. For explorers, prospecting scans have a low Sudden Impact when used, and then a very slow Ongoing Impact for some time afterwards. Setting fire to anything, digging, mining and terraforming all have high Ongoing Impacts while explosions, combat effects, lasers and heavy packages being deployed have high Sudden Impacts.

Everything the players do in the game world should generate Impact. As this rating gets higher and higher, the game world will respond and attempt to remove Impact generation sources. One might liken Impact to “agro” or “threat” in some MMO games.

Explorers should be attempting to keep their Impact very very low so as to increase the time they can spend searching for claims. If they wish to continue exploring after surveying an area or calling in transport for a specimen, they will have to find ways to reduce their Impact back to respectable levels. Not doing so will cause them to face enemies they are unequipped for.

Mercenary groups will benefit from managing their Impact. Sharing impact among members, only using the minimum force necessary and generally not causing too much fuss for the industrial player will all go a long way to advertising their skill. A group of new players all trying their hardest to kill every enemy that shows up will only cause them to get into more severe trouble sooner, also costing the industrialist player more money to call in more mercenaries, which in turn generates more Impact! This spiral can be managed by co-ordinated player groups with lower ongoiong impact, creating more potential income for everyone at the extraction site!!!

# **TECHNOLOGY**

Since a Lobby system will be used, extractions could theoretically be located on different servers. This may or may not cause problems with latency due to localization of players. Perhaps long extractions can be periodically moved to a server closer to the location of the current players.

Most the weapons used in the game will be advanced ballistic weapons, and railguns. Most of these will use the hitscan technique for calculating if they can hit. The instantaneous effects should reduce the requirements for the server to predict movement of fast opjects.

Mortars, Launchers and Lasers will require more complex prediction algorithims and such will most likely be added later.

Placed explosives and effects can be added early as they do not rely on predictive systems.

If a majority of weapons utilize hitscan techniques, the extra computational power can be used on a more complex hit location system (See Damage Model).

A series of dedicated servers will most likely be required to minimize cheating. Early builds will most likely allow Client-Client interactions so as to minimize infrastructure requirements for testing. Once a persisting economy is introduced the servers will have to be secured.

All economy transactions and persistent player information will be housed on a central server. Purchases and character modification will be completed outside of core gameplay so as to encourage players to prepare beforehand. Once in an extraction, the market and character options will be unavailable.

# **MELEE COMBAT**

Melee combat may have its own system developed seeing players become “locked-in” to HTH. This would play out like a simple fighting game using skills and combos the players add to their characters. Quick time events may also come into play. This would be to demonstrate the close range mayhem of fighting wild creatures. Using smaller ranged weapons (pistols, built in weapons, shotguns) may be allowed as finishing moves (with the player returning to ranged combat with the used weapon at the ready).

# **OTHER IDEAS**

The “strategy” player must decide to ship in Ammo and Weapons for the defenders or let them do it themselves. Alternativly, the strategy player could construct local structures that provide ammunition/supplies over time. These would be quite expensive making them only efficient if used for the long term.

As the extraction continues, the strategy player can order in/build new structures increasing his investment in this extraction. As the investment increases, so does his need to keep mercenaries in the area. It becomes in his best interest to pay more than other strategy players.

Also, as more extractions are set up, the price for mercenaries will also go up. The less strategy players their are, the better it is to start up an extraction as they can pay the mercenaries less. If all the strategy players log off, most likely one of the mercenary groups will start an extraction as they can make must more money from this than from fighting for someone else.

# **WHEN SHIT HITS THE FAN**

Once Impact gets too high in an area, or the returns from extraction no longer make it worth staying, the industrial player can call in dropships to begin collecting equipment from the extraction site. This will bump up Impact while things are loaded, and once something leaves an area the Impact will drop. Mercenaries will still be required to defend the area while equipment is shipped out, so Industry players will continue their contracts until equipment is shipped out.

Once all players have left the area, the site is considered abandoned. Often some equipment will get left behind becasue the risk of losing a dropship is greater than the value of the equipment. When this happens, the area becomes available for re-claimation. Mercenaries can drop in and load left over damaged equipment into their dropship while fighting off enemies. If they fill their dropship, then they can send it home and continue to defend the area until it returns for another load, or to collect them. Remember that the initial impact rating will still be very high due to all the old equipment lying around.

# **MONEY SINKS**

A number of money sinks would be in the game to keep inflation down:

per time unit for Bunks/Food/Ect for their characters

per square meter of storage space (small locker for free in Bunk).

for medical treatment between engagements(see damage model)

for repairs to equipment (or time out of combat to repair it yourself)

for ammunition and equipment charge

for fuel to run vehicles and structures

rental for equipment, vehicles and structures you own

purchase of non-player built equipment

# **MONEY FAUCETS**

The faucets for wealth in the economy include:

Raw materials from extraction

collected explorer Specimens and rare artifact finds

# **DAMAGE MODEL**

It would be fantastic to follow a different vein for damage than regular FPS/RTS. Most games simply have Damage Reduction and Hit Points. When hit points reach zero, the target dies. This only really creates four unique groups of enemies (High DR/High Health, Low DR/Low Health, High DR/Low Health and Low DR/High Health).

It would be much nicer to have more options to create truly unique creatures and enemies. Perhaps “layered” hitpoints so that players must apply different weapon types in the correct order for maximum efficiency. Different Resistances and Recovery Rates would also be good. One shotting creatures should almost never occur, instead requiring several players to coordinate a quick string of attacks to quickly dispatch single enemies.

Multiple states for each enemy could also work. Different damage works better when different parts of the enemy are exposed. Weapons used against wings should penetrate, doing very little actual damage but causing the creature to fall. Certain body locations should have little effect when hit. Pain should effect creature behavior (Flee or frenzy). Death effects should be different based on why the creature died. Simply bleeding out should be a slow death, while shooting a creature in a vital place might make it leak acid, guts or worse! Eyesight, Hearing and Smell should all be available to be affected.

Selecting the wrong method to dispatch an enemy should give some penalty. Perhaps a creature increases Impact when it is bleeding, or another might explode when too much overkill damage is applied. Taking too long to kill an enemy might cause it to hide and heal, or to bring more friends. More targets means more gunfire, and more gunfire is higher Impact.

Visual and Audio ques should be used to tell the player when a creature is in a particular state.
