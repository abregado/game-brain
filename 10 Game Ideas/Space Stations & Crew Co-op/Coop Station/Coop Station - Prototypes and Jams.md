---
title: "Coop Station - Prototypes and Jams"
source: "Game Stuff/Game Ideas/Coop Station_ Prototypes and Jams"
modified: 2020-06-21
type: design-doc
area: game-idea
status: "prototyped"
projects: ["[[Coop Station]]", "[[Emerge]]", "[[Game Jams]]"]
concepts: ["Coop Station", "Design: Building State Machine Architecture", "Emerge", "Game Jam Prototype Ideas"]
words: 931
summary: "Prototype notes for Coop Station: event scheduler waves (heat, sandstorm, radiation), manager/state-machine architecture options, small prototype ideas and jam game concepts."
tags: ["area/game-idea", "project/coop-station", "project/emerge", "project/game-jams", "type/design-doc"]
---

Events scheduler

Add two waves to represent the suns, each adds a heat value.

When the heat value is too high or too low, add an event until it is over.

Each period should work out to be 1 hour long.

A second wave generates the sandstorms. These are much longer, around 3 hours.

A fourth wave generates the radiation events. These are much shorter, around 10 minutes and come more frequently.

Display these on a graph, and highlight the spaces where there are none of the first three. The radiation events are shown but do not block shift placement.

The player can select a space to start a shift, any time after the end of the last shift (+travel). They can also select the size of the elevator which affects the length of the Travel Phase.

Hot Event:

Machines outside operate at half speed

Solar Panels produce more power.

Scorching Heat Event:

Machines uncovered become broken

Solar Panels produce a lot of power.

Cold/Dark Event:

Movement speed reduced

Machines which are operating stop doing so.

Freezing Event

Machines uncovered are broken

Cannot interact with pallets and containers outside.

Sandstorm

Movement speed penalty outside

System 3

Input comes from unity

InputManager goes to CharacterManager, finds character, and lists which actions this button corresponds to (lift,drop,refuel, activate, ect)

CharacterManager asks BuildingManager for closest building, and based on the state, and which actions are available decides which action needs to be taken

CharacterManager calls BuildingManager.DoActionXToBuilding

BuildingManager runs ClosestBuilding.State.doActionOfType

Building.State determines outcome, possibly setting a new State on the Building. Returns a status or request (like removing an item from inventory).

BuildingManager determines what needs to change on the character based on what is returned, then makes a call to CharacterManager.

Based on what comes back, CharacterManager modifies the Character

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><ul>
<li><blockquote>
<p>Gameobjects only modified by their own controller</p>
</blockquote></li>
<li><blockquote>
<p>Feedback given when player presses a button with no effect</p>
</blockquote></li>
</ul></th>
<th><ul>
<li><blockquote>
<p>Every new state that is added means that CharacterManager and buildingManager need to have their logic updated.</p>
</blockquote></li>
<li><blockquote>
<p>InputManager and CharacterManager needs to understand which button is pressed and what it means.</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

System 4

Input from Unity

InputManager calls CharacterManager to find Input owner

If input owner found then InputManager sends input+character to BuildingManager, which passes input to Building.State if there is one in range.

Building.State makes changes to Character directly, as well as its Building, possibly replacing the state with a new one.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Pros</th>
<th>Cons</th>
</tr>
<tr class="odd">
<th><ul>
<li><blockquote>
<p>Building.State handles everything</p>
</blockquote></li>
<li><blockquote>
<p>More extensible, since each state contains its own logic.</p>
</blockquote></li>
<li><blockquote>
<p>BuildingManager only passes calls to a specific building, and has no logic of its own.</p>
</blockquote></li>
<li><blockquote>
<p>CharacterManager has none of the machine logic</p>
</blockquote></li>
</ul></th>
<th>A player cannot rebind the buttons for specific actions</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

Option 2

- Game manager deals with tick time and contains references to all managers.

- Input manager deals with input, and contains references to each player character in the game. If an input is associated with a player character, it sends a request to the character manager.

- Character manager deals with all Player characters. If it gets an input then it gives it to the correct character, and communicates between character and buildings via the building manager.

- Character manager deals with character updates

- The building manager stores and updates all building objects. It receives interaction requests from the character manager which include which character did the action and the type of action. These are handed on to the Building

- The building contains variables and has a State object. Interaction requests are passed to the state object.

- The Building State object deals with all interactions and behaviors.

Option 1

Game manager deals with tick time, keeps references to input manager, player manager, building manager.

input manager only detects button presses and position.

Input manager sends generic commands to building manager

Generic command contains which player interacted as index)

Building manager sends generic commands to building, or places new buildings/tiles

Building contains overridable work, move, update functions

Building has a state machine to change its interactions: PositiveInteraction, NegativeInteraction, AlternativeInteraction, Update.

Building state determines what it will do with update

Game manager calls updates on managers only

Input manager tells game manager if a currently unused player button has been used (new player has joined)

Click to place object. Only on tile.

Left Click an object to remove it. Max 1 object.

Object places tile 5 times.

Right Click an empty object to refill it.

Right click a working object to change its shape/rotate it.

2 character movement. Two buttons of controller.

Character can pick up 1 item and place it elsewhere

Starting area has a number of objects, no more

Time limit.

Put all objects back before the timer ends.

### Machine States

Ready

Requires resources

Working

No work to be done

Controls

Console/controller based inventory system: two rows, swap items back and forth

Caro’s Concert planning/timetabling game.

Sokoban game with push and pull. Player continuous movement, blocks tile movement.

Machine placement, timers and results. Player just interacts with mouse. See if keeping everything running is fun.

Machine placement, shared inventories within direct range, as well as “road range”. Visualization for what is connected to what.

Red green squares game in unity with UnityUI and PUN+ Classic

Red green squares game in unity with UnityUI and Quantum



Room based Fog of war mechanic.

Camera zoom and position test for multiple players on same client. Test enforcing arbitrary limits on distance between players

Resource management with recurring events in timeline. Each event just causes a state. Each state has a severity (integer) and applying the corerct resource for the correct time reduces the state.
