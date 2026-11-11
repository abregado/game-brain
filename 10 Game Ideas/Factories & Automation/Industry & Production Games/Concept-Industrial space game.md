---
title: "Concept-Industrial space game"
source: "Game Stuff/Game Ideas/Concept-Industrial space game"
modified: 2013-06-12
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Industry & Production Games]]", "[[EVE-like Player Economy]]"]
concepts: ["Industrial Space Game", "EVE-like player economy", "Design: Manufacturing Tradeoffs", "Design: Pre-programmed Attack Patterns"]
words: 1669
summary: "Design for a scalable industrial space game: player-run factory ships, site claims with threat-driven NPC attacks, mercenary contracts, hardish sci-fi travel, combat patterns and repair."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/industry-production-games", "type/design-doc"]
---

**Scope Change**

At first i thought this would have to be a very large scale game from the outset. What I want is a SCALABLE game, not one with large scale!

Setting: The entire game takes place around a single planet and its moons, or in a section of the asteroid belt.

Scale: The game should be initially designed for a single player. Then later on moved to multiplayer by limiting the number of Control Points each player has.

Development Scope:

No graphics are required at the beginning as all objects are represented as points in a volume of space.

In a single player environment, no market controls need to be designed as the single player will own everything that is made. This will turn the starting product into a “survival” style game.

UI will still require a lot of work at the start. However it wont be important to develop the UI past the point where a player can control more than a handful of ships.

Industrial systems, mining, combat and all the related math will take up most of the development time

Database Systems to record all the information.

**Playcycle Expanded**

Players log on and find there are no active sites.

Solo players can explore the Solar System to find sites. (\*1)

Asteroid Belt for Metals Mining

Jupiter for Atmospheric Gas Mining

Saturn Rings for Ice Mining

Team players can create squads to explore the more dangerous areas past the outer planets

Uranus ruins (Machine Life) (\*2)

Kuiper Belt (Survival due to distance) (\*3)

When a good site is found a claim is made and auctioned off.

The new owner earns rights to “Deploy” factory ships in this area of space.

Other players must request permissions to deploy here. (\*4)

Once the first factory ship is deployed, the site begins to generate “Threat”

Also the location is broadcast system wide.

Miners arrive and begin preparing resources for a refinery ship.

As a site increases in “Threat” pirates and eventually machine life will begin arriving and attempt to destroy the factory ships.

Both quantity and quality will increase over time.

Tactics/Combinations should change according to Spawn Design

Targeting priorities and abilities of individual NPC ships will determine the range of challenges

Factory Ship owners advertise for players to defend them for a fee. Contracts options include: (\*5)

Timeframe

Renegotiation Times

Price per minute/hour

Upfront fee

Mission Success flags

Mission Failure flags

Distance from escorted ship

Payment per craft destroyed

Ammunition subsidy

Factory ships must be retooled for a particular job and run length. Mass production is much cheaper but requires being set up for longer. Which means harder enemies and more money spent on mercenaries. Mfg processes should include:

Time:Waste:Quality:Efficiency trade-offs

Batch Size

Total runtime

Retooling fees

Batch inputs or Bin loading (\*6)

By-products and Waste are actual items (can be refined or used again)

When the factory ships are finished working, they will return to a NPC station/drydock to place their goods on the market. The mercenaries mop up the remaining ships and wait until everyone has left to get the most from their contracts, then head home to repair and refit for the next mission.

Setting up for another factory run takes a while, and in the meantime mercenary/fighter players will move on to help the next set up, or if none exist will go exploring, triggering another mission eventually. This cycle should be self sustaining, even if all players decide to play solo. Well organised groups will take charge of the harder stuff, but basic requirements can be completed by younger/poorer players. Ammunition and other consumables (Fuel) could be completed by solo industrialists or very small unorganised groups.

\*1) The quantity, quality AND combination of materials in one area should be important.

\*2) In this setting Uranus has been destroyed by a self replicating AI machine sent to mine it.

\*3) Distance between objects, player groups must take everything they need to survive as they will not return home if unsuccessful.

\*4) Advertised in a mission type browser list thingo

\*5) Industrialist players will want to stay safe, but also hire the minimum number of mercenaries. Industrialists with balls will have lower operating costs.

\*6) Basic mfg runs can be done with one large factory ship, however the complex jobs, requiring several simultaneous, coordinated processes must be completed by a group of factory ships. Factory ships can open up a number of external cargo bays (incoming only) for use to transfer materials and products between ships.

**Methods of Travel**

This is supposed to be a hardish sci-fi setting. Combat maximum speeds are dependant on hull integrity and shielding. Acceleration is based on thrust:mass ratios. manoeuvring is done in an frictionless environment.

Inter-planetary travel is achieved by sub-light drive. C+ speeds are not available within the solar system. 90% light speed should suffice for the larger craft. Travel times from one side of plutos orbit to the other would be roughly 5-6 hours. This is the extreme case. Travel from Earth (starting location) to the Asteroid Belt being only 5 minutes at this speed.

Fuel costs for near C speeds are based on mass of the craft and cargo. This means that it is often cheaper to build items at the material source to avoid shipping large amounts of raw materials. Combat craft are for the same reason kept small. Only the military operates capital class sublight craft.

When a craft wishes to enter speeds close to C (really need a name for the drive system), it must align to its destination, and complete a series of jump calculations. Once these are complete it may “jump/warp/accelerate” to ~C speeds. Acceleration up to this speed will be an arbitrary value, determined over time with testing.

Ships will exit ~C Speeds at the same speed that they entered. This means that smaller more agile craft “jumping/warping” while at combat speeds may collide with objects at the other end.

(Possibility of Fines imposed for exiting ~C too fast or too close to NPC structures)

Fuel costs will be a fixed amount to enter ~C based on Mass, and a ongoing cost based on distance travelled and efficiency of ~C drive. Selecting a slower ~C speed will save on distance based fuel consumption, so pilots can select to take “the slow boat” when shipping unimportant items long distances.

the ~C Drive should require a substantial cool-down period after a long trip.

**Methods of Communication**

Instantaneous communication is available. The pilots themselves are located on the Earth Station and control spacecraft remotely. Due to very long travel times and high fuel costs, often pilots will purchase ships at a farther destination rather than remotely fly ships to those destinations. (creating localised markets as well)

**Methods of Combat**

Most combat is performed by smaller craft 30-200m in length. Unlike factory/refinery ships, combat craft are very manoeuvrable. Both turret and fixed mount weapons are available, the latter being much more accurate and powerful. Factory ships have a few close range turret weapons, while the smaller fighting craft mainly use fixed mount weapons. The larger military ships may have some turret weapons for point defence purposes.

Anti-capship missiles and torpedoes may be intercepted by the smaller craft before they hit the factory ships. Laser and projectile weapons cannot be intercepted, although projectile weapons can be dodged by the faster craft.

Ships can be equipped with electronic suites to generate targeting noise, making it harder for enemy targeting computers to hit them. They also can be used to “fake” a larger ship but generating a signature of a larger/smaller vessel. This may fool enemies into attacking them instead of the factory ships.

The smaller ships will engage in a “dogfight” style combat. Several enemies will prioritise the factory ships as targets, using torpedoes and anti-capship missiles. Some harder enemies may even be equipped with artillery projectiles or long range laser weaponry.

Being hardish sci-fi, spacecraft will not have energy shields and must rely on armor and structure to protect them.

**Methods of Control**

Pilots create “Attack patterns” in a simulator and then assign these to their ships. These vary in effectiveness against different targets. Pilots select the orbit size, elongation, plane of elliptical, as well as speed, firing points and when to reload.

Pilots select a target and an attack pattern for each craft they are controlling. Certain patterns will be more effective against craft that are stationary, or perhaps more effective against an aggressive foe. The combination of craft fighting with different attack patterns should give the combats a very “dogfighting” feel.

These attack patterns are also designed by the game designers as AI routines for NPC craft.

Craft always complete their last pattern or order if the pilot disconnects or logs out. If a pilot disconnects while a ship is travelling at ~C Speeds, the ship will hang in space after completing its journey. The pilot can reconnect with this ship later to finish moving it around.

This is mainly so that a pilot who is controlling a group of craft can retreat one or more to drydock and simultaneously undock replacements, either directing them to fly to the combat zone, or from a local capital ship.

**Methods of Repair**

All ships can take a certain amount of combat damage. As the craft becomes more heavily damaged, its systems should become non functional. A ships ~C drive should stay online even when the ship is terribly damaged, however the drives top speed is severely reduced. This allows even crippled ships to retreat from combat.

Once a ship has been combat crippled, it will begin taking irreparable damage. This damage is accrued slowly, and each time more damage is taken at this level, there is a chance the C-Drive will explode, completely destroying the craft. Veteran craft that have seen many hard battles will eventually become retired from service due to this damage. If a craft reaches 0% integrity and doesn't suffer from a catastrophic drive failure, the ship will become a hulk (wreck).
