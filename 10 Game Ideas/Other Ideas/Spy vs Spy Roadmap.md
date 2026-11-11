---
title: "Spy vs Spy Roadmap"
source: "Game Stuff/Spy vs Spy Roadmap"
modified: 2021-12-19
type: planning
area: game-idea
status: "prototyped"
projects: []
concepts: ["Spy vs Spy"]
words: 486
summary: "Day-by-day dev roadmap and playtest bug list for a Spy vs Spy remake, mostly ticked off, plus bloat features (traps, remedies, items, light switch)."
tags: ["area/game-idea", "type/planning"]
---

Playtesting bugs

~~Map camera angle iis busted~~

~~Map “has item”~~

~~Winner does not currently go to You win screen~~

~~Trapped furniture wiggles a little bit every 3-5 seconds~~

~~Medical box is spawned once in every level~~

~~If everyone is dead, respawn immediately~~

Items sometimes disappear

Add a Debug view to show where items are

“Trashbag” item spawns in the centre of the room if there is no furniture when an item is dropped.

Make trapped furniture wiggle more

Disarming button - stuck for 2 seconds to be sure there is no trap.

Setting a trap takes 1 second.

Sound for setting a trap.

Spy vs Spy

[*https://www.youtube.com/watch?v=Yu2e866bEcM*](https://www.youtube.com/watch?v=Yu2e866bEcM)

[*https://www.youtube.com/watch?v=LJC7DIP5JIw*](https://www.youtube.com/watch?v=LJC7DIP5JIw)

[*https://gamefaqs.gamespot.com/nes/587639-spy-vs-spy/faqs/14615*](https://gamefaqs.gamespot.com/nes/587639-spy-vs-spy/faqs/14615)

**Day 1**

~~Camera and room switching~~

~~Splitscreen view~~

**Day 2**

~~Player movement/Rewired setup~~

~~Fighting when two players bump into each other, and one does not have an item.~~

~~Fighting animation takes 3 seconds. Winner is determined from the highest of these states.~~

1.  ~~Hurt -4~~

2.  ~~Carrying Item -1~~

~~Each button press during the fight adds 0.1~~

~~WInner becomes Hurt, Takes item from victim if the winner does not have one~~

~~IInteractable: Door - Activate to travel (no open/closed state)~~

~~IInteractable: Furniture - search animation~~

~~IInteractable takes player object, and checks if you have an item or not~~

~~Inventory - 1 item only.~~

**Day 3**

~~Briefcase item - when you hold it an find an item, it is added to the Briefcase~~

~~Inventory UI for each player.~~

~~Basic level, three-four rooms, some different furniture~~

~~Traps - Press X on a furniture/door/room centre to lay a matching trap~~

- ~~Furniture trap - kills when someone searches~~

~~Traps are single use, invisible and have no remedies for now.~~

~~Death/Respawn after 30 seconds in a random room (not the one you died in)~~

**Day 4**

~~Medical cabinet in level to remove Hurt~~

Playtest and Tweaks

**Day 5**

~~Random item placement~~

Level Design

Timelimit

~~Win/Lose screen~~

Player \# select in main menu

Polish

**Bloat Features**

~~Attacking and being hit slows you down~~

Trap Types

- Door trap - kills when someone enters or exits

- Room Trap - triggers when a player enters the room. Kills all players in the room after 3 seconds.

Remedy Furniture + Items.

Press B to discard a Remedy

Door open/closed State: They stay open. You can activate the open door to close it, or activate the “hole” to travel. Door traps can only be placed on closed doors.

Map screen - shows which rooms have items. Needs extra button.

Graphics

Sound

Two items which can be found: Knife and Club

3.  Knife +3

4.  Club +2

Weapon discarded if the player wins and the other has a quest item.

Red Herring. Item which is useless, makes a squeaking noise and shows up on map.

Light switch: Cameras go blank for 5 seconds, and the spies do not make sounds when they lay traps or move items. You can still see the eyes of the spies..
