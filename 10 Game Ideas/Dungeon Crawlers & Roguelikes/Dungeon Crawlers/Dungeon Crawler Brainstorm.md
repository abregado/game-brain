---
title: "Dungeon Crawler Brainstorm"
source: "Game Stuff/Dungeon Crawler Brainstorm"
modified: 2026-03-20
type: brainstorm
area: jam
status: "idea"
projects: ["[[Dungeon Crawlers]]", "[[Game Jams]]"]
concepts: ["Grid Crawler (Godot)", "Design: Grid Crawler UX", "Ludum Dare"]
words: 522
summary: "Notes on grid-based dungeon crawler UX and a Godot 4 prompt for a basic grid crawler, with the jam rules requirements of a dungeon crawler jam."
contains_external_material: "Jam requirements text appears copied from a jam page"
tags: ["area/jam", "project/dungeon-crawlers", "project/game-jams", "type/brainstorm"]
---

Dungeon Crawler

What i dont like or understand about this genre. Why limit the UX? How do we turn this into part of the gameplay?

Mouse look allowed but isn’t allowed to be part of your direction selection.

Prompt

We are building a Dungeon Crawler (aka Grid Crawler) in Godot 4.

The first task is to create a basic grid crawler game that we can expand later with new mechanics.

The player views the game from first person

The map is divided into cells on a grid.

The player occupies one cell and has a cardinal facing.

The player can move to the cell in front of them with w.

The player can move to the cell in behind them with w.

The player can strafe to the cells to the side of them with a/d

The player can change facing with q/e

Jam requirements

The game must have first-person exploration at all times. Exceptions are point to point overworld map movement (fast travel), combat screens, cut scenes, town screen, inventory screen, other relevant screens.

The game must have explorable locations. It doesn't have to be a dungeon in the traditional sense. It can be urban environments, outdoors, spaceship interiors, planetary surfaces etc. (depending on the jam theme). Whichever environment the game has it must be viewed and explored in first-person.

The game must feature step movement on a square grid (no hexagons, octagons, etc.). Smooth transitions between grid squares are allowed. Half-steps or dividing a logical grid square into smaller squares are NOT accepted. The size of a square should equal the size of the wall segments it is connected to. Consider a grid square as a cube with a ground, four walls, and a ceiling. If there are visible enemies, they must also move on the same grid as the player.

The game must feature 90-degree turns in four cardinal directions. Smooth transitions between 90-degree angles are allowed.

Turning must be invoked by keyboard (or gamepad) control. Mouse-look is permitted as a temporary way to look around, but it should snap to 90 degrees when not in use. Games that allow 90-degree turns up and down are also acceptable.

The game must have a player controlled character (or party of characters), or the abstraction of a character or persona.

The game must at the very least have some basic stats. (Minimum a single health/power bar)

The game must have combat or a similar mechanic for determining outcome of certain situations, enemy encounters and events.

The game must have a win condition.

The game must have a death/perish/fail condition, or some other end-of-game mechanic. Roguelite mechanics where you restart game upon death but retain some progress is allowed.

The game must have at least one way to affect character stat(s). Examples are resting, potions, items with bonuses, food, water, powerups etc.

The game must include an interpretation of the (to-be-announced) theme.

Your game must not contain nudity, hateful language or visuals. Please consider avoiding extremely strong language and excessive gore, as the games in this jam should be suitable for a general audience. Failure to do so may result in disqualification.
