---
title: "BS- 7drl ideas"
source: "Game Stuff/Game Ideas/BS- 7drl ideas"
modified: 2022-02-28
type: brainstorm
area: jam
status: "idea"
projects: ["[[Roguelikes & 7DRL]]", "[[City & Colony Builders]]", "[[Industry & Production Games]]", "[[Pocket Monster Games]]"]
concepts: ["7DRL", "AtmoRL", "Train RL", "Loop RL", "Combat Food Clock", "Archeology Team RL", "Abstract Monsters Combat", "Abstract-Away Roguelike", "Heroes and Dungeons RL", "Hotseat DungeonKeeper RL", "VillageRL", "Multiplayer RL", "DiveRL", "Tank / War Train Roguelike", "Armored Core RL", "Vampire Roguelike", "Chaos Warrior / Cultist RL", "N Dimensional RL", "Battletech RL", "BLAME/SLA Industries Roguelike", "Design: Roguelike Tactical Play", "Design: Roguelike Gimmicks", "Pocket Monster game", "Roguelike on Phone"]
words: 5724
summary: "Very large brainstorm dump of roguelike / 7DRL ideas: abstracted-away systems, combat ideas, tank/war-train roguelike, Armored Core RL, vampire RL, Battletech RL, BLAME-inspired RL, multiplayer RL, plus AtmoRL (station generation with power/data networks), Train RL, Loop RL, VillageRL, DiveRL and an abstract-monster combat system."
tags: ["area/jam", "project/city-colony-builders", "project/industry-production-games", "project/pocket-monster-games", "project/roguelikes-7drl", "type/brainstorm"]
---

### AtmoRL

### Random room and corrodor genertion

### Place doors

- Fill black space with Maintenace Tunnels, break them up a little bit

- Place Maintenace Doors into Corrodors

### Determine airblocks

### Add Scrubbers and vents and APCs

- Add Fire and Air Alarms

### Add power substations as abstracts

- Add gas Junctions as abstracts

- Add SMES and Engine as Abstracts

- Add Main Scrubbers, Gas Tanks, Valves as Abstracts

- Once abstract chain is complete, begin placing objects in reverse order (Engine and Tanks first)

### Once all objects placed into map (as prefabs) then start to place cables and pipes which can only go through walls and maintenance areas

### 

### Do the same but with information. 

### Each object is linked to a local controller object and to an information hub.

### Information hubs are linked through data conduits to a network controller, archive and Central Cortex

### Command Control Computers are linked to the network through Information hubs, but require that they have a direct connection to the machines they are linked with AND the router.

### Machines can be controlled manually by touching them, or but using the local control panels or the Command Controls

### Max data transfer is set by the router

### More controls being shared means more data sent on network

### More router usage means more heat and power in the whole network

### Information hubs are kept in rooms with Airblocks. 

### Train RL

- 4 way movement

- Player does not shoot or choose targets

- Facings based on location

- Carriages

  - Attacks - shoot in straight lines

  - Attacks - 360 range based

  - Aura

  - Bonuses to neighbouring carriages

  - Rams

  - Core - Control point, decides which half is the player half

  - Active Abilities

  - Non-combat abilities

  - Cargo

- Attaching

  - Push carriages by driving into them

  - Get your back carriage next to a new one to connect

  - Attach/detach button

  - Select where you detach from

  - Clock or External pressure to stop players having infinite time to reassemble

- Themes

  - Actual train

  - Monster

  - Horse drawn Wagons

- Enemies

  - Other Trains( approach ai, patrol routes)

  - Single tile mobs (melee and ranged)

  - Movable walls and obstacles

  - Minelayers

- Terrain

  - Standard roguelike generation

  - Destroyed Carriages

  - Disabling terrain, carriages in this terrain dont work

  - Shoot through but not move through

  - Roads, increase movement speed if all carraiges are on

  - Rail, makes you move slower if not all are on it, but really fast if all are one it

- Goals

  - Travel between many points

  - Traversing makes sense for a train

**Loop RL**

- Aim to get the player moving in and out of combat in a cycle

- Abiltiies

  - Select 5 fixed abilities that compliment each other

  - **Melee/Big Hit/Cry**, Stun, AOE, Dash, **Knockback/Bomb**

  - **Beam/Ranged**, Knockback, Debuff, Pull, **DoT/Weakness**

  - Ranged and Melee

  - Damage falloff over range

  - Random teleport, **Random Lightning Strike**

  - Placeable Bombs

  - One of them damages the player

  - Cooldowns only go down when using an ability

- Player has some fixed hitpoints

  - HP does not get regenerated

- Player has a shield

  - Waiting for a turn fills the shield to half

  - Waiting for a second turn fills the shield to full

- No Experience Points

- Enemies

  - Typical RL monsters (ranged, bumpers)

- Terrain

  - Typical RL terrain

  - Arena style, one screen.

  - Lots of LOS blocking terrain

- Kill all monsters with your very limited HP

- 

&nbsp;

- Pokemon Collection Mechanic - Gotta Hack em All

- Pokemon longgrass spawning. Monsters spawn in long grass

- Monster spawn but dont move toward you unless they are higher level.

- Single screen roguelike. Each screen is a room. Defeat it and move on

- Limited time to search

- Dice block gameplay. Number of dice rolled in defence. Select which dice to use on each hit as they come in. Lock dice and reroll a set number of times.

- Never end a turn adjacent to an enemy (one hit kill)

- All attacks are ranged

- All attacks have an arc and minimum range

- **All attacks have cooldowns equal to the number of remaining moves. 5 moves max, need to use them all before they activate again. One of the moves hurt yourself.**

- Auto full heal after using all abilities once

- Each attack moves you to a different place

- Bumping moves you through and past an enemy. You are dazed if you hit a wall.

- Enemy ranged attack target tiles nearby and fire on next turn after giving indication

- You can only move two tiles at a time in the same direction per turn

- **Halo shield. You have limited hp and die if you hit zero, but recover to half HP if you stand still for a turn, and to full if you stand still for two turns.**

- You can only knock enemies out. Finishing them with overkill damage lengthens the time they are knocked out for exponentially. Go for the big finish.

- Multisquare heros. Heros take 2x2 tiles. Monsters could take 1x1, 2x2 or 3x3

- Ley Lines or Mana getting sucked out of the room.

- More types of mana, spells cost different amounts of each. Replace all other consumable gameplay with this.

- Spells having multiple turns of spin up but are left behind as fixed objects

###  

### Combat Food Clock

While in combat a food clock diminishes rapidly. Combat needs to be resolved quickly, or the hero needs to run away.

Combat should be more about timing and risk taking. Killing enemies quickly should be easy to accomplish if the hero takes risks with his other resources. Kiting and taking the safe route should be obvious, but the time clock will put pressure on.

Players should be able to take an absolutely safe path through combat, but it will require running away multiple times.

### 

### team RL

Archeology RL. One or two diggers, a warrior and an archeologist.

Simple AI for heroes

Dig walls to uncover new rooms

protect non-combats with warrior

move treasure/artifacts carefully out of the dungeon/tomb

protect travel/supply lines

only one warrior

cartographer/photographer/archeologist is needed to gain points, and to move fragile peices

diggers are labourers to move heavy objects and deconstruct walls

Asyncronous turnbased multipler

Players can move as they wish but team bonuses require players to be close to eachother geographically and in the number of turns.

Players can see how many turns the others have done.

Items dropped by a player can only be picked up by players who have more turns.

Option to get help by your own ghosts?

Powerups or spells available when in range of others.

Combat system ideas

- monsters are represented on the travel map, each one has hit points and minimum damage for a hit (armor), and a group defense bonus. A fight runs automatically until victory or defeat, each turn the monsters attack as a single unit. Monsters that dont attack add their group defense to all other monsters, The hero attacks a random monster after this doing damage. Each time a monster is killed there is a chance that the others will flee to adjacent rooms. Allowing monsters to build up will mean you cant win. Monsters may also single block on themselves, adding doube the def value to their own defence.heros have a lot of defence value, and each hit can reduce this. The player should decide to leave when his armor is damaged enough that their is a good chance he will die. lone monsters check to flee every turn. [*See Here*](#abstract-monsters-choose-who-to-attack)

- Just dont get spotted

- Once you fight, the alert spreads through the dungeon

- You get one turn notice of attacks, move instead of attack to dodge

- Magic the gathering attack/defense, wait a turn without being hit to refresh your stats.

- Movement based attacks, hit only enemies nrxt to idicated tiles. Cant move only one tile

- Hit a random enemy that is adjacent after moving, being surrounded means damage is spread out

- Archery only, cant hit adjacents, one turn to aim, must lead targets, move faster than targets, very few one hit kills, enemies regenerate after a few turns undamaged

- One of each spell, use all before reloading, splash damage on most spells, discrete predicatable knockback

- Spells can only be cast on leylines, or where they cross. Each level has random leylines. Magic immune, slow moving enemies. Lure enemies onto leylines. Cast some spells only while standing on the correct combination of lines.teleport to other intersections or travelate up lines.

- Bomberman style, bump walls to place bomb, goes off the next turn hitting everything in a line

- Weapons can be thrown, and are very powerful but cannot be retrieved until after combat, cannot throw your last weapon.

- Laser gun that shoots once every 3-5 turns. More damage the longer you aim

- Disable enemies through fighting and use multiturn finishers to stop then recovering.

- Whenever you kill an enemy you get 10 free inputs that all execute instantly without time passing.

- No bumping but waiting while adjacent to the enemy will attack, and be attacked.

2014 7drl ideas Abstractaway

- Abstract away most of the supporting systems

- Food (cost per heal/rest)

- Mana (spells reload when resting)

- Timelimit (cost per room)

- Leveling (none or item enchantments)

- Dungeon generation (rooms are not connected but are random)

- Inventory (4-5 slots)

- Exploration (once the stairs are found you can go to next level at any time)

- Character class (select only a few from the available starting items and equipment)

- Focus all attention on the tile based combat

- Small single screen areas

- Target priority overrides

- Kill all creatures to clear a room before moving on, kill enough so they all flee?

- Loot rooms automatically, take only what you need to survive. simple choices

- Obvious enemy movements and strategy

- Combination of enemies makes each room interesting.

- before making a choice for the next room, the player can see what might be available in each room (throne room might have more gold, armory more weapons, storeroom has more food)

Heroes and Dungeons RL

- characters are generated randomly based on a seed

- this seed is also used to generate a very short, but harder dungeon

- players use a seed for their character and must complete the short dungeon with the character before using the character to play in other maps (shared seeds from friends)

- characters seeds could be shared as well, or be based off the characters name.

- These prologues mean that there will be randomly powerful heroes with easy dungeons and shitty heroes with hard dungeons.

- its up to the player to find a hero he like using

Hotseat DungeonKeeper RL

- One player quickly designs a dungeon from several room designs

- then he selects the type of monsters

- then he selects the type of loot

- then his opponent plays the levels

- role switch

- each design choice must be chosen before all the choices become available again

- at the end of each play through both players get a summary of eachothers heroes to help make choices for the next round of design.

- winner is the one who survives the longest

- **can record designs/hero/seed combinations for challenges to be shared**

VillageRL

- Your hero starts out next to a hut with a single villager (wifey)

- travel to nearby screens to complete single screen combats and collect loot

- return to your hut to have new structures built over time

- new villager arrive and your town grows

- only so many spaces per screen that is cleared

- allocate villagers by asking them to follow you and dropping them in the screen you want

- villagers can loot for you after you clear an area

- screens have a biome and sometimes a feature

- screens become wild again if not visited or populated

- a merchant arrives regularly to take your trade goods to town

- simple bump combat

- no melee

- return home to rest

- day night cycle

- some areas have mini dungeons

- populated areas must be adjacent

- build a road to have an "empty" plot for adjacency

- tool must be purchased from the merchant

- 

Multiplayer RL ideas

#### “race”

as you finish a level it is passed to the next player. They can see a ghost of your character based on each turn. Points are awarded for finishing early, both low turns and short real time counts for this.

There are a number of levels running at any one time. The last player will have more ghosts and can see how fast they have to go to beat the earlier players but will also have more pressure to do so.

#### punishment for slow play

players in a turn based game should be promoted to play faster. reward fast play or punish slow play.

More RL Ideas

generate ships stats

generate room list

corridors as junction to more rooms

generate room stats

place first room

generate doors for first room

add doors to first room

place room/add door loop

consider left over doors (airlocks or corridors)

while( rooms left to be placed) \>0

room to be placed = rooms left to be placed.shift()

door to be placed on = doors to be used.shift()

if (door to be used list.length ==0)

else {

DiveRL

- Limited Air

- Nitrogen Management (the bends)

- Get in and out

- layered level generation

- all levels are generated at the same time

- can “descend” at any time

- must stay on each level for a minimum time to avoid nitrogen poisoning

Proc-Gen Enemy Groups

### Rougelike on phone interface

Press and act on release

4 way movement

Prediction icons

Dodging moves enemies

Deployable cameras for killTV

Terrain that grants advantage - ie standing on high ground.

In an encounter - only limited set of items available - take 5 weild 2. When you change, unweilded items are dropped and lengthy to recoup. Boondock saints inventory management.

Each item has an ability you can use to sacrifice it for a bonus, but is recoverable at the end of the encounter.

Or one free item change per turn.

Town summaries at end of game/death. Each town has 1 major quest to resolve, outcome recorded in bones.

EG: The Town of Zigzoroth was overrun by zombies.

The town of Palemesh was rescued from harpies by a wandering stranger.

Persistence between characters - towns lives with their consequences, but they can be changed.

WHAT CAUSES TACTICAL PLAY IN EXISTING RLs?  
  
Terrain obstacles:  
  
Wall, block movement and LOS.  
Liquid, block movemnet, not LOS.  
Smoke, block LOS only. Least well used.  
Floor, block nothing.  
Window, block movement and projectiles, not LOS  
Door, toggle to block both.  
Exploding barrels, environmental tools and hazards.  
Destructible terrain.  
Terrain that buffs/penalties.  
Soft barriers - smoke only partially blocks LOS, liquid partially blocks movement (slowing, damage).

**areas where killing guys won’t yield as good rewards, or better rewards (killing near a cliff will have the enemys corpse fall over, areas with killcams for more points)**  
  
Movement options:  
  
Choke points - funnel enemies (especially melee) into narrow spaces, more easily allowing your character to defeat them.  
Corner shooting (DoomRL) - defence bonus in certain configuration.  
Running away, avoidance of too-difficult fights.  
Stairscumming - moving up/down level stairs to filter monsters into smaller groups.  
Stealth - to sneak up for backstabs or to draw the crowd.  
Aggro - peeling off single opponents at a time.  
Pillar dance - moving around pillar to avoid being hit.  
Kiting - dancing out of range of a slower monster, while hitting it.  
Movement sequences to buff - charging up damage with sequential movement in a single direction.  
'Bursting' energy - fill a meter that allows for extra actions, but requires waiting to regenerate. Essentially once per encounter use.

**your character has a number of “hero” points which can be spent to perform an interrupt ation, and take a long time (maybes requiring you to be well fed/rested) to regenerate.**  
Moving - bonus/malus for moving, not moving.  
Waiting for monster to move next you for first hit.

> **several different “wait” options. Defensive pause, charge pause (as in charge up a bigger next move/attack), rest wait, counter attack wait, ect**  
>   
> Attack options:  
>   
> Bump to hit.  
> Projectile attacks.  
> Spell attacks.  
> Damage types.  
> Switchable weapons.  
> Patterned attacks, AOE, beams.  
> Forced movement - knockback, pulling in, etc.  
> Status effects: poison, slow, haste, armor reduction, XP reduction, confusion, rot, sickness (healing prevention), movement prevention, action prevention.  
> Luring into environmental hazards.  
> Minelaying.  
> **attacks which move the enemies in predictable ways. Line up enemies and then perform short range aoe attacks.**
>
> **Attacks always hit more than one square, but there are also friendlies around to hit accidently**
>
> Resources:  
>   
> Potions, single use buff/spell/healing/teleport etc.  
> Wands (limited use, rechargable)  
> Which spells to cast from mana pool.  
> Ammunition for projectiles.
>
> **durability on items**  
> To spend health regen or damage dealing ability in a fight (fast/slow resolution).**:temporary stat loss for immediate gains/damage/protection?**  
>   
> Misc:  
> Delayed effect actions. Eg a potion doesn't heal until a few turns later.  
> Enemies that if not eliminated within X time, will trigger an effect.  
>   
>   
>   
>   
>   
> STRATEGIC PART:  
>   
> Combination of class attributes with levelling, under player control and improvisation with the items found. Fixed items swing more power back to the planning player.
>
> **the “bursting xp level” we discussed in the car on the way back from cowwaar**  
>   
>   
> Resrouces:  
> Long time action (prolonged rest, etc) to modify, heal, etc. Cost to food clock, possible ambush.  
>   
>   
>   
> Coffeebreak RL - only get XP for killing your own ghosts  
>   
> Highlander monsters - monsters fight amongst themselves a lot and gain experience, you have to get stuck in and kill fast lest the monsters become overwhelmingly high level.  
>   
> BONES FILE - what to do with dead guys  
>   
> Unknown Wolrds style magic - food wizard like GW ogre  
> Player gains 1 level each staircase descended - can respect by fighting back up the dungeon  
> then down again.**:awesome idea. coupled with multiple downward paths so the player must come up and down a few levels at a time. Lets players try a few different things, plus you can present more different obstacles on each play through**  
> Original ability you lose is never again attainable?**:injuries remove the option for abilities that you have current “equipped”. You risk taking the good end game stuff early as you might lose it to a silly situation.**
>
> TANK ROGUELIKE (INSTEAD OF MECHS EH EH) WAR TRAIN HULL!!  
>   
> dijkstra map ai, vector vs scalar field? flanking ai  
> Turret - single, double, tripel, quad mount  
> Random weapon generator  
> secondary weapons  
> defence modules  
> acquire upgrades from enemies  
> different damages for different targets  
> AA/AT/AI  
> select target for autofire guns, then manuever**:always liked the idea that your weapons/attacks are automated based on weapon settings/variables and you just focus on the movement strategy**  
> upgrade skills with AI boards?  
> can be ambushed while changing components?  
> multiple barrels better agains weaker more numerous foes - single better against tough individuals.  
> drones - defence drones, attack drones, sensor drones  
> workshops to do total rebuilds?  
> schematics for new hulls?  
> hull mounts, sponsons  
> space per mount, weight per turret and hull  
> turrets balance armor, speed, weight, space  
> hulls likewise  
> nanofab amunition  
> energy  
> elevation? 3 elevations?  
> omnidirectional movement? if so how to handle hull mounted weapons?  
> local teleporter?  
> EMP effects - corruption on screen  
> corrupt hardware = cursed item  
> armor most effective on front - but bonus to hit to front or rear arc  
> action game?  
> spotters call in airstrike  
> hacking/electronic attack device  
> energy injector/battery items (potions)  
> turret autorotate and fire at target, unless out of arc, ask for new target  
> position important, flank enemy for easier/more damaging hits**:cant flank when you are solo**  
> different enemy AI based on vehicle property - some try to slug, others to flank  
> multiple square movement?**:i had an idea for this, ask me**  
> repair item - variable rate/efficiency, healing over time.  
> missile bay has to fit launcher and ammunition  
> low rate efficient repair outside combat
>
> **damage can be repaired after combat quite fast, but a % of damage is of a more severe, longer lasting type. Big hits also cause a small % of perminent damage. This should top regen monkies where you can tank forever with high regen/resist/damage reduction as you always take a little perminent damage.**  
> special versions of itmes - howitzer, autocannon, high velocity, dam, ROF, range  
> aiming - optimal range % to hit, trending to 1/2 difference between th% and 100%, modified by  
> target size - every 3t over 60 +-1% TH%. never better than 90% or worse than 5%  
> maybe real time with pause tactical game? control multiple units?  
> defensive mortar - smoke grenades, anti infantry, anti missile?  
> each weapon has its own energy - update unit, then updates its weapons.  
> moving forward is cheapest, then diag, etc around to reverse.  
> (r) for reverse backwards without changing turret direction  
> different mobility types (track, wheel, hover, fly?) have different costs for directions.  
> turret with limited heavy slots for cannons - lighters slots for missiles and ulility.  
> missiles uses much more ammunition but lighter and strong alpha - good for glass cannon/rogue type  
> ghosts or tails to show velocity of units  
> Terrain difficulty - broken terrain makes for slow speed. Partial cover?  
> Impassible/slow terrain does not effect flyers - very dangerous chasers.  
> Stability meter - stability effects accuracy, and is effected by chassis, motility, turret. Increases with speed and moving, decreases with staying still and stationary.  
> Higher damage weapons require more stability for accurate shooting.
>
> **MINIMUM SPEED. You want to move a bit and fire, but are in a too high gear, or moved too fast last turn so instead you have to move farther than youd like, meaning you miss a target of opportunity. Player must plan movement 2-3 turns ahead.**  
>   
>   
> ARMORED CORE RL:  
>   
> normal RL controls - maybe free attacks?**each mech has a number of locked targets. the mech fires appropriate weapons at locked targets as you move around. More targets means less control over damage application, but more resistance to them moving out of arc or into cover temporarily. Less targets means you can overcome their defences, but might miss a shot or two due to them skirting behind a pole**  
> quickboost moves you two spaces, gives dodge bonus
>
> **move than one tile movement. Intercept movement from melee enemies, Chance for collision if paths cross.**
>
> **Skating momentum from minimum movement of 2-3 squares. Limited turns/direction change.**  
>   
> ridiculous destruction roguelike - multiple weapons, lasers missiles etc. like hamilton warriors.
>
> **no perm damage applied unless you reach a damage threshold over several turns. Like damage reduction/thresholds but over a few turns. Once you have dealt 14 damage out of 15 needed to do a point of HP, you will take different risks on the last turn as you stand to lose 14 damage worth of effort.**  
> procedural gunsin an RL?
>
> CHAOS WARRIOR RL  
> focused on gods, mutations, gifts, travelling the chaos wastes/eye of terror as a champion of chaos  
>   
>   
> V:TM ROGUELIKE & CK2 mod.  
> start as vampire, gain levels and powers through diablerie of random boss enemies.  
>   
> vampire boss is master of level - lesser vamps and ghouls will bear his traits and powers, giving clues to the player  
> werewolf levels  
> human levels  
> medieval? modern? future? could be different acts  
> humanity/corruption? drinking from innocents - multiple endings - lord of night, status quo, light in the dark  
> overfilling blood  
> agro damage  
> regeneration rate of mild damage, automatic?  
>   
> abilities:  
> flash - teleport x squares, damage all enemies in between.  
>   
> enemies:  
> coloured in red - brighter red = more blood  
> skeleton  
> human  
> zombie  
> ghoul  
>   
> **cycle based levels. each night is a level with limited time available**
>
> **player must find “food”, complete part of the level/defeat an enemy or two, then seek shelter for the day**
>
> **stealth component could be to do with feeding**
>
> **combat componenet could be against other vampires**
>
> **can always challenge the boss during any play cycle, but the player has to judge when he is ready (dont say YOUR LEVEL 20 NOW YOU CAN WIN EASY)**
>
> **unless very weak, combat vs humans is bump to kill instantly**
>
> **bump to grab a human, then press wait for several turns to drain them, when you move away from them you perform a killing blow for free. combat against humans would be a dance between enemies, waiting for a short drink between moving to the next target. Take advantage of one enemy reloading a shotgun/panicking, to drink for an extra turn from his buddy.**  
>   
> powers:  
> strength  
> speed  
> toughness  
> hypnosis - illusion  
> sense  
> necromancy  
> transformation - bat beast  
> stealth  
>   
>   
>   
> cultist-chan RL/wh40k chaos cultist RL  
>   
> level up favour with gods by doing appropriate things  
> using shrines will dice roll - maybe boons, maybe mutations etc  
> start in the eye of terror  
>   
> eldar scout character creation - select previous paths to generate starting skills/class  
>   
>   
> //made this one  
> N DIMENSIONAL RL  
>   
> 9 dimensions? as many as I like.  
> visually represented by a series of columns - rows of keys move forward or backwards along axis of each dimension.  
> space ship  
> different dimension cost more to move in?  
> monsters move towards player in different pattenrs - some sort of adjacency warning device  
> monsters can move and fire in specific restricted dimensions - differing patterns of persuit  
> hyperspace ship themed - "you awaken to the cold scraping of a particle beam on your hull. how many millenia have you slept? no matter".  
> dialogue upadtes to give plot.  
>   
> battletech RL  
> -momentum: the longer you travel in one direction, take easy bends, the faster you travel.  
> display speed and direction. direction orders are acceleration. no order is coast  
> firing weapons takes 0s.  
>   
> ATTRIBUTES OF MECHS/items  
> -stability, when firing penalties begin with speed  
> -tracking, how much they counter target speed (modifiable by turret  
> -weight limits of hull  
> -transverse component to hit penalty  
>   
> diagonal movement costs? (1.41) or hex?  
>   
> timing - each actor is stored in the master array. each engine tick the array is stepped through, checking each actor to see if they ahve an action. If yes, they act (shoot/move/etc).  
> shooting and moving each have a separate cooldown.  
>   
>   
> ROGUELIKE  
>   
>   
>   
> objectives:  
>   
> different classes have different end goals - must battle the other classes to get a different end  
>   
> SLA/BLAME! heavy influence, but original material. Blobber/squad? Individual? JA?  
> More money for killing people on TV/with melee weapons.  
> find TV crews who follow you like NPCs/companions - bonus money/xp while they live.**:awesome idea. perhaps this is the only way to get xp. The player will want to avoid combat and only kill enough enemies to make them flee. A bit different to the standard “clear each dungeon level” RL. stealthing through to the next level gives you XP based on NPCs alive. Zombie survival theme maybe?**  
>   
> classes - heavy weapons guy, stealth guy?, speed guy, hacker guy?  
> human - comes with armor, equiptment based upgrades  
> synthetic - xp based upgrades?  
>   
> levels:  
>   
> falling off ledges but surviving and being on a new level: **parallax scrolling :D**  
> uptown - wealthy gangers, delinquints, infiltrators  
> midtown - same as above  
> downtown - real gangers, mercs,  
> fighting in melee gives bonus money  
> each level is a floor - some have towns that you can heal etc - some have monsters. destructible terrain sometimes.  
> like blame - matter creation towers? builders?  
>   
> xp for clearing/escaping, not just slaughtering monsters - exploration based objectives/xp  
> save townships encountered - miniquests  
>   
> monsters - wild synthetics, evil synthetics, humans of various sorts, monsters, robots  
> separate magazine/ammunition count  
>   
> overworld map - give sense of scale/progress.  
> **can also force revisiting hub areas to show progress. Provide a faster method of transport for old areas so the player can go though unexciting areas again faster (unlock door, start elevator, teleporters, escalators, tunnels). Anything that lets them see they are returning to the same area but things are different.**  
>   
> 7drl - manchine skin wearing?  
>   
> recommended to use FSM for AI.

Gimmicks

Inventory:

Autopickup/autoequip - Vicious orcs had auto select better equipment

Only 2 slots - left and right hand I guess, or abstract them. Collecting a new items means dropping an existing one. one button for each hand to pickup. picking up will drop old item.

Combat:

Hit multiple squares. Each weapon could effect a different area. Monsters could all have area damage so you must learn their patterns to dodge.

Bumping/no bumping. Tough question. Bumping to attack is very rougelike. Furiously tapping the F key in DoomRL was exciting!

Levels:

Unending procgen. Standard kinda rougelike thing.

Notrium style levels. Procedurally placed large parts.

Holes in level looking down to lower floor. As discussed about BLAMErl. Paralax scrolled layers, each dungeon floor below can be seen when moving near the void. Showing multiple levels below may create a exciting image. Being knocked off the edge of a walkway might be a good mechanic for perma death.

Persistant world. Permadeath is in for your character but the game world persists. Each new life you will have some knowledge of the map. Would work best with branching maps, and many loop connections.

Level tranition:

Teleporter one way. No way to test the waters

Find the exit. Each level has a hidden exit that requires you to visit several locations on the level.

Jump out any tile leading ti the abyss. to go with the paralax level display earlier. You simply find an edge which is over the next level and jump off, landing in the next lowest level.

Multiple exits. Use procgen to create multiple levels connected to each level. The player can comeback to choose a new one if the last one was too hard/was a dead end. The number of connected dungeons increased exponentially.

Monsters:

Multitile monsters. Hit locations/crit damage based on tile hit

Multi hit location monsters. Choose where to hit enemies. Learn their weaknesses.

Afraid gang monsters. Monsters wont throw their lives away fighting you. They will run away to find help when injured. Perhaps monsters that survive and get away will be tougher in the next play through.

Enemy animosity

Different senses (smell, sound, magical, psychic)

Monsters modify the game world.

Traps

Multipart traps. Triggers and effectors, but with many parts inbetween that are connected to eachother in a chain. All these parts can be discovered. Attempting to disable a trap from any part may trigger it, but it can only be triggered without your intervention from the trigger point (chest/pressure plate/lever).

Goals:

Can start the last level at anytime. You carry a portal device that takes you to the boss. You can begin with ready.

Pile the slippers high! You must find several items, which you can only carry one of at a single time. These must be brought to the starting area. You can use different characters to complete the main goal

Multiplaythrough goals. Parts of the goal that are complete when you die do not have to be repeated.Promotes players playing multiple times as not all of their work is unraveled.

Each character has a personal goal that must be accomplished. PROCGEN objectives

Time pressure

Hunger bar. How to make it interesting

other limited resources you might need to live: Air, water,company,sanity,blood,ammunition,

### abstract monsters choose who to attack

Types of Monster:

- ratman. Small (5 hp), weak (2 defense), aggressive (50% attack chance), 8 attack damage, Cowardly (40% block chance), 10% help others, Group Bonus 1, 80% flee chance, packs of 5+

- golem. Huge (30hp), tough (5 def), defensive (50% chance to help others), 15 attack damage, 30% block self, 10% attack,, group bonus 5, 0% flee chance unless alone. support (comes with other pack)

- goatman. medium (7hp, 3 defence), balanced (33% attack, block, help), group bonus 2, 30% flee chance. packs of 2-3

- turret. weak (2hp, 1 defense), passive(80% block, 20% attack), group bonus 10, 0% flee chance, damage 10, support creature.

&nbsp;

- Mushrooman

- Fourarms

- Eyetopus

- Bluedrake

- Redscythe devil

- Freshalien

- Bluemagi

- Facegolem

The combat strategy comes from selecting which enemy to hit, to block or to run. Each turn the enemies randomly take a stance (attack, block or help/support). The player can then see which stance each enemy has and select a target or chose to defend. Weapons cause a range of damage, and if that damage is over the total defence, then the weapon causes its Wound stat in damage.
