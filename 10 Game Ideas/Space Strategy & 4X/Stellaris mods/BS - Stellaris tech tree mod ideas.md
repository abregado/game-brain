---
title: "BS - Stellaris tech tree mod ideas"
source: "Game Stuff/Game Ideas/BS - Stellaris tech tree mod ideas"
modified: 2022-02-24
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Stellaris mods]]"]
concepts: ["Stellaris mods", "Design: Tech Trees"]
words: 748
summary: "Six alternative methods for reworking the Stellaris tech tree so empires differentiate by tech choice (closing doors, gateway tiers, rare techs, tech cloud, poker machine reroll)."
tags: ["area/game-idea", "project/stellaris-mods", "type/design-doc"]
---

**New Tech tree**

**Goal:** By the end game, each empire should be more differentiated by its tech choices. Currently every empire will get every main tech, it is only a matter of when.

**Method 1:** Use a Closing doors approach on the tech tree, so that each empire only ends up with half of the non-repeatable techs. Pair each “required technology” with one of the non-required ones. If one shows up, the other is 100% likely to show up as well. If you have one of those researched, then the other will never appear again in your deck.

Military ship techs would still be gainable via battle debris, unless Enigmatic Engineering is taken. Passive techs would gain the Enigmatic tag which means they cannot be traded by Research agreements.

Examples:

- Blue Lasers (+30% dps) or Administrative AI (+5% research speed).

- Hydroponics Farming (space farms) or Eco Simulation (+20% food from farmers)

- Ceramo-Metal Materials (armor tech) or Supersolid Materials (+20% engineer tech from jobs)

Side effects:

- Research agreements give bonuses for following along the same path as your agreement partner

- Late game Scissor/Paper/Rock effects of weapons is more pronounced since each empire will not have taken all the weapon types

- Special weapons from anomalies, events or special projects are more valuable since they let you take the passive bonus instead of a weapon/armor tech.

- Tech rushing leaves you more open to enemy ship specialisation since you will not get new military tech if you always take the passive bonuses.

- Base Tech alternatives need to be increased.

- UI isn’t designed to handle this, so more info will have to be shown in tooltips.

- This is the most work of all the mod concepts.

**Method 2:** Use a Gateway approach to tiering. All techs of a given school (Physics, Society, Engineering) of a given tier are locked behind one Gateway technology. Once that gateway technology is researched, all techs in the tier behind it will no longer appear in your deck. When the Gateway tech appears you can ignore it and continue researching techs in that tier until you have them all. Tech rushing means you are leaving techs behind. Other forms of prerequisite are removed from techs (so you have get the tier 3 version of a tier 1 tech you didn't pick).

Side effects:

- Tech rushers have a new choice, deep or broad.

- Low tech military empires can focus on military only techs and move on to the next tier faster.

- Might not solve the goal, instead just introduce a “new best, only way to play”

- Makes research pacts pointless with empires who are in a different tech tier to you, since their techs will not appear.

**Method 3:** More rare techs, less prerequisites approach. Techs which define an empire (weapons, defenses, ship sizes, optional buildings, robots, terraforming, genetics) become rare techs and drop their prerequisites. Empires simply will not see all of them during a game, and need to decide when they see them if they want to integrate them into the playthrough.

Side effects:

- You can’t plan your playthrough strategy from the start.

- Research federations become mega strong (you can trade rares easier)

- Tech Ascendancy perk becomes mega strong (more rares)

**Method 4:** Tech cloud approach. Remove all prereqs from all techs. Modify weights so that they are the same at base. Modify weights only based on empire ethics.

Side effects:

- Way more random

- Ethics matter more

- Research agreements with empires of different ethics matter more.

**Method 5:** Tech cloud approach 2. Remove all prereqs from all techs. Modify weights so that each successive tier has 3x weight than the previous one.

Side effects:

- By the end game, there will be techs you never saw.

- Random but with more consequence (not good)

- Research agreements are only good with empires at the same tier as you

**Method 6:** Poker machine approach. Remove all techs which increase research speed. Add an extra research penalty to every technology. Add a cheap repeatable technology that gives nothing (and no penalty) called Reroll. Reroll tech has infinite weight so it always shows up. Players will want as few technologies as possible. Tech rushers will just get more rolls.

Side effects:

- Chance to never get the tech you want

- AI probably isn’t going to handle this very well.

- Several hardcoded systems are broken by, or break this.
