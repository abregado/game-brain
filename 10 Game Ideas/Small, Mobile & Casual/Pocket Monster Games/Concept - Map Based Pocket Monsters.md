---
title: "Concept - Map Based Pocket Monsters"
source: "Game Stuff/Game Ideas/Concept - Map Based Pocket Monsters"
modified: 2017-04-25
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Pocket Monster Games]]"]
concepts: ["Pocket Monster game", "Design: Shareable Seeded Encounters"]
words: 959
summary: "Design for a simplified Pokemon-like collector game with map routes, minigames at encounters, catch screen, seeded shared encounters, art asset list and monetisation options."
tags: ["area/game-idea", "project/pocket-monster-games", "type/design-doc"]
---

**Aims:**

- To create a gameplay experience targetted at the Pokemon collector player type by removing elements that are less interesting to theseplayer types and making it easier to follow this playstyle.

- Reduce overall complexity a lot to create a game with far less footprint.

- To make the game mechanics scalable

Components/Playstates

- **Map Screen:** This shows all of the cities on the map, and displays the routes leading away from the current city.

- **Routes:** As the player scrolls through the routes, they are shown which pokemon are available on each route (never encountered pokemon are shown as “?”, seen but not caught are shown as grayed out portraits. Certain routes are only available if the player has acquired special equipment. Some routes are only single direction. There are about 4 routes between each town.

- **Pokemon Portrait:** This is a single image page which shows creatures as they become caught. The player can click on any pokemon to learn more information and see their portrait image. This page serves as a progress meter and library of collected information. This takes the place of the Pokedex.

- **Route Progress Screen:** One a route is selected, the player is shown this screen. It displays how many encounters are left in on the route and what the previous encounters were. When an encounter begins, the player is taken to the Minigame screen.

- **Minigame Screen:** These games are played at the start of an encounter. The player can cancel the minigame at any time to skip the encounter. If the minigame is completed then the player is taken to the catch screen. As the minigame is worked on, it should become obvious to the player if this is a pokemon they have encountered before (via graphical and audio queues). Some encountered also give catch items. Cancelling a Minigame means no chance to catch the monster, but still gives items from the encounter.

- **Catch Screen:** Here the player has a number of options to catch the viewed creature. Candy will decrease the change of the creature running away, rocks make the creature more likely run away but make the catch chance higher. Then there are the Catch items, each has a different formula and therefore a different % catch rate against different pokemon in different situations. These rates are shown to the player before they are given. After each move there is a chance that the monster will run away.

- **Scoreboard Screen.** When you collect all the monsters then the number of moves you took is uploaded to a scoreboard. Here you can see how many people are above and below you.

Initial Art Content:

- 3 Towns

- 12 routes, 4 routes between each town

  - One single direction, freely travelled road

  - One of each direction road that requires the first Travel Item unlock

  - One single direction road that requires the second Travel Item unlock

- 2 Travel Items

  - One gained after visiting all three towns

  - One gained after visiting all 6 of the Routes that require the First item

- 24 Monsters

  - 6 that are common to each area between towns. So 2 common between Town 1 and 2, 2 common between Town 2 and 3 and 2 common between Town 3 and 1.

  - 6 that are common between a pair of routes which are between the same town. So 1 which is common between Routes 1-2, 1 common between Routes 3-4, ect

  - 12 that are only available on a single route. Each route has a single unique Monster.

- Images

  - 24 Monster Portraits: Small and circular with unique shilouette and coloration

    - 1 additonal per monster greyed out (seen but not caught)

    - 1 Unknown Monster icon with “?”

  - 24 Monster Action Images for Catch Screen

    - 4-9 frames of animation could be nice here.

  - 1 large Image which a landscape, the image of the player (need Male, Female and Neutal characters) that contains all 24 monsters at the correct scale.

  - 3 Chracter Chibiis for Route Selection and Map

  - 3 Town Images for Map

  - 2 Symbols for Travel Items

  - 6 Various Catch Items

    - Item Selection icon

    - Item Pickup image

  - 3 Icons for Catch Screen

    - Feed, Throw Rock, Flee

  - Map Icons

    - Unknown Encounter

    - Completed Successful Encounter

    - Completed Unsuccessful Encounter

    - Monster Caught

    - Item Found

  - Map Background

  - Enough Parts to display 12 routes

    - Collected as a simple tileset

    - 2 Blocker tiles for the Travel items

  - Menu Art

  - Scoreboard Screen Art

  - Company Splash Screen

  - Game Splash Screen

  - Minigame Art (3 sets)

    - Tiles which can be colored

    - One tile per monster

    - One tile per item

  - One Minigame Cancel Button

  - Success and Failure Banner

**Monetization Options**

- Purchase extra catch Items for microtransactions

- Banner Ads

- Full page ads between

**Interesting Psuedo-Random stuff**

- Make the randomseed change based on day, and based on how many moves you made along each route. This means that if two people go to the same route on a given day, the same encounters will take place. If a single route is traversed more than once, then add one to the seed so that consecutive trips will also yield the same thing. This makes the game very shareable. Couple this with a Tweet or FB Share button.

**Other gameplay ideas**

- Every encounter gets you money which you can use in each city to trade for Catch Items. Each City has 2 types of Catch item, the common type and a unique type. The other 2 types of catch item are found only in Encounters.
