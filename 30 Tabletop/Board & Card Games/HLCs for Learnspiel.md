---
title: "HLCs for Learnspiel"
source: "Game Stuff/Game Ideas/HLCs for Learnspiel"
modified: 2015-10-30
type: pitch
area: past-project
status: "designed"
projects: ["[[Board & Card Games]]", "[[D&D Homebrew]]"]
concepts: ["Learnspiel", "Sales Technique Card Game", "Clerkport Game", "Babushka Game", "DelayedRewardTimetabler", "SalesWell", "Design: Bartle Types Features", "Design: Playtime Limiting"]
words: 6309
summary: "High-level concept and design summary for 'Learnspiel', a gamified e-learning ecosystem of four touch-screen minigames teaching mobile-shop sales techniques, with timing limits, persistence layer and Bartle-type features; detailed write-ups of minigames 1-3 and teasers for a 4th."
tags: ["area/past-project", "project/board-card-games", "project/d-d-homebrew", "type/pitch"]
---

# 

# High Level Concept - Whole Ecosystem

## Introduction 

This game is an interactive learning experience for employees of a mobile shop. The players will learn sales and merchandising techniques as well as company policy through a series of four mini-games. The game is also designed to me as undisruptive as possible while still being interesting to the staff members.

## Play Experience

John arrives at work on Monday morning. Every store has recently received a tablet with a new e-learning experience pre-loaded. Curious but not hopeful he loads up it to try it out.

After making a profile with this pseudonym John is presented with a choice of four minigames. Being more puzzle oriented he selects the 3rd game in which he must match customer needs to products.

As his playtime was uninterrupted he is done in just 4 minutes. The game displays his score as well as some reinforcement text as to the concepts he just utilized and how they can be used in real life as well.

Next the game displays a virtual shop, which is a representation of John's progress and learning. His playtime has also increased the quality of some elements. John is eager to try the other three minigames but sees a timer letting him know that this is not possible for a few hours.

He puts the game away as the first customer enters the store.

## 

##  

## Key Features

- **Integrated learning**: Learning is built into the game mechanics, rather than being layered on top. This increases the student's attentiveness.

- **Replayable:** Unlike with standard e-learning, the player will play each game many times. This increases retention of knowledge.

- **Visual Progress:** Students can always see how far they have come and recap on helpful tips.

- **Restricted Playtime:** Players can choose when to play but the game regulates how much they can play.

- **Undisruptive:** All parts of the game are designed to be pausable so that learning can take place during regular work hours.

## Artistic Theme

The game takes place in a radical pseudo-future where the player is selling his hightech communications solutions to the more primitive inhabitants of this planet.

## Platform

This game is designed for large format touch screen devices.

# Design Document Summary

Views:

- Profile Selection

  - Option to make a new profile

- Minigame Selection

- Virtual Shop Overview

- Minigame 1 (CustomerBuster)

- Minigame 2 (ShopDefence)

- Minigame 3

- Minigame 4

- Minigame results screen + Real World Tips

- RLW Tips, Collectables and Achievements Gallery

Technologies

- Instant Save states for each profile. When the player pauses it goes back to the Profile Selector, resume when selecting that profile

- Timing system. Maximum play time per day, Maximum play sessions per day, refilling these each day.

- 4 Minigames

- Persistent Layer with some sort of Power Creep mechanics

- Collectables and Achievement system

# Points to demonstrate in the Presentation

4 Minigames to begin with, expandable to more (n) that are linked together with a persistent layer, commonality of graphical theme and a unique timing system.

Gamification is used to increase student attentiveness and to reinforce the learning process through repetition

The educational content is built into the game mechanics, rather than built on top.

Features for Bartle Types

Achiever

- achievements

- star ratings

Explorer

- Collectables and categories for achievements

- first on device achievements

- achievements for min-maxing in a strange direction

Socializer

- visual login screen

- passive view sharing

- Seeing what others achieved

Killer

- “impossible” achievements

- first on device achievements

- ability to hide their progress from other non-super users

Match each mechanic to a lesson as requested

- Minigame 1: sales technique drilling - Technique Card Game

  - Sales Techniques and Phases

- Minigame 2: sales preparation situational awareness - Clerkport Game

  - situational awareness

  - Roles of Gurus and Team Leaders

- Minigame 3: customer-product matching - Babushka Game

  - Product-Customer Matching

  - Needs and Traits of customers

- Minigame 4: time-management - DelayedRewardScheduler Game

Explain how the Time limiting mechanic will work (coins per day), Giant pause buttons

Infinite Replayability and comparability (random seed generator)

Multi-session tutorial - building up the difficulty and complexity

Rewards: 3 star rating, Cosmetic Coins

Address problems they mentioned

- cheating during e-learning

- others?

Example games to pull credibility from

- Counting Kingdom

- Puzzlecraft

- Space Chem

- Tiny Tower

- Forest

- Habitrpg

- Papers, Please

Terminology

- Microlesson

- Ecosystem

- Learning platform

- 

Product Categories: Mobile, Tablet, PC, Zattoo

Where does traditional e-learning fail?

- Cheating

- Only do the content once

- Learn only enough to pass the exam

- Low retention, low user attention

What are we doing that is groundbreaking (Core Concepts)?

- Repeatable lessons, reusable content

- Integrates learning content into mechanics

- Microlessons displayed at the perfect time

- Complexity of solutions increases over many plays

- Designed as a learning platform so new content can be added easily

What we are doing due to fill requirements?

- Giant Pause buttons

- Play time control with game currency

- Gameplay and systems targeted at Bartle types

How do we motivate the player?

- Minigames have a higher density of fun!

- personalized aesthetic customization and virtual goods as rewards

- Achievements and Collectables

  - Collecting customer portraits

  - Informing the player when they break records or get new stuff

  - Inform the player when they are the first to reach an achievement

- Consistent visual style across minigames and persistence layer

# 

#  

# The Minigames

## Minigame 1: Sales technique Dialogue Card Game (WIP name)

### Introduction

This minigame is designed to have the player learn which sales techniques work in each of the 4 Phases of a Sale. This aim is achieved by giving the player a set of techniques at random which they must apply to the current customer to achieve a maximum score.

### Experience

As the game begins our player Jeff is shown a hand of 5 cards on the side of the screen, one of which is highlighted. This is the new ‘unique’ card for this playthrough. Reading through the description Jeff notes that this technique “Demo a Tablet” works best during Phase 2 of a sale and will help achieve a primary need of any customer looking for a Tablet product. Extra points can also be scored by using this on a customer at the end of any other sale to attempt an upsell.

The first customer is presented, filling one of the four slots in the middle of the screen. Jeff can see that this customer is Male, about 40 years old, wearing a suit and is carrying a Mobile Phone. Some additional information shows that the customer is in a hurry.

Knowing how to deal with Phase 1, Jeff immediately plays a Professional Greeting card on the customer. Its Super Effective! The customer is immediately upgraded to Phase 2. Perhaps Jeff will get to play is unique card earlier than expected...

### Features

- **Action Gameplay:** Sales is a fast paced adventure in real life, so why have it different in a game?

- **Real world ties:** Situations in this minigame are modelled directly on the real world and are therefore immediately applicable by the student.

- **Built in Tutorial:** By slowly releasing the number of technique cards into the ‘deck’ we can teach the player over several play sessions.

- **Expandable:** Content is easy to add. New company endorsed technique? Done! New customer archetype? Too Easy!

### Outcomes

The player will learn which techniques are important during each of the 4 Phases of Sales. Through repeated plays, all of which are similar but not identical, the player will learn much faster with a higher retention. Skills learnt in this minigame are also immediately applicable in the workplace. Other skills taught are how to Read Customers.

### Details

The interface shows 4 slots for customers, an area displaying 5 cards and a large pause button. At the start of each play session on this profile a new type of Technique card is added to the deck. This new type of card is always dealt to the player in the first hand. An information window is open is opened automatically at the start of the game to describe the new card (first time the player has seen it).

Once the player closes the information window gameplay begins.

The customer slots begin empty. Customers appear as front facing portraits with a series of statistical icons floating near their heads. To begin with they are greyed out until the player taps on them to “Greet” them.

If not Greeted, these customers will eventually leave the shop. Dealing with multiple customers at once is not necessary to succeed, but is the main way to get a high score.

Once Greeted, the customer will start to run out of Patience but his progress through the 4 Phases will also begin. Sometimes this means that a customer will reach Phase 4 without any player input, but it is not the aim of gameplay.

The player can at any time press on a card to see a detailed description of the card. This also pauses the game. Cards can be played on customers and will have a positive effect (as listed on the card) if played at the right time.

Once a customer runs out of Patience or reaches the end of Phase 4 (Bought something) they leave the shop. Some particles will pop out to show how much money they spent and a total cash number somewhere on the screen will go up.

Primary Gameplay is playing the Technique Cards on the right customers at the right time and cycling through as many customers as possible.

Once all 5 cards are used, 5 new cards are ‘drawn’ from the ‘deck’ randomly.

The game is over after 5 minutes, or a set amount of Customers.

##  

## Minigame 2: Sales planning and situational awareness

WHAT: Clerkport resource management game

WHY: Saying the right thing at the right time is important to sales, but understanding what is going on in your store and being attentive is even more important.

LEARNING OUTCOMES: Using time resources effectively, Dealing with Customers in an abstract way.

### Introduction

This game is designed to teach timing and preparation for peak sales periods. The player will control between 1 and 4 clerks and attempt to reach all customers before they become impatient and leave the game area.

### Experience

Another customer! Jill was right in the zone now. The field already had four customers waiting, with two others being dealt with by the Clerks. The two engaged Clerks were not very experienced so Jill kept having to swipe too and fro to keep the more experienced Guru moving back and forth between them.

Eager to capture some more of the new customers, Jill swiped for the Guru to greet one of them (a risky move!) and also signalled for one the of Clerks to try for a Close immediately, even tho the customer was not in Phase 4.

Another Customer appears and Jill then realises that the Guru will need to go on break any second now!

### Features

- **Intimate Controls**: The touch and swipe nature of this game means the player will feel more invested in the outcome.

- **Positional Puzzle:** Matching the right Clerk to the right Customer is only part of the game. The path they take to each other must also be calculated.

- **Cognitive Work:** The player needs to do non-trivial work to make trivial decisions, which means their retention of the subject matter will be more successful.

- **Pressure Flow:** To simulate a real shop environment the influx of customers will be dynamic over the 5 minutes of the game.

### Outcomes

The player will learn to deal with forecasted peaks and troughs of customer activity by planning ahead. Limited Clerks means making choices about how they can best be used. While this minigame does not teach how to deal with customers directly, it does teach how to deal with a multi-customer sales environment.

### Details

The player is first briefed on the situation. They can see a rough plan of the day including when staff members will be available, and the expected customer traffic over the 5 minute game session.

On the screen is also a large pause button and a “Sales Desk”. In this case the desk is in the middle of the screen.

Once the game is begun Customers start entering from the edges of the screen. They will move slowly toward to Sales desk, but will passively not touch it. The player can draw paths from his Clerks to destinations to get them to start moving.

Once a Clerk and a Customer touch, the Customer begins to get converted. This takes time. The player can move the Clerk away at any time but this stops the conversion process. If two Clerks touch without a Customer being involved then they become stuck for a very moments.

Over the course of the game the player must simply convert as many customers as possible.

There are a few special scenarios which may occur which require particular Clerks to solve, or that require a second Clerk for a few moments.

When a Clerk needs to go on break, they move automatically towards the Sales Desk and then become Greyed out for a period of time. When they need to go home, they move toward the edge of the screen and then disappear.

The customer types will follow the same pattern and format as those found in the first minigame.

## 

##  

## Minigame 3: Product-Customer Matching

WHAT: Babushka Game

WHY: Matching products to customer needs is important but the needs are rarely presented openly. The player should get several ‘turns’ to uncover what the customer is looking for. Then can never be 100% sure. If they take more time to understand the need there is a chance the customer will leave. They can select a product at any time.

LEARNING OUTCOMES: Relationships between customer traits, Choosing the right product

### Introduction

Simply asking students to remember complex relationships between customer needs and products is ineffectual. This game acts as a Mnemonic Bridge to help the student remember and to effectively build up all the required knowledge.

### Experience

She knew it!

Sally is just figured out the perfect product for the customer before her. Each of the customers needs were laid neatly in front of her, having been unpacked moments ago. Sally had already guessed which product was needed but wanted to be sure and so had taken extra time to uncover more information.

Adding the Mobile package to the pile she begins to repack all of the customer needs into the categories. In her rush to discover the problem, Sally realises she has forgotten how several of the pieces go back together. Was the “Impatient” trait taken out of the “Personality” box or the “Work life” box?

### Features

**Hands on:** This puzzle requires the player to arrange the parts themselves, and doing so strengthens the primary memory

**Direct with a Twist:** Standard matching games are ineffectual. This method takes a different approach.

**Abstract Visualization:** The complexity of the challenge increases over time. The player can always dig deeper for more information.

**Rewarding:** The patterns can sometimes be recognized with very little information. These “AHA!” moments are what we want the player to learn in real life.

### Outcomes

The player will not only learn which products are suitable for which customer needs, but will also learn to recognize triggers for various customer needs. Eventually the player will be able to grok requirements without searching very deep by training their intuition.

### Details

To begin with the player only sees a box shaped representation of a customer in the middle of the play area and to the side a scrollable list of products. Clicking the customer box “opens” it up to reveal several other items which could be customer traits, constraints or information.

These can be moved freely around the play area and when tapped will also open to reveal more components. Boxes with more components go about 4 layers deep. After every object is opened, there will be roughly 25 icons in the screen.

The player must learn which product fits with this customer. One product must be ticked as the primary product, and an additional product can also be ticked as an upsell.

Then all of the items must be recombined. The player can get this wrong, and will be awarded bonus points for recombining the items correctly. This mechanic provides an opportunity to do simple cognitive work immediately after making a product choice, and also an incentive to make a choice without opening all of the boxes.

Once the customer is repackaged, the player can drop the customer box in a hole labeled “Sale!” and they will receive a quick report to show how they went. Immediately another box will appear on the screen.

One star is awarded if the product was correctly selected, one if a suitable upsell was attempted and another if the customers needs were correctly repackaged.

##  

## Minigame 4: Expandable

We have any concepts that could be used for the fourth and future minigames. Just some short teasers are:

- **DelayedRewardTimetabler:** The player modifies staff timetables to cover the week. Projected customer rates and staff wellbeing change throughout the game to offer more challenges.

- **SalesWell:** Modify a board of pipes to fill customer needs. The most direct routes are also the least rewarding. Clever design is rewarded greatly.

- **SalesBlaster:** Blast objects with the right sales techniques in order to make them ready. Objects passing through the score area with the right preparation score highest!

- **ResourceCrisis:** Spend your 7 resources on solving store based problems. Staff come and go, bringing resources with them. Use what they bring wisely else they will take it all home with them.

- **MerchDefence:** Correctly arrange your merchandise so that customers survive to the end of a store-themed maze.

- **CustomerLane:** Deploy solutions in the right order to lanes to keep them clear and to maximize your score.

- **Screen Filler:** Given a field of obstacles, fill as much of the screen as possible with different colored squares while also matching your solution to a set of Customer Needs.

#  

# Persistence Layer (Virtual Shop)

Deal with power creep!

- ARG ITS STILL NOT DEALT WITH

Each Minigame gives different buffs? No they all give the same buff (coins)

Timing Currency… is it worth it?

How does this layer help the overall effectiveness?

- as a mechanic to increase player investment?

- to demonstrate how far the player has come?

- Ties everything together

- Gives value to player action

- Gives player something to check back on

- Shows progression of the player

- Holder for the timer mechanic (currency)

- Sink for the customization currency

Reward players who play often with more playtime so they are more invested in continuing to play consistently.

Components of the Persistence Layer

- Options for Customization

- Timer Currency

- Minigame Selection and Dynamic Cost

# Other Views and Concepts

Customer Trophy system and display

Minigame Victory screen (delivering microlessons)

- Microlessons

- three star scoring

- real world/game world tips

Profile Creation and Selection screen

Ecosystem Explanation

Theory behind getting the player to play again

Passive View mode

Maybes

- “regular customers” different for each profile

# ~~Requirements~~

~~To be played in an E-Plus store~~

~~Range of age 25-35 Mostly Men~~

~~Hop on Hop off. Short game loop, pausable game state~~

~~Reward structure not based on moving up hierarchy~~

~~Bartle Based content: demonstrate targeted content for each group~~

~~1-2 hours per week playtime (wow not much!) This is a hard limit and a mechanic to reinforce this needs to be designed.~~

~~1-5 minute sessions~ ? that is 24 sessions per week 5 per work day - distracting?~~

~~no social pressure to play~~

~~no penalty for not playing~~

~~Only one player concurrent player per store but many actual players~~

~~Play on a store level?~~

~~The game is loaded onto a company tablet (one per store)~~

~~fits into E-Plus culture.. what are these people interested in?~~

~~Graphically they are searching for a fantasy shop theme… this is not fixed~~

~~success driven reward structure~~

~~Use Mechanic-\>Lesson matching format~~

~~Good Mechanisms that were mentioned~~

- ~~show action: user to copy it~~

- ~~promote user to make choices himself~~

# 

#  

# From Process Doc

Examples of relationship guest host:

• Prepare the visit before, arranges the room and makes for a pleasant atmosphere

• welcomes the guest immediately upon occurrence, shows his joy

• Worries about the well-being of his guest

• Is interested in the guest, and listens to him

• is geared to the wishes and needs of the guest

• Try to offer the guest the best that he has

• Ask the host to an early follow-up visit

• accompanies the guest if possible farewell to the door

~~IDEA: Higher reward for the ‘+1” above the goal, lower rewards for +2,+3. Really add getting the +1 to the strategy.~~

~~IDEA: Rewards for ATTEMPTING +1s~~

~~Arrive, Care, Deal Close. Phased based gameplay where you cannot move forward without finishing the previous phase. Timer causes gameplay elements to drop out.~~

Links to Videosequenzen?

~~“kleine Führung durch den Shop” is part of the Sales process. Gameplay involving moving around to keep a timer from going down?~~

~~“Auf Informationen Bezug nehmen, die der Kunde in vorherigen Phasen genannt hat” Linking gameplay from previous phases… this could be interesting.~~

IDEA: Single use powerups are collected in earlier phases but can only be used later on. Incorrect use can cause a negative effect on the outcome.

“• Nicht fragen, ob, sondern was der Kunde möchte (A oder B)” also important to reinforce during this phase. Asking IF is ok earlier, but during later sales phases this is not an option.

~~Differing time costs for actions. Demonstrating a product and letting them do it themselves takes longer but has more effect. If the customer seems impatient but trusting then perhaps it's better to just describe the function.~~

Product Categories: Mobile, Tablet, PC, Zattoo

~~THEME: Your super space radical products are being brought to a city where everyone has old crapola steampunk tech. Reinforce in the game that your products are superior (abstracting away the subjectivity of that claim).~~

~~Reinforcing other subjective claims using gamer terminologies. Example:// New salespeople are often shy and meek, in the game give them a powerful title like Hero, Master, Giant.~~

~~SMART goals technique is included in their company policy~~

# 

#  

# Meeting 1 with Ali

~~Ideas decided on with Ali:~~

- ~~Profile Selection Screen showing incidental events but no highscores or anything~~

- ~~Persistent gameplay layer as shop which becomes better over time~~

- ~~Short length minigames which can be paused and apply bonuses to the persistent layer only after completion.~~

- ~~Radical near-future theme~~

- ~~Minigames played once per play session~~

- ~~Staff work 6 days a week.~~

- ~~5 minute play sessions~~

- ~~1-2 hours of play per work week means 12-24 play sessions~~

- ~~2-4 play sessions per day~~

- ~~some way to “check in” without being able to play after the player as used all this allocated time~~

- ~~collectables in the form of Customer Masteries. Use customer portraits as trophies. Collect them all by completing the content.~~

# Meeting 2 with Ali

- minigame choices finalized: Dialogue v2 cardgame, babushka, Clerkport, DelayedRewardScheduler

- need HLC for each game

- much more detail for minigame ideas

- Learning paragraph deployment using victory screen

- three star ratings for minigame performance

- ~~TowerDefence is out for now~~

- ~~Commonality of customer types and artistic style across all minigames and persistent layer~~

- ~~Persistant layer to feature personalized aethestic customization~~

- ~~Timing mechanisim to be abstracted to coins. Players pay for minigame plays~~

- Costs for minigames change to encourage even play

- Reward players for playing consistantly by allowing them to play up to 4 times per day

- Players who play more often can be more choosy about which games they play

- PCoins given get used to play games, games reward cosmetic coins which are used to buy cosmetic upgrades

- Door-Closing customization options. More personalization without being competitive

- Profile screen, Play with this profile or view

- Anyone can view other profiles persistent layer

Points about the presentation

- develop terminology and buzzwords

- Microlessons concept

- 

- show how and why we chose these options

- we are delivering a Platform that is scalable

- targeted gameplay for the learning outcomes

- focus on the team: Both core members are educators AND game designers

- screenshot mockups

- screenshots of example games. Sell on others successes

- 

# 

#  

# Brainstorming Ideas

~~Is this a game that the students want to play (or cant they) after finishing the content?~~

~~What is the run-time of the project?~~

~~Do we have access to some sample lesson content ?~~

~~Abstract Choices~~

- ~~Make a fun game they want to interact with and then lay the learning on top~~

- ~~Weave the learning into the game content and mechanics~~

- ~~Have the game mechanics represent the learning content but not directly~~

~~input based on work conditions~~

~~encourage data collection (customers entering store, unterhaltungszeit)~~

~~link playtime to work schedule (play before you go for lunch, when you arrive at work)~~

~~2 hours per player or 2 hours per store?~~

~~social peer group umpiring? To combat previous cheating~~

~~Real world metrics?~~

~~one ‘umpiring’ player per day who enters the data from everyone? this role rotates?~~

~~Registration of players in shop by manager - team games?~~

~~Links to real work situations (Thematic)~~

~~Building up, persistence? Just of rewards or also of gamestate?~~

~~Competitive gameplay against other members?~~

~~Nimblebit tiny towers~~

~~Radical Realism~~

~~Product information~~

~~Passive “store income” based on persistent layer~~

~~Players better or change the persistent layer by playing minigames~~

~~My own ideas:~~

~~On Profile Page display number of logins this week/day and number of minutes remaining. We can give these over time to make sure that players always have some per day by ‘releasing’ play sessions over the week. This is similar to ‘tick’ based games but much less granular.~~

~~Make the gameplay teach the content. Focus on the Sales process highlighted in the first document.~~

~~Come up with 2 minigames to cover this content (4 Phase sale system, after sales assistance)~~

~~2 minigames to deal with store presentation (inside and outside)~~

~~Focus on second-second gameplay of other reflex story games like 5 Nights at Freddies for the sales oriented games. Selling is emotional and action/reflex based.~~

~~Focus on slower paced thinking and puzzle elements for the presentation games. Merchandising is strategy based.~~

Pause buttons should be very large and always available.

Force players to select one of the 4 minigames each time they have a play session. They cannot improve everything in one play session. This adds value to all decisions and also lets the player decide what is more important.

~~Each minigame should be important to the persistent layer but they do not need to be equally important.~~

Persistent layer needs some basic economy that scales over time. In this areas power creep must be dealt with in the design. Solutions:

- Store “moves” to new location with more difficult customers, layout stays same (scaling difficulty)

- Store state resets. You get promoted to a new store which is doing poorly (state reset)

- Increasing one part of the store reduces another part or introduced harder events (tug of war)

- state is forever decaying so the player needs to upkeep. Decay increases until it balances growth (diminishing returns to asymptote)

~~Experience points could be called Executive Credibility (as per training document). Once you reach a hurdle you get a promotion. Maybe Cred drops over time. Perhaps increase if increasing the points you need, at higher levels your Cred goes down faster (Executive Expectations).~~

~~What are the DESIGN GOALS of the game?~~

- ~~students learn x after y times playing?~~

- ~~‘improved uptake’ in new staff. How to measure?~~

- ~~just a better way to deliver the new content?~~

- ~~staff need to have fun at work?~~

~~What are the Design Axioms (things that should be set from the start and never change) ?~~

~~Minigame Ideas (try to use intuitive and already proven games):~~

**Abstract block shooting game**: As discussed. Use associative language to link abstract gameplay to real world processes. The 4 phase system is perfect for this as “customers” must be moved through the phases linearly.

**Match 3 style puzzle:** Making associations is just as important to sales. A match 3 puzzle board for each customer could work. Ali and I both have experience in grid based puzzle mechanics. Match a untrusting customer with a trust increasing technique and the right product to “match3’. Perhaps new customers appear and need to be matched to a Greeting before you know what type they are. Maximum number of ‘open’ customers based on staff levels. If there are ungreeted customers you need to close one of your open customers to greet them.

~~**Dialogue game:** This one is awesome but actually A LOT of work. Developing content for this minigame will be a full time just in its own right. This would need a decent set of mechanics, the dialogue system itself AND a buttload of content.~~

**Labyrinth game:** Draw a path through a maze over a few turns. Getting to the exit (a sale) is pretty easy, but being more careful on the way will yield more score (exploring and reading your customer). As it is turnbased the default state is paused. It doesn’t fit well with sales as face-face sales is more about the second-second reflex gameplay.

**Resource Conversion minigame:** Join items to make new ones in the correct ratios to score the most points with the same starting conditions. Starting conditions are based on persistent layer. Items can be combined in several ways (crucibles with verbs). Different items in different crucibles results in a lot of combinations.

**EventTextBox series.** Use RNG to create a miniseries of events in which the player needs to make a choice. FTL, Curious Expedition or King of Dragon Pass events as an example. Player can see the name of the upcoming events to try and be ready for them. Content is highly linked to teaching content. Benefit here is that new content can be added easily as it is text based.

~~**Slots and Tanks:** There are a number of slots available. You can place a tank in a slot and start to fill it with the same color liquid or gems. There are more colors than slots. Player needs to decide when to score or tip out tanks to start new ones. Potion Brewing theme? How to show going on break?~~

~~**Box Opening:** The player is presented with a box. When opened there are a number of objects inside. These objects can be reacted in various places. The player has a limited number of moves to replace a faulty part and then return all the items to the box.~~

**Walls and Barriers:** Each encounter involves using the correct weapons to break down walls to reveal an inner core. Along the way you reveal information about the core and then must make a choice about which weapon to use to score the most points.

**Tower Defence:** Place objects in your store and then watch as customers come in. Will you convert them all or will they leave unhappy. Signage, Product placement and staff positioning come into play. Abstract to something else maybe. Tower Defence games are really specific.

**Cook Serve Sell:** Limited positions for customers (number of staff). Passive customers wait in a queue until they get angry and leave. Give them what they want ASAP to free up staff to access more customers.

**Cook Serve Sell (Quiz/Match):** Similar to above but turn based. Each turn you can ask one question to your customer. Each customer will only tolerate so many questions. Once you know which service they need you match them to it and then you get a score at the end of 3-5 customers.

**SalesWell:** Oilwell style “pipes on tiles” game where you can only rotate tiles to make a connection between the customer and their needs. Once a connection is made then the pipes start filling regardless if you are finished or optimized.

**Just Select:** A wide range of different pieces on the screen. Just connect them together or even just select the correct ones and press “Try solution”. Solutions can be hidden and then traded to other players using the patented “Real World Interface - Mouth and Ears”. New combinations can be added to the game over time without alerting the players.

**OnceturnPACMAN:** A pacman maze is on the screen. There are a number of different obstacles and items available. You can draw a path through the maze to collect items but you can never cross your own path. Players choose which items to collect as they cannot collect them all. Each ‘turn’ the maze is regenerated and randomized. Players collect points into 4+ fields but only get points based on thresholds to promote different choices.

**Find the Order:** Place pieces of a puzzle in the correct order (use Phases from the Sales Policy) to generate strong combos. There are negative pieces and counters for them, you get extra points for adding in negative pieces if you counter them properly. Chain length is rewarded well, but short chains can be considered ‘successful’ but reward minimally. The pieces are shuffled and regenerated when you collect a chain. New pieces can be added in over time. See Thurn and Taxis and other deck/combination building games.

**TeamTimeUnits:** Crew management game. Time Budgeting for several team members. Sales and trading oriented. Game events reflect real world scenarios. Positive in game effects are associated with positive real word actions.

**LoginHighscore(Feature):** Login screen look and feel: Initial screen shows all player accounts in avatar form. Use simple mobile unlocking for passcodes (libraries available I’m sure). All players play from one tablet. Countdowns on characters that are unplayable right now. PlayTime management of both number of logins per week and number of minutes spent in game. This can also be used for a high score screen, as everyone sees it before they log in.

**DialogueEventer:** Event management game like King of Dragon Pass. Random events are the main driving force in the game. Players make a series of choices during one event. During each login a player must deal with one event, then can ‘play’ in the main game a bit. These events can be focused on delivering the learning content.

**LearningActionPuzzler:** An Action puzzle game where the player needs to complete actions to convert opportunities into score. The actions in game and game objects are named after different concepts that the staffer should be using in the store. When loading the game each time there is a short description of how these techniques actually affect their work. The game object names are simply helping the player remember the concept names.

*Example: Blocks appear on the screen and have a countdown timer on them. The player can tap to rotate them. Each side of the block shape has a Need. On the sides of the screen are a number of effectors which can be activated. These fill needs if activated at the right time, and if the blocks are rotated correctly. The Needs are named after steps in a sales process (based on company policy).*

**CollectionTrader:** The players receive a virtual box filled with random items each time they log in to the game. These can be combined to create different items and then sold to each other or on a global marketplace. Each time a box is opened the learning content is delivered in mini-exams. Correct answers mean the player gets a bonus to the value of the items in their box. Items can be named after concepts the company policy wants to reinforce and the combinations can be representative of company procedures.

~~**VirtualCustomer:** We model a random customer generator. The player must uncover the customer's needs and then try to convert them into a paying customer. Time limits represented by customer patience. Mistakes or heavy handed selling at the wrong time increase distrust, and frustration. Basically give the players more practice iterations than there are real customers. Use photos of attractive people to incentivise play (haha).~~

**ItemHunter:** Simple Item hunter game. Word match -\> Image. Reinforces correlations

## Non-Minigame Stuff

**Collection Mechanic (Customer Faces)**

# Persistance Layer Ideas

Power Creep: how to deal with it?

# Goals. What Do WE want to player to do?

The player should want to use the game

The game should allow the player to demonstrate the knowledge in the learning sessions

The game should strengthen the memory of the sales procedure

Active and Passive layers to represent the store appearance and the players own work

The player can “check back” on his passive progress after running out of time

Repeating blocks of text kept to a minimum.

The player should play though one of the minigames during each play session.

The player should choose which minigame to play

The player should want to play all minigames, even if one is more fun for them.

# How do we prove the player is learning?

The minigames become harder over time?

Sometimes there will be a boss level in each minigame which is very difficult to overcome without the correct knowledge.
