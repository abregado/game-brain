---
title: "Notes - Game Architecture and Design"
source: "Game Stuff/Game Ideas/Notes - Game Architecture and Design"
modified: 2013-06-12
type: notes
area: design-theory
status: "idea"
projects: ["[[D&D Homebrew]]"]
concepts: ["Design: Game Design Process", "Design: Feature Classification", "Design: Gameplay and Fun"]
words: 1516
summary: "Study notes on game design process: architecture qualities, creativity/craft/technique, four-step creative process, five elements of drama, treatment analysis, core design, gameplay, features (integral vs chrome), rules, level design."
tags: ["area/design-theory", "project/d-d-homebrew", "type/notes"]
---

A good designer:

Makes his ego transparent in the game

Designs a game, not a movie with unlockable challenges

Rewards their players for FINISHING the game

Adventure game/plot/narative tips:

The MINIMUM paths through your game should be equal to a “choose your own adventure” book

General Game Tips

Original Gameplay allows you to be forgiven for minor geviences in PLOT

Game architecture

Modularity – Being able to modify, re-iterate sections without effecting everything else

Robustness – Crash proof design. Knowing how other members work

Reusablilty – Writing/designing for reuse

Trackability – Documentation and KPI

Gamplay Treatment - “vision document”. What it is like to play the game, what it feels like to play the game. More empashise of how it is to play rather than HOW TO play it.

Software Plan – Logical abstraction?

Technical design – how the code actually works

Three types of skill in creating

Creativity, Craft and Technique

Creativity is deciding on the idea (exceedingly rare, cannot be learnt but can be refined)

Craft is deciding how to do it (Rare talent, can be trained)

Technique is actally doing it (Common, can be trained, proceedural, no creativity)

In game deisgn you have instead (rarities like above)

Concept – CRITICAL to success

Structure

Design

Creative idea gestation period. Dont rush to write your idea down! (ive been doing this wrong)

Creative Process as described by 4 steps

Ignore Critical and Analytical opservations during the first three steps! “It is impossible to create ideas when you are concerned if they are good or not”

Inspiration – Conception

“Creative motherlodes are waiting to be mined. So start with a brainstorming session in

which anything goes. Leaf through a Victorian encyclopedia. Go to an opera. Browse

obscure sites on the Web. Watch a movie with subtitles. Sit in on a random lecture

at your local university. Go scuba diving in Florida or hill-walking in the Pyrenees.

The movie director, Ang Lee, draws inspiration from his sand and rock gardens. Do

anything that will help you get rid of the stale thinking. ”

Synthesis – combining ideas – Invention

Imporatnace placed not only on combining a number of ideas, but the correct ones AND in the correct ways. Cliches are born of combinations and assosciations. eg//: Vampires and Coffins, Camels and the Desert, Slapstick and Canes, Blue aliens and sex

Resonanace – Creating Synergy from ideas ???

Synergy is definded as making the whole woth more than the sum of its parts. The resonance step is designed to make maximum use of the idea combinations you have decided to use. Each idea should give something extra to each other idea. COMBO BONUS!

Convergence – Completing the idea

Subject your synergized idea to critique and analysis.

Review games that are even remotly like the one you have conceptualized. Were they good? Why/Why not?

This is the cusp between the Creativity step (Concept) and the Craft Step (Structure), and thus you must find out if your idea will hold together in the next step, without actually subjecting it to the processes therein.

Five Elements of Drama

Style

AKA genre. How broad is a genre? Fantasy/sci fi are broad and considered a genre (sometimes considered the same thing!)

Games seem to be defined by “genre” even tho the common labels are simply categories for their core mechanics (such as RTS, FPS, Strat, Sim, Educational).

Plot

Every game has a plot. Even if one is not included with the game. These are the stories that players tell each other about their in game experiences.

Character

The player s avatar is only one character in a game. Often this characters traits are not explicitly stated, instead they are implied via the options that the player is given. The example in the text book was the game Populous, where the player is a God. Some of the options the player has at his/her displosale are extremly evil, thus giving this god a lot of evil traits.

Another example would be the game Prototype where the main way the avatar regains health is by consuming innocent civilians. The player is given the option to consume innocents, although doesnt have to use this mechanic. The care-free animations of your avatar consuming an innocent give him a “anti-hero” feeling, however if the player never did this the feel of the character would change.

Setting

Every game has a setting. Internal consistancy is key here I feel. Once a player knows what to expected in the world, he can begin to feel at home. The example given in the text is Tetris, where the setting is the small box with strict rules governing how things interact. No metaphor is required as the player is quickly hooked and feels attached to the game world. Once they are attached they will not want to see harm come to this place (thus not wanting to lose!)

Theme

WRITE TREATMENT! Dont take technical limitations into account! Just write down all the things you think will be COOL!

Analysis of treatment

Ask yourself the following questions?

What genre is the game?

What will you do similarly to other titles of the same genre?

What Will you do differently?

In what specific ways are you doing things differently

Evaluate your treatment

How many Unique Selling Points do you have?

Are you doing enough things differently?

For each feature ask?

Is the feature Fun?

Has someone done this feature before?

If not, why?

Will the feature lead to good gameplay?

Technical difficulties to do with this feature?

Is it realistic to impliment?

Think about the controls for this feature alone.... Only so many buttons on a KB

Justification.

Once you have convinced yourself its a good concept, subject it to the client and team for debate. Be prepared to defend your concept!!!

FEASABILITY!

Does your idea have a market, target audience or commercial application that it will fill?

Is the technology needed for your game currently available?

As the iterative process begins, prepare for new challenges in feasability. Features calsh with eachother.

CORE DESIGN

What a game is no:

It is not a bunch of cool features.

It is not a intruging storyline

It is not fancy Graphics

It is not a series of Puzzles

Putting in cool features that detract from the gameplay is called GOLD PLATING

Puzzles are not GAMEPLAY, they are challenges/specific problems

Avoid using your game to tell a story or develop a universe. Frustrated Writer Syndrome

Gameplay is not as important as FUN. The first rule is “Is it FUN?”. Being considered a game is secondary to this.

Facebook games are less games and more Viral Marketting tools. If a FB game was designed as a Social Interaction then it may be more successful.

Can your needs for this game be better suited in another medium. Could it make a better movie or book, or boardgame? Computers generate Interactivity!

A Game has Gameplay.. so..

What is Gameplay?

Gameplay must make the player employ strategies of his devise to win. Winning can be defined as achieving a goal, one that you as the developer set.

If you have more than one goal make sure you have them interact, otherwise you are designing multiple games in paralell. My Example would be Mass Effect. The characters land on a planet and must drive on the surface. These levels are barely linked to the overall gameplay at all.

What are the goals?

How will the player achieve them (Tools)?

What will it be like to play?

Which key features, mechanics and conflicts will combine to create the gameplay?

GAME SPEC

Features

Each feature can be classified as either Integral (+), Chrome (+) or Gameplay Substitutes (-)

Each feature should be discussed as a single entity and how it will be implimented should not be discussed.

Feature based guidelines will (shold) endure the entire development cycle. The rules to make them happen will most likley not.

Gameplay

Here we need to explain how the features will generate gameplay, Consider the genre, and the intended features. Are there any combinations you can think of that will cause the gameplay to suffer? Is there too much for the player to consider at one time?

Think about each feature, is it Integral or Chrome? Integral features should not be ignored in order to fit more Chrome features in.

Your text should expliain to the devs how the game will work

This section will serve as a vision of how the game will be in the end, good to compare at several points throughout the dev cycle.

Interface

Rules

This section is all about writing the underlying rules of the gameplay/features. Here is where you should also be looking for emergent behavior. As the iterative process continues, the rules of the game will change drastically.

Level Design

Should enhance the inherent gameplay

Should never be used to cover bad inherent gameplay

Gameplay choices should be NON TRIVIAL, each choice and outcome should effect the end result. (Its seems to me that this still happens a lot in modern games)

Describe how the levels will enhance the inherent gameplay
