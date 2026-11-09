---
title: "Concept-Goblin Pathfinding"
source: "Game Stuff/Game Ideas/Concept-Goblin Pathfinding"
modified: 2013-06-12
type: design-doc
area: design-theory
status: "idea"
projects: ["[[City & Colony Builders]]", "[[Dwarf Fortress mods]]"]
concepts: ["Design: Pathfinding-Driven Settlement AI", "Dwarf Fortress mods"]
words: 558
summary: "Essay on using pathfinding in reverse to simulate how creature groups (goblins) build defenses and adapt, with intelligence and thinking-speed factors."
tags: ["area/design-theory", "project/city-colony-builders", "project/dwarf-fortress-mods", "type/design-doc"]
---

Different uses for path finding AI

Actors in a game world move through it using Path finding AI. In modern games this can be as simple or details based on the complexity of the game world and the variety of the decisions an actor can make.

I would propose instead to use pathfinding in reverse to calculate scenarios and generate environments that are more believable.

Some might say this is simply procedurally generated content, but I believe it could be much more.

A simple Example.

A group of Goblins has made its home in an abandoned cave. They set up their small camp in the driest place they can find that is furthest from the entrance and closest to the water supply. Some other creatures from deeper in the caves feed on the newcomers. The Goblins pathfinding extends from its camp to its closest water source and to a nearby farm that is located outside the cave.

After being attacked for a while, the Goblins decide to construct some defences…

Since the point at which the goblin AI overlaps with the enemy AI is known, the Goblins construct a wall (shown by the black box). The attacks near the water cease, but soon begin again nearer to the camp. Now that the Goblins are closer to their camp they can defend easier and a flag tells them that they have been successful in bettering their surrounds. However raids to the farm are still encountering attackers at the point indicated. More constructions are started.

This time the result is worse than expected. The defence point is not moved and Is still jeopardizing the water supply. The goblins instead build an obstruction (or change their path) to the water…

Now the way is clear. The path that the enemy takes is completely separate to the goblin waterboys. Now the Goblins can work on building traps along the enemys warpath and eventually when the attacks become weaker, push the creatures back to the entrance.

Of course looking at this diagram shos that the attackers can still make headway if they were to change their pathfinding. After enough losses they would seek alternative routes, and the goblins would counter those as well. Again, when the heroes show up to investigate the goblin raids on the farms, the goblins may not be so well prepared.

Relative Creature Intelligence

Creatures of greater intelligence can be simulated by calculating multiple different route changes and selecting the most successful one BEFORE making a change. This would give smarter creatures a hefty advantage over less intelligent ones as they react much faster to change.

Speed of Thinking

Another thing that needs to be taken into consideration is how often a group decides to change its strategy. A cowardly race such as goblins would probably decide quickly after loosing a few water boys. Perhaps if they were beaten badly they would pack up and leave very quickly.

Other things to consider

Connections to:

Allies

Others of same species

Treasure/Stockpiles

As a population increases, more resources will be necessary. Limited resources means that boundaries will shift over time. Groups that cannot protect a resource all the time will resort to raids or bartering (depending on alignment).

Dungeons and caves make great places to live because they are easily defensible, however many species will not live underground (humans for instance).
