---
title: "Project DRC - Design Doc"
source: "Game Stuff/Game Ideas/Project DRC - Design Doc"
modified: 2014-05-16
type: design-doc
area: game-idea
status: "prototyped"
projects: []
concepts: ["Project DRC", "Design: Bot Behaviour Types", "Design: Procedural Level Generation", "Design: Jump System", "Design: Target Acquisition Priorities", "Design: Mobile Monetisation"]
words: 2679
summary: "Design doc for a turn-based mobile/web game where a UFO deploys swarms of robots against enemy robot guards to collect resources across procedurally generated worlds of ~10 single-screen levels. Covers finalised features, many bot behaviour types, open questions, feedback from Steve, and prototype plans (combat proto, level generation proto)."
tags: ["area/game-idea", "type/design-doc"]
---

## Finalised Features

### Play Experience

The player controls a UFO type craft and attempts collect resources from the local environment before progressing to the next level. These resource piles are guarded by enemy robots, which the player can fight by deploying his own swarm of robots.

### Hexes or Squares

Squares.

### Input Limiting

5-10 times per second to stop massive DT buildup. This can be modified if we use the state animation system.

### Particle/Animation system

bots will use a state animation system to show if they will move or fire this turn. This only updates when the player stops input. Units will slide to their new locations and then update their animation, but if the player inputs again before it is done then the bots will jump to the new location and update their animation immediately.

### New Jump System

The Jump take a fixed number of turns to charge up, then the player can move to the exit location, press the wait button and then go to the next level. No resources are consumed for Jumping. The Jump location will be visible at the start of a level, but should look not available. Juice animations when it becomes available are also a must.

### Perspective Isometric or Planview

180 degree Oblique Projection

### World Design

Each world is made up of a series of Levels (~10) of similar difficulty that use the same tileset. Terrain features are randomly created and added to a “terrain library” that all Levels in this world will use. Unique, hand crafted features can also be added, although these should be kept to a minimum.

Each world also has components to build a subset of the different robot varieties. Players must use the same robots as the local enemies.

A set of available robots is also generated per world. This should include one unique bot for this world type, and then a subset of the remaining bots.

The Worldgen seed is based on todays date. The seed is incremented each time the player wins or loses a world. Every time the player wins a world then the next world will be harder.

### Level Design

Each Level is designed to fit on a single screen, no scrolling or exploring is needed on the part of the player. Since this is a turn based game, we want the player to be able to assess the entire level and formulate a strategy before making the first move.

The terrain is made up of pre-generated terrain features from the Worlds terrain library. These are placed procedurally into the level to create a different landscape. Objective terrain is added last and then a “solvability” check is run to adjust the level geometry. If a resource point location, these also contain the amount of type of bot that will spawn at that location, as well as resource quantities.

The Level tileset is also drawn from the world tileset, so that each level in a World will have the same graphical style.

## Features Under Discussion

### Multi bot deploy

The player can choose 3-5 bots to deploy in a single turn. A secondary squad building screen can be used in which the game is paused.

### Shooting manager?

Should each bot manage its own shooting, or have a manager for them all together?

### Building Bots and Resources

The enemies that the player will face are the same variety as the ones he will use. Each world has a single unique type and some randomly selected ones. The player gets a starting allocation of bots, and then must raid supply areas in each Level for more. Each storage area contains a single type of bot, and a limited supply of them.

should bots be placed perfectly underneath the ufo?

perhaps in a 3x3 area underneath?

if there is already a bot is it forced to move?

multiple turns to deploy some bots?

bot deployment when on top of a resource point?

### LOW PRIORITY: Ambient SFX and Music that differs for each world

### Boss Fights

There should be one at the end of each world. Unsure if these will be mobile bosses or static installations

### Terrain types and World objects

for now we will have one type of terrain that blocks bots but not the UFO. In addition we will have point objects that generate fields of effect around them. Some examples could be

- Sam site that forbits UFO movement in the area, or damages it if it comes in range

- Bot immobilizer, slows down bots in this area

- Anti-missile, makes bots that fire missiles less effective

these areas and how they overlap should create an interesting scenario each level

Bonus movement could be awarded for driving on a special type of terrain as well.

UFO movement should be unblockable but perhaps enemy installations don't allow you to move into range until they are destroyed. (Sam sites?)

### Graphic Content quantity

if each world has a unique bot, and there are three additional types, with three world types, there will be a total of 9 world combinations. We would need six bot ideas (three new ones) and three sets of art.

Currently we have two movement types, ground and air. We have one type of terrain that blocks one type of movement (mountains that block ground movement). Animations for these are nesseasy.

Each Bot needs its on firing animation and particles. It would be easiest if all shooting was either ray effects or particle effects, but we could have both.

GRaphic representation of bot damage?

### Saving and Pause

The player can pause at any time. When the focus is removed from the game, it will save and pause. If the application is closed then the game will resume its old state when it is reopened.

### Combat and Damage Mechanics

Everything does one damage. Range and HP differ between bot types. Some bots might shoot multiple times per turn. Bots “spooling up” needs to be addressed as well.

### Target Acquisition

Instead of damage types, bots could have all of the different target types listed in an array to determine which priority they attack. Artillery might fire at enemy bases before bots, making them require support. This could be better than scissors-paper-rock effects.

### Bot Varieties

two different behaviors for each bot, selectable when you spawn them?

Movement Modes: Walker and Flyer with varying speeds

kingbot - moves toward bots but never moves outside of 5 tiles from where you put it. Moves back to the centre when nothing in range.

akimbobot - if there are two enemies in range it shoots once at each, if only one it moves and shoots

harasser - shoots and then moves away, moves toward nearest enemy until in range

Toughbot - is tough and attacks bases

FastBot - moves fast and hunts other bots

Artillerybot - move, deploys, then has longer range

Shielding Bot - moves, deploys, then has an area which protects other bots and the UFO

smartbot - uses smart pathfinding

kitebot - moves to a maximum range of a point and then moves in a circle around it

defenderbot - stays in formation around the ufo

flybot - uses the same movement as the ufo

SAMbot - hunts down other UFOs

~~stalker - waits until something moves within range then jumps on it, very fast, short range, invisible until it attacks~~

~~wormbot - is immune to terrain and damage until it attacks. hunts down bots~~

~~magnetbot - long range, but only does damage if there are three enemy bots nearby, but then does extra damage to all three!~~

minigunbot - doesnt fire on the first two turns when it can, then it fires twice every turn after

**climberbot - moves to the nearest cliff/terrain feature, climbs up, then has a long range attack**

**troopbot - moves toward the ufo. once there are more than 4 near eachother then they will attack a location. If there is less than three then they move back toward the UFO.**

decoybot - moves away from the UFO and attracts other things that move towards the UFO

beaconbot - stationary and like the decoybot

**leaderbot - attacks other bots, andmakes other friendlies within range change behavior to “attack other bots**”

**shamanbot - attacks bases, and makes other friendlies within range change behavior to “attack bases”**

scarebot - other bots move away from this bot, it moves towards enemy bots

### Ambient SFX and Music

Per world, or the same throughout?

### Pathfinding and Behaviors

Auto agress?

Detection radius?

Questions for steve

Progression?

Persistence of player resources?

Bots that cost 2 resources?

Save in the middle of a world or only at the end?

Save in the middle of a level or only at the end?

placeable beacons for your robots to move towards

not brining offworld bots means that unique bots are not as interesting. THey will always be facing themselves, and its only acase if their counter is available locally or not.

terrain types and movement modes

Platform: Mobile and Web

Codebase: Undecided

Documentation: text file in repo

Contact Steve on love2d irc or steam

Mechanics from proto that need reworking

User Interface

- “hover”/information mode for mobiles - how to handle this?

- campaign mode? Something to show progression?

- tutorial - first world is hand made, gated tutorial?

Level generation

- solvable levels

- granular difficulty adjustment

- terrain features

- different tilesets

- terrain types

- tileset blending

resolution detection

- landscape and portrait mode

movement system

- terrain types

graphics

- two frame animation

- particle system

- world tilesets

- better display of the path bots take

combat complexity

- weapon ranges based on tiles

- different weapon types

- less obvious scissor/paper/rock effect

- bots working together in more obvious ways

- more bot types

- multipart bots

new ejump system

- more intuitive

- less awkward

- more obvious when you can make each kind of jump

- remove emergency jump?

control scheme

- tap a quadrant to move

- bot buttons shown on the sides

- next level button

- information mode

Move to Hexes or Isometric. Control issues?. The quadrant tapping to move is too good of an idea to waste

Weapon ranges to tiles - 100% agree

Clean up Ejump/Jump - I would move them to large buttons on one side of the screen that only are visible when the jump is available

2 frame animations, easy to do if the art is there

Music - of course, but could also read from the users music library

Input acnologment - It already makes a sound every time you click something, becasue everything that you can do has a sound effect! For menu related actions, agree++

Worlds: I was thinking that there could be a short “Tutorial” world that can be played once.

Different art for each world is good, artist/art budget willing.

Boss levels are a good idea as well, just surviving until you can jump is probably not a good enough climax. Bosses could be installations with different parts that can be destroyed separately.

Powerups…. were you thnking persistance between levels? between play sessions? other options could be that after completing a world you can select one of three Boss-specific powerups that effect you for the next world. Then we could have any world selectable like Megaman. This way the player chooses the order of the levels and which powerups to use on which worlds.

Campaign mode: just a non-linear way to delivering the worlds/levels/content. Let the player decide which order to play the levels. This also means we could put in some sort of…

Permadeath. So the player loses his progress when he dies. Turns it into more of a survival game. Is this actually nessesary?

More bot types: Each world could have a single unique bot type, and two out of three common types. Carrying bots between worlds would mean your inventory might fill up with many types of bots, which might cause UI issues.

UFO types. Were these going to become bosses? If not, having different types, especially different behavior would be important.

More terrain types: I think is would be very important to the feeling of the different worlds.

control scheme - i think those are on the money.

monitization - i would just go for the \$1 option for ease, playable on pc for free

other concerns of mine below…

crafted levels vs prc gen

If we have an endless mode then we def need proc gen. Im sure I can come up with a better algorithm for this but it would be more time expensive than crafting say 40 levels in tiled.

Crafted Levels would let us minimize the need for a tutorial as we could craft a set of 10 increasingly difficult, and mechanically tailored levels.

Also we could put in key challenges at certain points.

Procgen… I would probably create a system with crafted feature objects and well as proc’d terrain features. Re-using similar terrain features for one world could also help to develop a visual style for each world. More terrain types would help a lot.

Tutorial. I was thinking about a blank map (with faked mechanics like the real game) where the player can experiemnt with the controls and see what everything does. hint boxes could pop up or have a simple “next” button once the player wants to see the next hint/prompt. Perhaps in this mode the player can see weapon ranges and hitpoints.

Having less tiles per map means we will have to use the space much better. It also means the pathfinding will need to be smarter. Alo the number of bots deployed in each level will need to be lowered.

Deployment Cap?

Wait button when you tap on the centre of the screen?

Frenzy mode. If you dont make an input in 0.3 seconds the game thinks you mean WAIT. could create a much faster paced game. Also is a kind of soft time limit.

Defence mode - you just have to survive as many rounds as possible, each round you get some resources and killing enemy bots gives you some as well. Perhaps you unlock each bot type in the main game to encourage players to try out different modes (mobile games do this very frequently)

Difficulty settings? Lots of mobile games just want to play of casual mode and we like to make hardcore modes. Perhaps this just affects the auto-wait time mentioned above. Could just have a strategic (turn based) or tactical (semi realtime) mode…

Animation - only animated when moving? Having 2 frame animation while waiting for user input might make it unclear that the game is waiting for you. Will each unit move sequentially, or all at once as they do now? If we have less bots, it may be better to use sequential movement as the placement of individual bots is MUCH more important.

input repeat for ease if moving long distance

Testbed prototypes

prototype objective graphics

random placement of objects

combinations

minimum number of tiles for maximum combinations

value?

combat and animation proto

units spawn on the left and move to the right

units of another team spawn on the right and move left

units detect eachother and fight

used to test state change, combat mechanics, game loop and animations

no input or UI

Level generation proto

ui to select world type

tap to generate a new level

after 10 levels, return to world selection

generation

- place objective points

- generate noise

- generate less dense noise around objectives

- 4,5 cellgen on large map

- add random features

- detect open areas

- detect paths between objectives

- widen paths between objectives

detection

- locate middle most objective

- detect closest objectives

- attempt to fit both in a rectangle, evening margins

- fill edge

- retest paths between objectives

- drill paths, or expand flat area if failed

- detect additional objectives

- replace additional objectives with supply areas.
