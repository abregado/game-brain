---
title: "Coop Station - State Machine Designs"
source: "Game Stuff/Game Ideas/Coop Station_ State Machine Designs"
modified: 2020-06-07
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Coop Station]]"]
concepts: ["Coop Station", "Design: Building State Machine Architecture"]
words: 250
summary: "Two alternative Unity architectures for input -> character -> building state handling in Coop Station, with diagrams missing."
tags: ["area/game-idea", "project/coop-station", "type/design-doc"]
---

System 1

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

System 2

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
