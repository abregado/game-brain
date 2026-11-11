---
title: "BS - Space Station 13 Ideas"
source: "Game Stuff/Game Ideas/BS - Space Station 13 Ideas"
modified: 2020-12-11
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Space Station 13-14|Space Station 13/14]]"]
concepts: ["Space Station 13/14", "Design: Inventory UX", "Design: Antag Moderation Tasks"]
words: 1144
summary: "Ideas for SS13: context sensitive hotkey inventory, autostow, job ban system to encourage nice play, dob-in antags and job task lists."
tags: ["area/game-idea", "project/space-station-13/14", "type/design-doc"]
---

## User Interface and hotkeys

### Context sensitive number hotkeys (1-9,Tilde)

Inventory Slots grouped into following areas with submenus

1.  Belt (1-5 or just itself if no belt is worn)

2.  Worn: Accessory - PDA, ID card, Eyes, Head (1-4)

3.  Worn: Easy - Pocket 1, Pocket 2, Hands, Ear (1-4)

4.  Worn: Inaccessible - Body, Body Exterior, Shoes (1-4)

5.  Backpack (1-7)

Press Key to access this group.

Then press the next number of access submenu items, or tilde to cancel.

If doing this with an empty hand, it will take the item to the hand

If doing this with a full hand but on an empty slot, it will stow the item

If doing this with a full hand on a full slot it will swap the items or autostow the held item if possible, dropping it it not

Pressing Tilde while in a submenu will cancel the selection

Pressing Tilde with a empty hand will pick up the nearest item or something on the floor

Pressing Tilde with a full hand will autostow the item in an appropriate Slot

Holding ALT and selecting i slot will dump that slot. Selecting a first level slot with an inventory item (backpack, belt) will dump the whole thing.

Holding CTRL and a slot will drop your held item and retrieve the slot item, or if it is a first level slot with an inventory item (belt/backpack) it will put the whole thing in your hand.

Holding SHIFT and selecting a slot will force stow an item in that slot, dumping the existing item (even if it is a first level slot)

Now all inventory changes are accessible within two button presses, all of which are within reach of WASD.

### Autostow

When swapping to another slot with full hands, automatically find a slot which fits the currently held item and stow it. If no slot is found then drop it

### Problems

Direct Intent Switching needs to be moved.

## Giving players a reason to play nice

This system is designed to encourage players to only cause trouble every few rounds. It does so by mechanically punishing players with Job bans if they do not at least act like their chosen job.

Keeping your job should be the most important thing to both Protags and Antags. There is nothing better than a round in which you win covertly as an antag, and for small player maps this should be the aim of any implemented systems.

Each job gets given 3 objectives. These are fairly simple things. At round end they need to have completed at least one otherwise they will receive a job ban. Completing more may just help bored protags.

This goes for the Antags as well. If they do not complete at least one of their Job Tasks then they will receive a job ban for that role.

If a player completes all three of their tasks in one round they will have one of their other job bans cleared.

The actual goals should involve other departments and jobs.

Dead staff and Assistants don’t have to worry about getting job bans.

## Promoting Covert Antag play

At the end of the round all living players can either pick one other player to “dob in”, or chose not to say anything. Once a timer has completed, the Antag and his missions are revealed. If an Antag had been “dobbed in” then they receive a ban for their current Job. If the player was not an Antag then the dobbing player receives a job Ban for his own job.

This should promote Antags to fly under the radar if they want to continue being Antags in later rounds using the same job. Of course if they want to be Murderboning Antags they can still join as Assistants and work their way up.

Ordering a balloon could also protect them from losing their job access.

## Task Ideas

Below are lists of minor tasks. The ones in red are “semi-antag” acts which I would consider to be “content generation”.

General: Collect 5 papers with specific Stamps on them, Collect 10 papers of any kind, Eat X of n food, Send X PDA messages, use the Request Console X times. Dont harm anyone, **Access three areas that are restricted to you, dismantle something, break 5 light bulbs, hack a door or APC, remove 5 floor plates, cut 2 wires**

Medical: Perform Surgery at least once, Clone at least one staff member, Use a needle 10 times, Apply X bruise packs, **Remove at least one limb or eye,**

Cargotech: Receive 20 crates, Use your stamp X times, Sell 20 Crates, Sell at least 5 plasma plates, **Hack the autolathe, order a weapons crate, Hack the MULES**

Engineer: Positive energy for half of the round, Replace 5 lights, Wear a gas mask for 10 minutes, Wear meson goggles for 20 minutes, Hack a door, Hack an APC, Construct one machine, **Cause 4 APCs to lose power,**

Captain: Convince the Lieutenant to go Code Red, Use your stamp no more than 5 times this round, Carry your pistol at the end of the round, **Fire your pistol, Go EVA, Request a weapons crate**

Lieutenant: Never go to Code Red, Have 20 sheets of paper in your file, Use your stamp 10 times, Collect 10 of the captains stamps, Have one of each job onboard, Go into every area

Bartender: Cook X of n food, 20 bottles of alcohol consumed on station, 10 pieces of non-vending food eaten on station, a food crate arrives at station, **put something in the Gibber, Fire your shotgun**

Chemist: Mix 5 different Chemicals, Inject 2 different Chemicals, **Melt a deckplate, a staff member was burned this round, a staff member suffered suffocation damage this round**

Janitor: Clean 5 dried bloods, clean 5 oil spills, empty 5 bins, access every department on the station, **2 people slipped over this round, have any item from any area in your backpack, clean up fresh blood**

Scientist: Feed 10 items into the Deconstructive Analyzer, Construct a tank bomb, launch something from the Railgun, a Virus or Ripley crate was ordered, **A weapon is fired in the Lab, Trigger a fire alarm in the lab**

Detective: Scan 10 items for fingerprints, smoke 10 cigarettes, drink 5 bottles of booze, **Fire your Revolver, scan a corpse for fingerprints**

Security: Apply handcuffs twice in the round, Inspect someones PDA, eat 10 donuts, **Inspect someones ear radio, Hit someone with a stun baton,**

Clown: **10 staff slipped over this round, honk 20 times, another player was deafened this round, get access to all departments, hold the captains id, hold 3 or more ids,**

Every player gets one Semi-Antag task and two others. Each of the job specific task is only ever given to one player. Empty spaces are filled with generic tasks.
