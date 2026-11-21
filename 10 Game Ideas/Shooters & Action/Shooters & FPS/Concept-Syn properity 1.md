---
title: "Concept-Syn properity 1"
source: "Game Stuff/Game Ideas/Concept-Syn_properity_1"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Shooters & FPS]]"]
concepts: ["Source Engine Map Ideas", "Synergy Coop Maps"]
words: 644
summary: "Source (Synergy) co-op map design: rebels fight Combine dropship waves and a chopper at a crater, with spawn, street and dropzone sections plus Hammer implementation notes."
tags: ["area/game-idea", "project/shooters-fps", "type/design-doc"]
---

Syn_prosperity_1

SETTING/PLOT

After the destruction of the c17 citadel, combine forces from other areas arrive to determine what happened. The rebellion is caught while looking for survivors in the outskirts of the crater. Complete the objectives and help round up any stragglers.

CONCEPTS

Teamwork – The map should not be able to be completed with one player, this is the essence of a team objective

Punishment – Players who rush ahead should be punished, usually with death

Stepping Stones – Players move forward to the next puzzle and then are based in that area until the puzzle/objective is complete.

Objective Based – Killing all the NPCs is secondary to the objectives. This will probably involve unlimited or near infinite supplies of NPCs.

\[IMG\]http://i443.photobucket.com/albums/qq160/Abregado/syn_prosperity_1.png\[/IMG\]

SPAWN

The players spawn in a rebellion rally point where they can gear up and head for the street. Plenty of ammunition and weapons respawn quickly here. There is only one exit to the street.

STREET

Two story buildings flank the main section of the road. Destruction is high from the explosion but some buildings still stand. A combine dropship lands at a makeshift dropzone up ahead, letting out a squad of troops. The players must push forward to capture the dropzone and de-activate the landing beacon. Once all the soldiers are dead, another dropship lands with more troops after 20 or 30 seconds. The players must fall back to the spawn for more ammo or utilize ammo from fallen enemies. They can also choose to take shelter in one of the larger buildings halfway along the road where ammo and health spawns.

DROPZONE

Once the beacon at the drop zone has been de-activated, the players are given an opportunity to restock. An air raid siren sounds and a combine chopper flies in. The players must defeat the chopper without the use of RPGs. It also will not drop bombs for the players to “punt” back at it. The players must use 4 mounted guns that are scattered around the level. Each one has a limited amount of ammunition, and while there is a player using it, the chopper will attempt to destroy each emplacement with a salvo of missiles. If all the emplacements are destroyed and the chopper is still flying then it begins to drop bombs and the players can punt these back at it.

2 smaller squads of troops will enter from the outskirts of the level and begin attacking the players. Some players will have to hold off the troops while the others try to get to the emplacements.

DIFFICULTY AND REPLAYABILITY

Depending on how long it takes the players to deactivate the beacon, more troops will spawn with the chopper. However to counter this, each time the dropship lands, the troops inside will get harder and more numerous. This gives the humans a decent challenge regardless of how they decide to play.

HAMMER SIDE

Setting up the nodepaths and triggers so that the soldiers actually storm the builds that the players are holed up in will be the tricky bit. Each squad of troops will respawn once the last member is killed, and be flown in via dropship. Perhaps the soldiers should be split into two squads to stop the players killing all but one enemy and running for the beacon. 2 squads of 10 combine should keep 6 players busy.

The mounted guns should all be func_tank and the emplacements they are on should be built using func_brush and func_breakable so that as they take damage they look more ruined. Finally a very tough func_breakable will trigger the chopper to move to a particular point and fire its missiles. The explosions should use the right mix of phy_convert and func_breakable (on trigger) triggered through a logic_relay. The relay should also destroy the converted physics objects after 20 or so seconds to quell any lag issues.
