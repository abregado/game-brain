---
title: "HLC - Weekly Episodic Encounters"
source: "Game Stuff/Game Ideas/HLC - Weekly Episodic Encounters"
modified: 2023-05-26
type: pitch
area: game-idea
status: "idea"
projects: ["[[Game Business & Funding]]", "[[D&D Homebrew]]"]
concepts: ["Weekly Episodic Encounters", "Game business & funding", "Turn-based D&D simulator", "D&D house rules"]
words: 1734
summary: "Pitch/plan for an engine releasing short story-driven episodic scenarios weekly on a social media schedule, with Steam/Patreon funding plan, sprint/dev plan, scenario dialogue ideas, and a staged spec for a minimal turn-based D&D simulator."
tags: ["area/game-idea", "project/d-d-homebrew", "project/game-business-funding", "type/pitch"]
---

## Introduction

A game project that is designed to integrate with a social media schedule. We release new playable content once a week, and once a month we increase the capabilities of the engine.

The game itself is an engine for playing very short story driven experiences that the user can create or download from the steam workshop. Think of sketch shows or bottle films but in interactive form. These start out as simple visual novel adventures, but as we add more features, become mini-adventures in the style of tabletop roleplaying games with combat, statistics and other gameplay mechanics.

## Funding plan

The initial work must be done at our own expense. I would recommend using the Three forms of payment approach I designed.

For ongoing support funding we would have an active Early Access presence on Steam and run a Patreon. Patreon supporters would get access to all new scenarios as they come out. One month after a scenario is released on Patreon (to allow for bug fixes), it would be available on Steam for \$1. The Base engine would be free and come with 1-3 scenarios (increased over time).

After a few features are in, we can hire writers to create the scenarios for us, or at least write the dialog.

Once Workshop support is available, we can do weekly Community highlights, and if a writer is very prolific, we can offer to sell their stories as DLC and do a profit share.

Such a project would also be suitable to receive De-minimis funding up to 200k per 3 years, as a “module” could simply be a new feature or larger scenario.

## Social media

Clearly the frequent releases will fit well with social media. We can also do character reveals as we build scenarios.

## Art

Just use Synty assets to begin with. As we build up a stock of known characters, perhaps we will need to hire texture artists to give some of them recognizable faces.

Since the engine part of the game would be graphics agnostic, and each scene would be generated in Unity, we can use whatever asset we feel necessary.

## Development plan

2 weeks to make a package

2 weeks to make 3 scenarios with it

Release package 1 month

Release scenarios for the other 3 weeks.

### Agile development

We would use an agile management style for this project.

We need to have space to try a sprint and then not use what we made so that experimentation can occur. Basically, sprints need to be disposable. To make this possible, I would suggest only one of us is every working on a prototypical feature branch, so that at the end of a release week there is still something small to release if the prototype fails.

### Sprint cycle

Sprints are roughly ordered below based on prerequisites, effort cost and likelihood to be core to scenarios

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>Sprint Contents</strong></th>
<th><strong>Scenario Idea</strong></th>
</tr>
<tr class="odd">
<th><p>1 scenario per Unity Scene</p>
<p>1 dialog per scenario</p>
<p>Ink based Dialog System</p>
<p>Die rolls based on character stats</p>
<p>Dialog options with included die roll tooltip</p>
<p>UI to support these</p>
<p>Fixed camera angle showing the two characters</p>
<p>characters unanimated or idling in scene.</p></th>
<th>Conversations between two characters with one or more choices between fixed outcome and random outcome.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Cinemachine integration for changing camera angles via Ink</p>
<p>Animation triggers via ink.</p>
<p>Update character prefab with new animation options</p>
<p>Characters can be directed to change location, enter or exit the scene, from ink.</p>
<p>Characters can be told to change facing, from ink.</p></th>
<th>Characters in an argument with closeups on face, animation changes, ect.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>interaction controller that works from 1st/3rd/topdown controllers</p>
<p>Keyboard, mouse and controller support</p>
<p>Dialogs are triggerable from in world</p></th>
<th>Interview some suspects.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Interaction points that roll a dice and trigger based on roll</p>
<p>In world UI to support these</p></th>
<th><p>Escape room thing “Trapped in a space”</p>
<p>Search for triggers, then return to dialog partner.</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>UI skins that can be set per character</p>
<p>Default skin can also be set.</p>
<p>Frame, font, coloration can be designated.</p>
<p>Animation.</p></th>
<th><p>A group of characters have a discussion.</p>
<p>Their UI matches their UI.</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Item inventory per character. Simple list</p>
<p>Characters can give items using ink</p>
<p>Ink can check if a player has an item</p>
<p>Characters can have comments when shown an item</p>
<p>Characters have a default comment if they dont know what the item is.</p>
<p>Show items on character model</p>
<p>In world triggers can check your inventory</p></th>
<th><p>Convince someone to give you an item to win</p>
<p>Item chain: talk to each person, find out what item they want, then find the person to get that item from.</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Scene setup from text file</p>
<p>Objects and characters set up at runtime</p>
<p>Scene Cameras positioned in scene file</p>
<p>Character prefabs needs to have a set of cameras included</p>
<p>Editor tool using Tiled or some other editor</p>
<p>Scenarios become a series of very small files (scene text file, ink files)</p>
<p>Steam Workshop, weekly community spotlight</p></th>
<th>Demo editable scene on workshop</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Items and stats can be carried over between scenarios.</p>
<p>Ink scenarios can specify to load a new scene after this one and import the save.</p></th>
<th>Three conversations, with the characters getting older between each one. Last one is the younger character sitting next to the older one as they die of old age.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Turn based combat</p>
<p>Character actions created via ink</p>
<p>Combat start modifiers via ink</p>
<p>AI written using ink or other external file.</p>
<ul>
<li><blockquote>
<p>Simple logic priority list:</p>
</blockquote>
<ul>
<li><blockquote>
<p>If A do X, else try next thing in the list</p>
</blockquote></li>
<li><blockquote>
<p>Default action</p>
</blockquote></li>
</ul></li>
</ul>
<p>Rolls for attacks, defense value, option to pump up a roll</p>
<p>Resources: HP, attack buff points</p>
<p>Combat initiated with a dialog.</p></th>
<th><p>1 PC, 1 neutral NPC vs 3 hostile NPCs</p>
<p>Actions:</p>
<ul>
<li><blockquote>
<p>Move to new far target</p>
</blockquote></li>
<li><blockquote>
<p>Move to close target and attack</p>
</blockquote></li>
<li><blockquote>
<p>Attack engaged target twice</p>
</blockquote></li>
<li><blockquote>
<p>Shoot ranged attack at target</p>
</blockquote></li>
<li><blockquote>
<p>Reposition</p>
</blockquote></li>
<li><blockquote>
<p>Run away</p>
</blockquote></li>
</ul>
<p>Several options to change starting state.</p>
<ul>
<li><blockquote>
<p>Push escorted character away = that character cannot be attacked but you go last</p>
</blockquote></li>
<li><blockquote>
<p>Rush them = you go first but take more damage for 1 turn</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Local multiplayer</p>
<p>Any player can initiate a dialog</p>
<p>Toggle splitscreen at any time</p>
<p>Revert to single screen on keypress when near eachother</p>
<p>Go to splitscreen when a player initiates dialog</p>
<p>Second player can join a dialog by interacting at the same place.</p>
<p>When two players are in a dialog, one player is in control. They decide when to skip/continue and what to ask next.</p>
<p>When two players are in a dialog, the non-controlling player can press a button. When the next conversation choice comes up, they will gain control.</p>
<p>Non-dialog in world triggers can be interacted with once by each player, until they are triggered.</p>
<p>Each player character has different dialog for the same questions</p>
<p>Each question can only be asked successfully once</p>
<p>Some questions can only be asked by some player characters</p></th>
<th></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

## Testing plan

Testing == all the old scenarios need to continue to work. How this will work, I have no idea.

### Legacy content

As old content will have been available as DLC, we need to keep it available. If the engine grows to a point where a sold scenario no longer can work, then we can offer old versions of the engine client for use with them.

## Other dialog scenario ideas

At a train station

One says to the other

"You don't look like the sort of person to be nervous"

Agent sitting on a train

Talking with the earpiece

Watching a number of people sitting in the train

Supermarket setting

Worker sees someone stealing

Confronts them about it

Space station setting

One interlocutor is in the station watching the other on cameras

The other is outside working

Hard cuts between the two

Two soldiers prone in a battlefield

Talking about home or hobbies

## 

## DnD Content?

Minimum spec for a turn based D&D simulator. Already seems like a lot.

Gridded drag and drop within a maximum range

Image in background for map

Select action and bonus action during turn per character

One stat: Strength

Three variables: walking_speed, hit_points_max, armor_class

Two actions: Attack and Dash

New weapons: Axe + Sword (strength based attack/damage)

Pawns have movement steps, which are counted from their starting location. When the attack is pressed, it is calculated and then steps count from this new location. If the dash action is pressed then the base movement is doubled and the player cannot press attack anymore.

AI: Move toward closest enemy using astar and attack, move closer again if target killed.

New enemy: Orc: 15 hp, 30ft speed, STR +3, ac 13

New Hero: Fighter: 22 hp, 30ft speed, STR +3, ac 17

Reaction: Opportunity attacks on first opportunity

New Action: Disengage

New Bonus Action: Cunning Disengage

New Condition: Slippery - does not trigger attacks of opportunity

New Stat: Dexterity

New weapon: Shortsword (dexterity based)

Display movement range with and without dash. Player can move pawn freely and line up attacks, or if they have already moved the pawn into dash range, no attacks. Once confirmed, the whole action is run at once.

While running the whole action, pawns can trigger opportunity attacks from neighbours unless they have engaged a disengage move.

New enemy: Goblin: 7hp, 30ft, STR -1, DEX +2, ac 15 Cunning Disengage

New Hero: Rogue: 18hp, 30ft, STR +0, DEX +3, ac 14 Cunning Disengage

New AI: stay 35ft away from enemies, attack then disengage, moving toward friends

New mechanic: Cover (+2/+5)

New Weapons: Throwing dagger, and Shortbow (dexterity ranged)

New weapons: Javelin (strength ranged)

New type of strike: Ranged (single range band)

New AI: attack weakest in range while staying 35 ft away from enemies.

New AI: move to attack at range, then move away again.

New AI: find best cover and wait, while shooting ranged.

New mechanic: Advantage and disadvantage

New mechanic: ranged weapon ammo

New mechanic: Free action

New Free action: Fight Poison (dc 12 test to remove poison)

New Stat: Constitution

New condition: Poisoned

New weapon effect: Saving throw

New weapon: Hand Crossbow

NEW ammunition: poison bolt (DC 12 Con save or gain poison)

New enemy: Drow scout: ac 15, speed 30ft, hp 13, STR +0, DEX +2, Hand crossbow with poison bolt, swordsword.

New enemy: Goblin poisoner: ac 13, speed 30ft, hp 7, STR -1, DEX +2, Shortbow with poison

New AI: target unpoisoned targets as priority, stay away

New AI: fire from cover, but swap to melee if engaged.
