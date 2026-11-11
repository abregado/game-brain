---
title: "BS - 4x Economy"
source: "Game Stuff/Game Ideas/BS - 4x Economy"
modified: 2024-03-26
type: design-doc
area: game-idea
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]", "[[Stellaris mods]]"]
concepts: ["4X Utilisation Economy", "4X Slider Economy", "4X Control Only Map Space", "FourEcks / 4X Space Empire", "Design: Economies", "Stellaris mods"]
words: 1792
summary: "Design for a generic 4X economy built on resource potential, a Utilisation resource, population-driven Commerce conversion, production-target sliders, claim/hold/abandon per system, a resource list, and a map-control-only variant with stability and strategic systems."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "project/stellaris-mods", "type/design-doc"]
---

Aim. An economy that is :

- Only updates when it is changed

- easy to interact with

- Controls scale with large and small empires

- Gives feedback in a centralised place

- Takes time to change

- When optimised, is slower to change

- Can handle as many different resource types as the content designer wants.

- Should be agnostic of the other systems in the game. It is a “numbers going up” generator.

**Generating resources**

Typical Starsystems dotted about

Objects in those systems have “resource potential” values that are tied to technologies and each level has a cost. For example an asteroid belt might have:

- +1 , “outrigger-mining-companies”, 10 minerals

- +1 , “plasma-drive”, 2 plasma crystals

- +2 , “teleporters”, 1 strange matter

As those technologies are researched, more “resource potential” is available.

One resource is used to “utilise” resource potential. The cost of utilising a potential resource is dependent on the technology (shown above. The Utilisation resource must be spent in the same quantity and then the resource potential is turned into actual production. In the example above, accessing a +1 from outrigger-mining-companies in the asteroid belt will cost 10 minerals and 10 utilisation.

The Utility component of the costs are modified by distance from a colony world, and distance from a trade lane. Trade lanes run between planets which are of the home or allied empire.

**The civilian economy**

Colonies hold population. Population works similarly to resources. A planet will have a potential population resource amount. These cost utilisation and another “food” resource to fill, and also have a maximum spend per tick, which means they take much longer to fill. Population has an upkeep of 1 “food” resource (different for each empire) so growth is only limited by your “food” production.

Population is used to manipulate your base resource income into the income you want to have. For each population on a planet, a potential resource called Commerce is created. Commerce works differently from other potential resources as it can be filled with anything, but also consumes an already utilised resource.

Resources from Commerce are added on top of utilised “raw” resources, so you cannot convert resources back and forth to make an infinite windfall.

The options for what can be changed into what are based on technologies. These technologies start off returning less than 1:1, but can go up to higher than 1:1. Some resources are harder to make or rarer to find. Technology can also increase the “conversion density/catalyst effectiveness”, the total converted per point of Commerce.

**Resource storage**

There are resource storage limits for each resource. Expanding these simply costs that resource and Utilisation. Excess resources generated over the cap are converted to one of the non-potential resources at a very bad exchange. **Probably have excess resources converted to Utilisation at a very low exchange. Have Resource storage cost only Utilisation, but have this use the lowest priority.**

20.03.24. Unspent resources accumulate in a pool which creates a resource expenditure. Keep your storage pools at zero to maximise income. Perhaps it is easier to just cap resources and put that burden on the player?

Wait. Perhaps it is better if there are no resource storages. Everything is income like in ZeroK. Unspent resources are simply wasted. Income can be used to refill income buckets like fleets or planets, but once full, the excess is lost.

**Production targets**

The whole economy is managed from the same place. The player only sets their desired production per tick for each resource. If a desired production is lower than the raw production, then the excess is available to be converted using Commerce.

Utilisation of Commerce and potential raw resources is automated. The player does not need to individually choose which raw resources are utilised next, or how each potential commerce is used. As the player changes their production targets, Commerce is swapped to create the desired economy, and raw potential resources are tapped.

Unused Commerce is more expensive/slower than Unused potential raw resources. Raw resources are generally cheaper/faster than swapping a Commerce utilisation to a different one. **Probably means that Commerce utilisation needs a “deconstruction cost”**

Resources can also be given a priority, which indicates to the automated system which resources should be converted or expanded first (if available). Commerce which is being used to convert to a higher priority resource will not be swapped. **(Perhaps this can just be based on how far under your current limit you set the desired level)**

Since this all costs Utilisation, it takes time to change your economy. Also, as Utilisation is also used to tapping new potential resources, requesting your economy to change will slow expansion of borders.

**Guiding expansion**

As you find new systems, and survey them, there will be some that you do not want to utilise. Each system can have its Desired Utilisation state set to one of three states:

- Claim: Utilise resources here, and if we don’t own the system then take it

- Hold: Don’t Utilise new resources here.

- Abandon: Actively prioritise resources here for de-utilisation, and leave if there are no resources being utilised.

**What do we spend these resources on?**

Winning! Some ideas for stuff to buy:

- Timed bonuses (Timed Edicts from Stellaris)

- Technology

- Piracy (increasing the “distance from colony “based utilisation costs for your neighbours)

- Diplomacy

- Progressing Story content

- Ships and War

- Defense and Peace

- Adding bonuses to Planets (Terraforming, special structures)

- Culture

- Espionage

- Exploration of new systems

**What are the resources?**

Here are some examples for resource content and what they might be used for. The economy mechanic should be agnostic to the other systems in the game.

Energy

The similest resource. Low technology options to convert it into the other basic resources.

Food

Consumed by Population to grow and by existing. Potential Food is generally only found on Planets.

Minerals

Cheap to Utilise Minerals are common in space territories, while plentiful but more expensive Minerals come on planets. Converts to more complex resources cheaper than energy, but does not convert to food, and converts to Energy very poorly.

Military

Converts from Minerals or Energy. Spent to buy ships and starbases and colony ships. Could also be needed for researching or implementing new Military Technologies.

Components

Converts from Minerals or Energy. Spent to build colony ships, stations, planetary upgrades.

Research

Spent to unlock new methods of Utilization and new resources. Also spent in combination with other things to create Survey projects.

Culture

Converted from Energy easily. Used to add global modifiers to everything that is not resource generation (the effectiveness of spent resources). Can also be spent to add raw potential culture, which can be converted further. It’s the snowball that might get uselessly big.

Government

Converted from Energy at a bad exchange. Tiny bit used with each purchase action. The player will want to minimise this as much as possible while not letting it block them. Your capital produces some “raw potential” of this. The storage cap should be quite low.

Utility

Converts from Energy or Minerals at mediocre rate. Converts from raw Government at a much better rate. Capital and each planet produce some raw potential of this. Most empires will want a lot of this while growing, or immediately before/after substantial changes in situation (war).

Logistics

Used as Upkeep or Unit Cap for military fleets and new Colonies. Zero storage, so excess is lost/converted. Potential raw is created from spending on big infrastructure projects. Don’t want it unless you are going to use it.

Commerce

Raw Commerce produced from Population. Zero storage, so excess is lost/converted. A catalyst to allow anything to be converted into anything else.

Espionage

Converted from Government, Logistics, Culture at a good rate or Energy at a poor rate. Can be spent to gain Intel or bonuses against a specific empire cheaper than Clout.

Clout

Generated raw from Capital, and from completing diplomatic projects. Can be stored and spent to gain bonuses with neighbours. Can be used to buy uninhabited systems from neighbours.

**Bloat Scope**

**Intergalactic trade**

Potential Commerce can also be generated via setting up trade pacts with neighbours. Here, instead of having options based on technology, you have options based on your relative empire total production, and distance to one another. If your empire utilises one pairing option, the trading empire also utilised it, but in reverse. The initialising empire pays the cost.

Utilising these Commerce points probably costs a Diplomacy resource, but that is out of scope for this document.

**Different Species**

Each empire has a different resource for their population, and each planet has a different population potential for each type of population.

Each type of population resource has a setting if it can grow

Each type of population has a global modifier of how integrated it is into the empire. This gives a % penalty to its Commerce generation (but not its upkeep).

**Colony specialisations**

Planets could have a Size resource. Utilising a potential raw resource, or a point of Commerce would consume one of the Size resources. The player could decide on a split between how Size is spent. The economy automation system would work around these choices, or the choice could be given back to the automation system.

Depending on the type of game you want to make, it might be better to leave the entire economy to the automation system.

## Control only which space is controlled

The player only captures area on the map.

For each empire, a system has a Stability tracker.

When a empire has ships alone in an enemy system, it flips to their ownership

Stability of all other empires goes down very quickly while owned by someone else

Some systems are marked as strategic

Your empire grows to fill the space you have captured.

It goes outward between strategic systems, and then outward from those.

Systems with more stability are developed first

Systems are only developed when their stability is above a certain threshold.

Strategic systems generate resources for you (The Navy) based on how many developed systems are connected to them.

Strategic systems increase their development level over time, and also when connecting systems are added.

Strategic systems decrease their development level over time when they have not enough connected systems.

The minimum Stability that a system needs to be connected to a Strategic System is based on the Development level of the Strategic System.

Frontier territories that are regularly flipped between empires will never have enough Stability to heavily affect an empire’s economy. Only by holding space for a long time, can you build up your economy.

At a certain level Strategic Systems stop requiring connected systems and instead require connected Strategic Systems.
