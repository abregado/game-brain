---
title: "Stardrive-Levels of Abstraction"
source: "Game Stuff/Game Ideas/Stardrive-Levels of Abstraction"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Stardrive]]", "[[RTS Ideas]]"]
concepts: ["Stardrive", "Design: Freighter and Commodity Logistics", "Design: Planet Specials and Rarity", "Design: Procedural Galaxy Generation", "Design: City and Population Simulation"]
words: 771
summary: "Stardrive design note deciding what is abstract vs detailed: commodities, freighters, stars, planets, continents, cities, populations, and 40 planetary special properties across four rarity tiers; plus a galaxy and star generation algorithm and star life-cycle table."
tags: ["area/game-idea", "project/rts-ideas", "project/stardrive", "type/design-doc"]
---

Stardrive Levels of Abstraction

Commodities System should not be abstract. Objects should have weight, size and fragility.

The freighter system should be very abstract but also very complex. Made up of:

Flagfall cost (Frieghter cost)

Maximum shipment size (cargo hold of freighter)

Cost per distance travelled (based on weight)

Maximum distance before stop (range of freighters)

Cost per stop per size(warehousing cost)

Planets and Suns should not be abstract. Information on suns includes:

Type

Phase

Pop# (I, II, or III) a.k.a Metallicy

Color/Spectrum

Temperature

Luminosity

Size

Information on Planets will include:

Orbit

Mass

Diameter

Metallicy

Rotation

Average Heat (Determined by orbit and sun temperature)

Seasonal Change (Determined by Orbit Speed and Rotation)

Each planet will have an atmosphere which will be Abstractly measured:

Atmosphere Rating (1 to 100): Races will have a range in which they can breathe. If not within this range, special tech is needed to live here.

Each planet will have a number of continents:

Biome

Surface Area

Volatility 0-100 (How dangerous this continent is, this can be modified with tech)

Each continent can have multiple cities: Stats for cities are very complex:

Cities have many stats. It is assumed that all cities are self sufficient. Based on current technologies used in the city, the total land area is calculated. This can never be larger than the continent the city is located on. If the continent runs out of land, farming will be reduced and food must be imported (this is abstracted as increase in maintenance costs). Colonies on hostile worlds will not be able to have farms, and thus will have very high maintenance costs.

Populations will live in cities. Each population has stats like:

Birth Rate

Deathrate

Morale

Unrest

Quantity

Type/Race/Species

Unemployment

Biome Types determine the kind of facilities that can be built into a city. Generic facilities like strip mines can be built into any Biome, while others are very selective about where they are built.

Specials: Each planet may have one or more special properties. There are 40 different properties and each one unlocks different technologies. These are divided up into 4 levels of Rarity. Common properties are just that, common. Uncommon properties are half as likely to appear as Common. Rare is half as likely to appear as Uncommon. Ultra-Rare are half as likely as Rare.

Higher technology levels require higher rarity properties to be exploited.

Common (10 Types)

Water

Metals

Radioactives

Macrobiotic Life

Petrochemicals

Non-metallic Gasses

4 More

Uncommon (10 Types)

Complex Life

Heavy Metals

Solid Hydrogen

Metallic Gas

Geothermic Phenomenon

Rare (10 Types)

Sentient Life

Dense Metals

Element 121

Baryonic Particles

Gravitational Phenomenon

Ultra-Rare (10 Types)

Natural Singularity

Super-Dense Metals

Stellar Complex Life

Element 200

Dark Matter

Relativistic Phenomenon

Universe Generation and Exploration

In the beginning, an algorithm should be used to generate the placement of stars in the galaxy. A vast majority of stars generated should be either new stars, or have no planets. Stars closer to the galactic centre should be older (Population I) stars.

Larger stars move through their phases a lot faster.

Create Galaxy

1.  Select total Mass (accuracy)

2.  Select Galaxy Age (accuracy)

3.  Allocate Mass to Rings

    1.  Determine smallest orbit size

    2.  Determine number of rings (random)

4.  Allocate number of Arms (arms based on total Mass)

5.  Allocate Mass to Arms (randomly)

Create Star

1.  Select Ring

2.  Select Arm

3.  Randomly determine distance from centre (orbit)

4.  Determine sun mass (randomly, deduct from total mass)

5.  Determine birth date (randomly)

6.  Calculate orbit speed

7.  Randomly determine distance from arm

8.  Calculate actual position (based on sun age, orbit speed)

Protostar

> Time to form 100million years
>
> Determine Type of PMS (\<2 = Tauri Star, 2-8= Herbig Star \>8 =Instantly Main Sequence)

Pre-main Sequence

1% of total lifetime

Main Sequence

Calculate Time until end of main sequence (t=m^-2.5)

\<0.5 SM = Red Dwarf

0.5-8 SM = AGB Stage

8-70 = Super Giant

AGB Stage

50-70% mass lost

\<0.5 = Red Dwarf

0.5-4 SM = Red Giant

Red Giant

0.5-2.25 SM = Helium Flash causes planetary nebula  White Dwarf

2.25-4 SM = Continues to shed mass

White Dwarf

\>2.25 SM = Type I Supernova (only happens if mass added)

Super Giants

\<1.4 = White Dwarf after Type II Supernova

\<12 SM = small chance for White Dwarf after Type II Supernova

\<20 SM = All go supernova (Type II)  Neutron Star

\>20 SM = Supernova (type II)  Black Hole

\>50 SM = Black Hole w/ SN

> Determine Phase (based on age, size)
>
> If dead, determine outcome

Determine posisiton

Check for star density (based on position)
