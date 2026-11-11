---
title: "Love Libraries To Do"
source: "Game Stuff/Game Ideas/Love Libraries To Do"
modified: 2015-02-13
type: planning
area: other
status: "designed"
projects: []
concepts: ["Design: Love2D Reusable Libraries", "Design: Campaign Level Manager"]
words: 878
summary: "Technical to-do/spec for reusable LÖVE (Lua) libraries: tutorial overlay manager, campaign level manager, disposable gamestate manager, button lists, controllers and language module."
tags: ["area/other", "type/planning"]
---

Tutorial Library

- Slide instance constructor, as there may be several tutorials in one game

- properties of the manager

  - arrow tween

  - circle tween

  - tutorial alpha tween

  - arrow sprite

  - circle sprite

  - textbox background spritesheet

  - font

  - colors of default, non-sprited overlays

- setter functions for the above

- sound effects on display()

- cancel sound effect on complete()

&nbsp;

- addTutorial: adds a tutorial overlay

  - gets a string as identifier

  - has an array of drawn objects

  - has a interger state: 0 - unshown can be triggered, 1 - is visible, \>2 - invisible cannot be triggered

- display: draws any currently active tutorials

- update: updates tweens

- logic functions

  - display(stringID,{extra params}): sets a tut to status 1if it is at status 0 and no other tuts are currently at status 1, array of extra params is passed to the initTut function

  - complete(stringID,nextTut) sets a tut to status 2 if it is status 1, sets nextTut to status 0

  - prepare(stringID) sets a tut to status 0

  - tutmanager.draw() draws the current tutorial

  - passing of extra params on prepare, display

- display objects

  - Avoiding Text Box. double bordered box with wrapping text. Dynamically avoids the given x,y

  - fixed text box. as above but is rendered at the x,y and does not move

  - active arrow. a bobbing arrow pointing at the given x,y. third parameter determines which way the arrow is pointing/bobbing

  - portrait bubble. character portrait in one corner with speech bubble

  - Magnification: renders the given rect at the given magnification over the top of the given rect

  - Circle indicator. draws a circle at x,y of the given size. The radius should flex in and out

  - CircleLine Indicator. draws a line from x,y which connects to a Circle indicator at tx,ty. the circle will oscillate in radius.

Level Manager - Campaign thingo

Goals:

- Support for branching level options

- Support for Main Quest, Side Quest, Tertiary/Random Encounter

- Multiple Side Quest Chains

- Multiple positive, negative and nil dependencies (Quest 3 is available if Quest 1 was beaten, and quest 2 was failed)

- Branching Chains

- Option to pass and fail levels

Variables per Level

- Priority (1 = main, 2 = side, 3 = tertiary/optional, but can have any number of priorities)

- Completion: manager must track which levels you have completed. 0 = failure, 1=victory, 2 = unplayed

- Dependance: Levels in chains depend on their predecessors

- Progression: Levels have a variable to show in which order they appear (to help plan player progression and difficulty)

Logic

- getLevels(progression): returns all levels at this progression rating that can be accessed based on Dependance. These are sorted in order of their priority

- addLevel(Priority, progression, dependency list, level object): Creates a new level and adds it to the manager

- completeLevel(level, value): sets a level completion to 1 (victory) or 0 (failure)

- drawLevelMap(): visualizes the campaign using circles and lines, showing priority, progression level, dependencies and completion

Disposable Gamestate Manager

Goals

- Creates disposable gamestates to move through

- Automatically adds functionality

- Used for menus and repeated gamestates

Types

- Pause Menu: Continue/Options buttons

- Level Select Menu (Choice): Passed a result from the Campaign Manager, it will display your options

- Level Select Menu (Grid): Passed a Campaign Manager, it will display all levels, including unavailable missions. For Puzzle games with linear unlocks

- Level Select Menu (Tree): A horizontally scrollable tree map showing levels you have completed, and those that will be available later

- Credits Menu: Will display and scroll through a passed array of text, then move on automatically. Also accepts a skip button.

- Options Menu: Displays sound, language and other options. Also close menu button

- Landing Language (grid): Displays languages as flag tile buttons in a grid. Useful for initial loading of game.

- Level Complete Screen (% Tally): will display, tally and list each variable passed to it one at a time, with a total completion %

- Intro Screen (Slam/Pop): Two passed images will enter from the top and bottom, then a third will pop from the center out, either removing the other two or not. 4 Sound effects are passed in an array (slide, slam, pop, continue). game state ends on keypress or touch

Button List

- configurable grid rows/columns

- single x,y pos -\> feeds to buttons on draw

- combination of IconButton and TextLabel

- input width/height and number of buttons and it can generate the sizing

- can disable auto generation of locations, in which case buttons must be manually placed

Button

- Pre-render button and store

Reusable Gamestates

- Transition Gamestate

- Pause Gamestate

- Tutorial Slide Gamestate

- Intro picture sequence Gamestate

Callbacks

- Resize Callback -\> resets all global size variables, triggers everything being rerendered

Controllers

- Unit Controller, Garbage disposal and creation

- Option for Z level sorting on render

- Unit Entity utilizaing Hardon Collider

- Savegame Controller -\> Multislot saves

Unit Controller

- location tracking

- distination and absolute location

- moveTo instantly func

- moveTarget to func

- different movement types (four way, vector adding, neutonian,

Language Module

- Collection of common words
