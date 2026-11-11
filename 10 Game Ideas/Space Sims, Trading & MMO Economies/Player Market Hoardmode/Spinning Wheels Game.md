---
title: "Spinning Wheels Game"
source: "Game Stuff/Game Ideas/Spinning Wheels Game"
modified: 2015-04-22
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Player Market Hoardmode]]", "[[Playdate & Small Games]]"]
concepts: ["Spinning Wheels Game", "Design: Player Market Economy", "Player Market Hoardmode", "Design: Idle Game Timescales"]
words: 1277
summary: "Design doc for a long-timescale idle multiplayer game where players run hamster wheels to feed generators, balance resource tubes in a sweet spot, build items in The Chamber and trade in a player market."
tags: ["area/game-idea", "project/playdate-small-games", "project/player-market-hoardmode", "type/design-doc"]
---

Aim:

- A game that can be played over the course of a few weeks

- multiplayer interaction through trading

- simple interface, complex decisions

Mechanics:

- balancing production/consumption

- staying in the sweet spot

- slow wind up

Rewards:

- Social status

- high scores (most of each resource produced in the last week)

- epeen

- maintaining the sweet spot

## Gameplay Explainations

### Wheels, Pegs and Hamsters

Each player is presented with a board that has a number of pegs in it. Each peg is connected to the shaft of a generator. The player is given a number of wheels to attach to these shafts/pegs.

The wheels have different sizes, and each one when spun will keep its generator running for a different amount of time, and spin it at a different speed.

The player is also given a number of Hamsters which can be dropped into a wheel to start it running. The wheel will turn and the attached generator will generate resources every time it fully rotates.

After a time the Hamster will become tired and stop running. The player must click the wheel to remove the hamster and give it a short rest.

### Tubes and Generators

Each time a generators wheel goes around once a number of resources are generated and sent into storage tubes. These tubes are shown on the side of the screen. Each tube stores one type of resource. If a Tube is full, then the produced resources are wasted.

Marked on each tube are three guides or arrows. These show how efficiently the resources are being used for construction in The Chamber. The bottom arrow shows at which point the efficiency starts increasing above 70%, the middle arrow shows where the efficiency will be 100% and the top arrow shows when it will be 50%. The “best play” is when the player keeps all of the resources in the tubes as close to the middle marker as possible.

### The Chamber

This is a separate screen, not shown at the same time as the Wheels. When looking at The Chamber the Tubes will also be visible.

So what is it? The Chamber is a factory in which the player feeds resources to construct various things. The player can select a recipe to use in The Chamber, and the required resources per cycle and the number of cycles will be displayed. Each different recipe requires different resources (2-5 of them) supplied at different rates. Each time the Chamber completes a cycle it will consume these resources and advance the stage of construction one step.

The recipe also affects where the three arrows on each Tube are located. Harder recipes will need more resources as well as more precise play.

The player can choose what to construct only when The Chamber is inactive. The is the possibility that a player can have more than one Chamber (bloat feature).

### Recipes and Items

The items that the player produces are used to increase production. They include food for the Hamsters, upgrades for generators, the ability to move wheels, grease to make wheels easier to turn. Most of these should be consumables.

There will also be a number of “maintenance” items which the player must regularly build and which get consumed over normal gameplay. Upgrading the Factory should increase the consumption of these items, as will how close to the “sweet spot” the player runs his Tubes.

### Modifying the Pegboard

Upgrades which simply improve objects should be kept to a minimum. Perhaps there can be a mechanic of upgrading your Hamsters so they are more specialized and also just slightly better over time.

Other items should be consumed to modify the pegboard. Moving generators, replacing wheels, changing sizes of wheels. Tube capacities can be increased, per resource type so that greater excess of resources can be stored (for two part construction), or to access better efficiency on harder recipes (the arrows could be much higher on harder recipes).

### Timescale

This game is designed as a long time frame, zero player game. The simulation runs while the player is not watching, or while the game is closed. Similar to Farmville, Cookie Clicker or other such games. The player only needs to set up some long runs with him Hamsters and then come back later to check on their progress.

Perfect success might require some Hamsters to be set up on long runs, with the player attending every 20 minutes to set up some short runs.

The shortest run could be a few seconds, and by the success of Farmville games, early gameplay should be focused around runs no longer than 10 minutes. Building more advanced items should take up to 48 hours.

### The Multiplayer Element

While this game might play nicely as a single player game, where the players work to maximize their own Chamber, I feel that it would be a waste. As a motivator I think Rolling Highscore tables will have a great effect on the game.

The game should track how many of each item a player produces, and when they are produced. Rolling high scores for max production during set periods (1 day, 3 days, 1 week) will mean players can always compete to make the most efficient “Hammer making Chamber” or other specific item. There would also need to be “Highest of all time” ratings to drive players to continue competing (against themselves).

### Player Market

Another option could be a player market, where players can sell items they have made to buy other items. This means that players could focus their Chamber on making one or two items very well, and import all of the other items they need. As most items are consumable, and each player will consume most of what they produce, the inflation should not be too harsh. Items that players only want one or two of ever will most likely depreciate in value.

The player market would be implemented by flagging each item in a player's inventory as either buy or sell, and by giving a ratio. Then when a player wants to buy something, the market system can take into account what they want to sell and find the best offers. The market needs to be buyer driven, otherwise a currency will be needed (then we need to deal with wealth creep).

If this system was implemented, a per resource storage cap (or a global cap) would need to be added. This will drive the price for items down, and stop players asking for outrageous deals.

Price Rise Drivers: Time to make item, ease of tube balancing, cost of retooling, players wanting to focus on a few items only, access to recipe.

Price Decrease Drivers: Inventory Space limited, items are consumable

Price Dependency Drivers: Cost/Benefit for using consumables

Wealth Faucets: Player time spent, Hamsters spinning wheels

Wealth Sinks: Consumable items, itemless recipes(see below), retooling costs

### Other Benefits for Player Market

The market could drive players through the content organically instead of enforcing progression with mechanics.

As players gain equipment, player skill and access to better recipes/consumables, they will no longer want to waste time and resources retooling to make low grade consumables. If done correctly, high level players may drive the economy. This could be achieved by having very difficult recipes at various times in the progression arc which don’t produce any usable items. These “Useless Items” could be simply used for epeen/cred. These would have to be very complex to produce, require several different stages or have some special mechanic to make them interesting. They could also consume other consumable items to drive the market.
