---
title: "BS - 4x slider economy"
source: "Game Stuff/Game Ideas/BS - 4x slider economy"
modified: 2022-02-14
type: design-doc
area: game-idea
status: "idea"
projects: ["[[FourEcks - 4X Space Empire|FourEcks / 4X Space Empire]]"]
concepts: ["4X Slider Economy", "Design: Economies", "FourEcks / 4X Space Empire"]
words: 272
summary: "Concept where the player sets production targets and the game picks resource sources, with three tries: infrastructure cost, priority list, hold/decline/grow checkboxes."
tags: ["area/game-idea", "project/fourecks-/-4x-space-empire", "type/design-doc"]
---

Concept: The player only sets which resources it would like to produce at which levels, and the game chooses which resources to exploit to achieve that goal. Changing your targets can be done at any point, but it takes time for the economy to adjust to the new targets.

Try 1: Infrastructure costs to change targets. One resource is used to move production toward the player set production targets. The more of this resource is produced, the quicker production will change to match. This resource can be useful for everything else, so that the player will want to optimise it toward zero when things are going well.

Try 2: All resources are placed in a priority list, and the player can change their order, and goal. Multiple entries of the same resource can be added to the list, so that small amounts are at high priority, and larger production targets can be placed at lower priority. The option to set “unlimited” entries is also provided, but these are always at the lowest priority, and thus only trigger if no other goals need to be reached.

Try 3: Each resource has a three stage checkbox next to its readout. The player can cycle between Hold, Decline and Grow. New facilities are produced based on which resource pairs are set to Grow/Decline. For example, if Minerals are set to decline, and Alloys set to grow, then Forges are built. If Alloys are set to grow but Minerals are set to Hold, then only new Alloy mines found will be exploited. Priority is always given to sources that give resources without costing anything (Raw sources).
