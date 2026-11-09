---
title: "Concept Notes - 1d Populous"
source: "Game Stuff/Game Ideas/Concept Notes - 1d Populous"
modified: 2019-09-25
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[City & Colony Builders]]", "[[Game Jams]]"]
concepts: ["Populous-like God Game", "Design: Adjacency Bonus Economy", "Game Jam Timing"]
words: 1028
summary: "Dev notes for a Populous-like god game on a spherical heightmap planet: spells, water level, villagers, city/farm adjacency resource ideas, influence, combat and proto 1 loop; ticked-off todo items."
tags: ["area/game-idea", "project/city-colony-builders", "project/game-jams", "type/design-doc"]
---

Bens List of More stuff to do next

- passive/aggressive mode - q/w to toggle

- ~~spell selection using keys - number keys to select spells~~

  - ~~terraforming~~

  - ~~destroy city~~

- ~~camera zoom and centering on the edge of the planet~~

- ~~increase to the overall size of planet~~

- ~~large increase to the number of segments in a planet~~

- sprite graphics for

  - walkers

  - farms

  - cities

German Time start 7am Friday

Aussie Time start 5pm Friday

world as sphere in the centre

terrain can be adjusted up and down

planets stored as a series of heights. no need to record the points position/angle coordinate as it can be calculated based on the planets radius and total number of points

planets have a water level, which can be increased/decreased with spells

villagers that want to move over water build boats next to the water, which takes time

water level rising as time limit

resourcing - mana cap/regen rates

Spells from orginal populous

raise/lower

flattern

volcano

swamp

flood

armageddon

Lighting

fire

meteor

champion thingo

Mechanical elements

- Terrain system

- unit system

- resource system

- goal

- 

units only have 1 coordinate point

units change to boats when they hit water

**The Easy resource way**

one structure per position

render adjacent structures as a single one

each one produces a point of resource per “economy tick”

efficiency from bigger structures could be simply one extra resource per tile, per adjacent or if adjacent.

*Example 1: three structures in a row generate 3 resources, plus all structures are adjacent to another so they generate 3 extra (one each), this only penalizes single structures on their own, so buildings of 2 are the best.*

*Example 2: three structures in a row generate 3 resources. then each end one is adjacent to 1 other structure so they generate an extra 1 each. the middle structure is adjacent to 2 structures so generates an extra 2. This makes larger structures always better and encourages making your cities as large as possible*

structures can only be built on flat land

flat land is flagged so if both its adjacent land areas are the same height, this can be recalculated on height change and water level change

units(villagers) automatically expand into flat land. Rate?

farms and pop new villagers at a fixed rate

cities pop villagers at a variable rate based on their population

on passive your new villagers join cities

if full, a city poping a new villager will add it to its “development level”. this improves the cities defenses and other stuff (influence maybe)

if on go forth, new villagers will always pop out to expand your borders

**Slightly more complex resource ideas**

two types of structure: towns and farms

towns generate mana

farms allow towns to grow larger

this system would be mainly to stop your territory ending up with one huge city.

farms and cities expand in the same way: villagers build on flat land

cities expand and consume adjacent farms

cities only expand if there is more adjacent farmland than the size of the city

cities do not join together, leaving one space of farm between them

*Example: City size 3 has farm size 3 next to it. Farm grows to 4, city consumes a farm tile. City is now 4 and farm is 3 again. Farm must grow 2 more tiles before the city will grow again.*

will cities starve if the farms are destroyed?

perhaps farms can be built on sloping terrain. this gives you some protection from enemy gods putting mountains in the centre of your towns.

Temples: represent the adjacency bonus with temples in a city. They are just a graphical representation.

towns get “fortified” when they stop growing. Buildings become stone then fancy and it gives a defensive bonus or influence bonus.

for each 10 worth of adjacency bonus the city gets a slot. These contain Temples, Barracks, Walls, ect. Choosable by the player.

Selectable global setting: Stay in house, go forth, aggressive.

On passive, your workers will stay inside your borders

on aggressive, your workers will move out to find new flat land

**Influence Ideas**

influence extends from buildings only. Defensive advantage

influence drops off over distance

influence..

to begin with you can just cast everywhere

**Combat Ideas**

Give a combat disadvantage to villagers/warriors that are travelling by sea. This should encourage players to keep an ocean between them and the enemy (when on the defensive).

combat needs to go long enough that the player can react

the player needs something to react with: spells, buffs, direct action

even if this is simple like clicking on a fight gives you an advantage (god watching over your troops)

how do you get your villagers to attack the enemy? Totem/rally point style? They do it themselves automatically?

dudes run away when low on health?

A Knight spell to convert a villager into a leader who collects a few other villagers and moves to defend or attack

~~on passive, knights will look for targets inside your borders, but never leave your borders~~

on always ~~aggressive~~, knights will leave your lands based on their direction from the holy city

some of the people popped will be military dudes who will defend your lands on both modes

knights will collect military people to help them attack enemy lands

knights have a maximum number of dudes they can rally

**Goals/Gameplay start end**

Armageddon spell is expensive, but ends the game at the point it is called

**Stuff that def go in**

Armegeddon

Knight spell

land mod

UI

buttons for

spells

aggression level (passive/aggressive)

displays for

mana

population total

population ratio

city hover info

population

farm/city plots

city slots

shown above cities

1-3 per city

influence overlay

shows strength of influence: yours and opponents

mouse cursor

spell cost

selected spell

das ist ein tlie

Proto1

\*Horizontal plane of tile heights

\*Can adjust height

+People walk around, build cities, farms

+Reproduce people

+city creation logic

+detection of flat land for workers

Loop

Render

re-render workers and units (land and cities only render on update)

Update

Mana

Pop growth

City upgrades

Fight

Move

Collect input

Enact spells

-
