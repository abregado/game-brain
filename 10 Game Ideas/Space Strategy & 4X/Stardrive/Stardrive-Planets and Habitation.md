---
title: "Stardrive-Planets and Habitation"
source: "Game Stuff/Game Ideas/Stardrive-Planets and Habitation"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Stardrive]]", "[[RTS Ideas]]"]
concepts: ["Stardrive", "Design: City Districts", "Design: Species Habitation", "Design: Planet Specials and Rarity", "Design: Freighter and Commodity Logistics", "Design: Species Decline", "Design: FTL Speed and Galaxy Scale"]
words: 1633
summary: "Stardrive design notes on cities as districts (commerce, industry, mining, agriculture), housing density, planet/species habitation factors, special-resource rarity, game axioms, FTL speed vs galaxy scale and species decline timescale."
tags: ["area/game-idea", "project/rts-ideas", "project/stardrive", "type/design-doc"]
---

Stardrive Levels of Abstraction

## ***Cities***

### **Surface Area**

The aim is to use surface area for a majority of the calculations for cities. Effectively surface area will show how much “space” is available on a planet. It will also help for abstract visualization in the beginning and hopefully later with graphical coding.

### **Cities and Colonies**

Habitations on hostile worlds and others on terrestrial worlds must operate in the same way. Hostile Environment habitats and Domed Colonies will be less efficient, take up more space, have higher maintenance and a whole host of other issues. Terrestrial cities also include vast tracts of land being used for agriculture. The scale and detail of these must both be the same. Players who understand one MUST be able to understand the other just as easily.

### **Districts**

Districts are areas of cities in which citizens perform different jobs. Building a district of a certain size is always cheaper than expanding a current one, however only one of each district can be in a single city.

As technology advances, different versions of each district will become available. Each will have its advantages and disadvantages. When building a new district the player can select how big he would like it and see an estimate of costs, time and maintenance fees. If there is already a district of the required type in the city, the player must expand it or upgrade it, both of which are not as efficient as building it to the correct size at the start.

### **Housing**

As technology increases, the number of people able to be housed in a km^2 will increase. A terrestrial industrial city might contain a small area with skyscrapers or arcology type housing while another more agricultural planet might use sparse single story buildings to distribute the population over a larger area.

### **Commerce**

This district creates internal empire income and distributes Luxury Commodities to the citizens. Higher tech Commerce districts have an income bonus per citizen in the city (later per planetary population, and system population). Commerce also generates a moral bonus based on which commodities are being sold.

### **Industry**

This district produces most items for your empire. The output is measured in “population hours”. Higher density industrial districts will be able to employ more workers but will also create more pollution and effect local biomes much more. Certain amount of the production will be used for planetary means and maintenance, however the “surplus” production will be dedicated to whatever you select for it.

Many factory processes will become available through research and it is these that are selected for your Industry Districts. Multiple processes can be selected and a number of Pophours distributed to each.

### **Mining**

This district focuses on claiming minerals and resources from the planet itself. Mining takes a lot of area but can potentially employ many people. Resources are generated while biomes are slowly destroyed, leaving only the Barren biome behind.

Different types of mining include: Forestry, Surface, Strip, Trawling, Ice, Oil Rigs, Core, Shaft, Ocean floor, Atmospheric, Asteroid, Gas

### **Agriculture**

This district uses the most area of any district. Bonuses are awarded for low density housing and penalties are suffered for high population and heavy industry. Agriculture also has the lowest worker density of all the districts. Thus planets that are dedicated to agriculture tend to have very low output of all other production types.

Different types of agriculture: Crops, Fishing, Animal Husbandry, Hunting, Xeno, Hostile Environment

Each type of agriculture works best in a single biome type.

Commodities System should not be abstract. Objects should have weight, size and fragility.

The freighter system should be very abstract but also very complex. Made up of:

Flagfall cost (Frieghter cost)

Maximum shipment size (cargo hold of freighter)

Cost per distance travelled (based on weight)

Maximum distance before stop (range of freighters)

Cost per stop per size(warehousing cost)

Planets and Suns should not be abstract. Information on suns includes:

Mass

Phase – position in timeline (proto, main sequence, death)

Pop# (I, II, or III) a.k.a Metallicy – generation of star

Color/Spectrum – product of mass

Temperature – product of mass

Luminosity – product of mass

Size – product of mass

Information on Planets will include:

Orbit

Mass

Diameter

Metallicy

Rotation

Average Heat (Determined by orbit and sun temperature)

Seasonal Change (Determined by Orbit Speed and Rotation)

Each planet will have a number of continents, each will have:

Biomes (any number of different ones)

Surface Area

Each continent can have multiple cities: Stats for cities are very complex:

Cities have many stats. It is assumed that all cities are self sufficient. Based on current technologies used in the city, the total land area is calculated. This can never be larger than the continent the city is located on. If the continent runs out of land, farming will be reduced and food must be imported (see freighter costs above). Colonies on hostile worlds will not be able to have farms, and thus will have very high maintenance costs.

Populations will live in cities. Each population has stats like:

Birth Rate

Deathrate

Morale

Unrest

Quantity

Type/Race/Species

Unemployment

Biome Types determine the kind of facilities that can be built into a city. Generic facilities like strip mines can be built into any Biome, while others are very selective about where they are built.

Planetary Factors contributing to Habitation

Mean Surface Temperature (simple range of tolerance)

Physical Volatility (made up of Surface and Atmospheric and Seasonal)

(% of each biome surface area that is habitable)

Atmosphere (type)

Biome Selection (type of biome)

Surface Area (size of each biome)

Gravity (planet mass)

When generating a species, players drag a slider to show the perfect temperature and the range of tolerance to temperatures.

Then, a list of atmospheres are displayed. Each can be changed to: Required, Harmless, Harmful or Toxic.

Oxygen

Nitrogen

Carbon Dioxide

Argon

Ammonia

Methane

Sulphur Dioxide

Fluorine

Chlorine

Hydrogen/Helium

Preferred Biomes are then listed. For each one selected as Productive, another must be selected as Hostile. Any not selected as such are listed as Acceptable.

Resistance is given as a slider. The higher it is, the less effect Volatility has on colonists.

Gravity is a scale of productivity. The farther from optimal the planet is, the less productive the populace is.

Specials: Each planet may have one or more special properties. There are 20 different properties and each one unlocks different technologies. These are divided up into 4 levels of Rarity.

Higher technology levels require higher rarity properties to be exploited.

Common (10 Types) - 1:100 planets have one of these

Uncommon Metals

Radioactives

Macrobiotic Life

Petrochemicals

Non-metallic Gasses

Uncommon (10 Types) - 1:1000 planets have one of these

Heavy Metals

Solid Nitrogen

Metallic Gas

Natural Copolymers

Amorphous Carbon

Rare (10 Types) - 1:10000 planets have one of these

Dense Metals

Element 121

Baryonic Particles

Gravitational Phenomenon

Solid Hydrogen

Ultra-Rare (10 Types) – 1:100000 planets have one of these

Natural Singularity

Element 200

Dark Matter

Relativistic Phenomenon

Helium Superfluid

Axioms of Stardrive

- Stardrive is designed to be a “hard sci-fi” setting. Players will need to make every effort to explain their technology and species.

- Players are rewarded for adding detail and “hardness” to their race.

- The content should be created by the player

- Level of detail should be small enough to provide a high level of micromanagement

- The scope of the game world should not impose restrictions on any player.

- All things can advance constantly and every successive advancement has diminishing returns.

- Life was kick-started at the same moment on all life containing worlds across the universe.

- Space faring cultures only last a very short time in the galactic timeline. Species will start to go into decline within several hundred years of leaving their homeworlds.

The search for Consistency

While a lot of things should be possible in the universe of Stardrive, consistency is essential for a believable world.

A note on distance and speed

FTL travel will be possible. But what will the “fastest” object be. The technology system will allow empires to research constantly in each field. Theoretically FTL drives could reach several hundred times the speed of light. The Ultra-tech list will include stellar teleportation of ships and freight over an increasingly large distance.

So how big will the galaxy have to be to support decent gameplay. The research system implements exponential expense for new technologies, and maintenance costs for technologies that are being utilized. This should keep a majority of empires from gaining this technology except through trade. Since the higher technologies are based on the rarer resources, conflict over controlling these special planets will most likely stall exponential technology gain.

Game turns will be broken into “months”. 10 months will make up a single game year. Early game empires will have FTL speeds of between 1.1c and 3c. Even the closest star to a homeworld will take 10 turns to reach at the start of the game.

The Milkyway galaxy has a density of approximately 1 star for every 0.07 c^2. This means that the number of stars reachable from an empires homeworld is equal to:

Pi \* Speed^2 / 0.07

Once speeds of 25-50

Species will enter “decline” after roughly 200 years (2000 turns). From this point, species will begin to gather a collection of negative attributes, affecting their birth-rate, deathrate, productivity, lifespan, fertility rate, ect. Once this happens the race should be completely unmanageable after 400 years even with the most focused research efforts.

The Scope and Scale of Stardrive

The game itself starts in a single ring of a single arm of a single galaxy. The sheer amount of stars in even this small part of a galaxy should be enough to house 10-20 empires even if they expand greatly.
