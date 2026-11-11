
A coop 4x game that utilizes a time paused phase where players read and take care of narrative events before playing a shorter 20-30 minute real time section. Short term goals for this session are set during the events, and the outcome of the events is based on which goals are accomplished.

A single game can take many of these rounds, and at the later end the game does become more of a survival game.

The game starts in a galaxy that is largely filled, similar to how Grand Strategy games begin, although the scope and focus of the game is far from a Grand Strategy.

The game design follows the rule of **"UX first"**. If a mechanic requires complicated, confusing or non-intuitive user actions, then it is dropped until a better UX can be designed. Sub-sub menus and right click menus that are 2+ levels deep are right out. MiddleMouseButton.OnClick() does not exist. Modifier keys are not the default solution. The only context sensitive buttons are left and right mouse click (not mouse hold).

The game design follows the rule of **"Coop first"**. It does not include any competitive or pseudo-competitive elements. it can be played in single player, but the experience is designed for 2+ players. 

The game design follows the rule of **"Get better friends"**. This means that the design does not protect players from griefers or trolls. You are free to play this game with randoms, but the target audience is a group of friends playing with each other in good faith.

This is a 4x so the design should address each of Exploit, Exterminate, Explore, Expand.

# Undecided design
Is there a win condition?
Is there a lose condition?

# Phases
## Event Phase
Players receive a list of events. There are two types of event shown here. Resolutions are the outcomes for the previous turns events, based on if the given goals were achieved. Opportunities are new events. Players can freely change their selection for any event during the phase. Effects are applied at the end of the phase once every player has ticked Ready.

Resolutions can have choices, but these are only used for giving the player the option to eject from an event chain. The bulk of these events are to show the imposed effects, and the calculation of numbers related to achieving the goal. The effect of resolution choices become active immediately after the Event Phase ends.

Opportunities always have choices. Each choice gives the player a goal to achieve by the end of the next turn. Choices may or may not have either a reward or penalty. 

*eg:// an event could give the player two goals to choose from, one easy and one hard. Neither has a reward for completion, but the easy goal has a larger penalty for failure.*

*eg:// an event could give the player two goals to choose from, one easy and one hard. The easy goal has a small prize for winning, and a penalty for failing, the hard goal has a much larger prize for winning, but a larger penalty for failing.*

### Committee
This is a coop game. During the Event Phase players will want to discuss some of their event choices. 

### Game state available
During the event phase, the player can view the state of the universe.

# Management Phase
Players complete a 20-30 minute session of real time gameplay in which they manage their empires. 

Gameplay is designed to be non-reactionary and certainly not reflex based.  

### Time flow
The speed of the game cannot be increase or decreased during this time. Players can individually set a "pause request" state, and if all players have this state on, the game is paused. Input is also paused during this time. The pause mode is designed for pausing play for RL interruptions, not for increasing thinking time or reducing cognitive load. These problems should be combated with good game design so it is not necessary to pause to make choices.

### Player agency
Choices that the player make during this part of the game are not instant. Instead, the player tweaks target values, and the values move toward the stated goal. This is relatively slow and has momentum. 

Momentum could be designed as either a penalty when you make a change, or a non-linear delta to reward players setting appropriate goldilocks targets, rather than micromanaging the values. The exact mechanic will need to be tested for intuitiveness and psychological effect.

### Cross empire effect
The important part of the game is managing the border regions you share with other players. Regions project effects onto neighboring regions, the effect being stronger the more different the two regions are. 

### Moving parts
But what does the player interact with and move around during the Management Phase?

**Assets**. These represent powerful objects or people. They can be "consumed" for a turn by an event. They can be stolen and traded between players.

**Fleet Power**. Ships are not controlled individually. Instead players set priority for deployment and they move around on their own. They are represented in a continuous, numerical way, rather than "X number of ships of type Y at location Z". Fleet combat is not the goal of the game, nor the focus. Fleet power is distributed amongst an empires Fronts.

**Blocks**. Colonies, planets, governments, organizations. These are grouped into regions. The combination of blocks in a region determine its impact on your empire. Some blocks are region locked. Others are movable.

**Research.** Each empire does its own research, in its own tree. Each empire also spends resources and time on disseminating technologies they have to other empires. 

**Surveying deep space**. The colonized systems are spread out and connected with fast travel, but the spaces inbetween are far from empty. Players need to search this deep space to find new systems to access. This should be an arduous process.

**Deciding focus**. Blocks and regions are marked with a claim state (claim/hold/abandon). Based on the combination of player claim states, Blocks and regions develop differently.

### Other things players will expect
I probably wont give any of these to the player, but I do need to find ways to have the other systems scratch the appropriate itches.

* Ship building, design, ect
* Fleet battles visible
* Mission based espionage
* Ground combat
* Colony building and building placement
* Population growth and management
* Colony ships

## Resources and values
One resource (Infrastructure?) is used for increasing the delta of change in your economy. The players should want to minimize this resource, as it cannot be stored, and is only needed while making changes to your economy. 

In general, I prefer resources that are not stored, although I think this is harder for players to quantify.

One resource must be kept in balance between all empires (Influence?). It represents the "galactic public opinion" of each empire. It is a fixed pool, and cannot be generated so much as traded slowly between players. An imbalance of this causes negative effects for all players, and may trigger events that cause damage to everyone. These events are a core of any failure spiral. Technologies might add or remove Influence from the global pool, making it more or less drastic to be a single point out of alignment with the others.

## Positional technology
Technologies, ability granters and unlocking objects should have a position on the map. Choosing where these go effects the spread of the ability, exactly how powerful the thing is, but also generate inflexibility in which regions and blocks can be easily traded between players.

*eg:// You research a new weapon technology and must place it on the map. This represents the factories, research labs or archives in which that technology is stored.* 

Losing that region means losing the technology. Its position effects which other empires get it first and the effort required to spread it. The type of place where you put it will effect its maximum effect and how quickly its effect is applied and built up.

*eg:// one system is nearer to the empire that is holding off the kraken invaders, so the weapon will be easier to spread to them, but there is another, more distant locations that contains a "pure crystals" tag that will double the effect of the weapon, in the long run.*

Perhaps a player cannot choose the exact location, instead they are presented with 2-5 locations and must select.

Regardless of the method of selecting, the player either needs to make this choice in the event phase, or it must not be important when during the management phase the technology is placed (only that it is).

# Pregame setup
## Role selection
There are a number of roles that must be taken by players. These provide specific actions that will be necessary for maintaining and completing the cooperative goals. Players can take an uneven amount of them, and it may be necessary to do so depending on the number of players.

Less complex games can be played where certain roles are left out. For example, if there is a role that manages the Space religion for the entire universe, and the player decide to leave that role out of their playthrough, then Space religion ceases to be a concern. In the same vein, if there is a role related to a galactic military crisis, then not using that role means that the crisis does not exist.

The requirements to complete the roles should all overlap. If defeating/holding off the galactic planet eater requires Metals, then another role (building a Dyson sphere senate) should also need this.

Thought: perhaps roles should come in pairs, or there should only be allowed sets. Maybe that there are easy and hard combinations is good.
## Main species selection
Each player selects a main species for their empire. This gives a set of strong bonuses, a set of events that can happen, probably some technologies, but also places restrictions on which roles they can take. The bonuses can be developed over the course of the game, via the events.

The combination of role restriction and economic bonuses gives the coop its punch and also increases replayability.

eg:// The S'sslark species is the best at building fleets, but they have a restriction that they can only have either the Combat Piracy role OR the Hold off the Darklings role, both which would benefit from the fleet bonus.
## Assumed alliances
It is assumed that the major powers of the universe are allied with each others. There are no direct player versus player actions. if the game has a victory condition, it requires all players to have achieved their role victory condition. If the game is a survival game, then if any player suffers its lose condition, then the game is lost.

## Early/Mid/late Game and Progression
The game requires a sense of progression, both in power level and in difficulty. What should not have progression is the complexity of gameplay. The type of gameplay can shift over the course of a single campaign, but the complexity should not