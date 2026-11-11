---
title: "Concept - Online Escape Room"
source: "Game Stuff/Game Ideas/Concept - Online Escape Room"
modified: 2020-06-06
type: planning
area: non-game
status: "designed"
projects: ["[[Narrative & Story Games]]", "[[Game Business & Funding]]"]
concepts: ["Online Escape Room", "Tomb of 4 Kings", "Game business & funding"]
words: 1323
summary: "Planning and design for a paid online multiplayer escape room: requirements, price/budget, mechanics, story formulas, puzzle types, and a detailed Tomb of 4 Kings puzzle set. Mentions Tom as interested partner."
tags: ["area/non-game", "project/game-business-funding", "project/narrative-story-games", "type/planning"]
---

Requirements

- Each client in a team gets a subset of the clues to find

- Can be completed by 1 client

- Clients see effects of other clients on their screens

- Time limit of 4 hours to complete the game

- Hints built in, availability by time

- 5euro per player, playtime of 1-2 hours.

- 10-14 puzzles

- Generic room structure

- Generic answer structure and mechanism

- Tom is interested in making this

- Ben is able to help with coding (Lapis?)

- Art budget of 200euro per room

- Theme agnostic

- Link to first page, and password, sent via email

- Connection to Stripe API for automatic sending of link emails

Nice to haves

- A way to get images from “free” locations, so we don’t pay for the bandwidth.

Mechanics ive seen so far:

- Email me to get the next clue (puzzle gives an email address)

- Call me to listen to a message (number is given directly)

- Type a code (numbers/letters) to progress to the next hyperlink

- Find something on google maps

Media types seen so far:

- Voice recordings as cutscenes between sections

- Still image/montage Videos with voice overs

- Still image clues

Other embeddables that can be used as clues

- Tables which can be sorted, and elements made invisible until there is only a few left

- [*https://www.vectary.com/3d-modeling-how-to/3D-web-embed-guide/*](https://www.vectary.com/3d-modeling-how-to/3D-web-embed-guide/)

- [*https://www.paperturn-view.com/paperturn-marketing/demo?pid=ODQ8487&p=13&v=2*](https://www.paperturn-view.com/paperturn-marketing/demo?pid=ODQ8487&p=13&v=2)

- Sliders which modify the css and reveal objects

- Godot games

Things to avoid

- Pixel hunting mechanics (just show which things are important)

Storylines/Formulas

Fixate on one each of item, place, person or conflict.

Skip to the start of the action. “You find yourself outside the dungeon, armed and ready”

Give two pieces of information about the item, place or person.

| Object   | Person              | Place               | Event                   |
|----------|---------------------|---------------------|-------------------------|
| shape    | Gender              | Temperature         | Where (town, country)   |
| Material | Cultural background | Activity associated | What                    |
| size     | job                 | Inside/Outside      | Why                     |
| purpose  | age                 |                     | Who                     |
|          |                     |                     | When (day, month, year) |

Each of these clues leads to one gate

The gate opens to reveal new information.

- A twist on one of the first two clues

- One of the clues is found to be false, therefore…

- A third clue which changes the context

Via mysterious circumstances you have the mcGuffin already and need to find the place to use it.

You find yourself in a place suddenly, the first room should give you some context as to what it is, but not why you are there.

An event is about to happen and you are on site to stop it.

Loop through three phases

1.  Finding

2.  Understanding

3.  Using

Each room has three of these cycles

Finding can be done without team interaction

Understanding might require communication

Using requires all players present

Finding can be reading the screen, rotating objects or moving obstacles. This only requires information and interaction from one player.

- Some objects are not findabale until another player does something.

Always give some items and clues as the game begins.

Understanding is solving a puzzle which opens something or makes something usable. This requires information from more than one player but only input from one.

Using can be as simple as each player clicks a button, wait until they have all clicked the button. This always requires all players.

Link instructions to character knowledge:

- Dr X was an avid reader of Y author

- Sergeant D was OCD so everything hasld to be in order.

- Nobleman J liked his bath at K degrees

Puzzles

Types

- dexterity/balance puzzle

- No thinking required/labyrinth

- mechanical/Try all combinations puzzle

- Translation puzzle

- Color matching puzzle

- Even distribution between points

- Ordered distribution in a scale (height/weight/ect)

- Correct rotation puzzle

- Complete the collection puzzle

- Odd one out puzzle

- Information collection puzzle

- Lookup 2 axis puzzle

A good puzzle can be half solved without any clues or with just one piece of the puzzle.

Story.

A god emperor died some 5000 years ago. We know that just before he died, he commanded that his 4 sons, at that time all kings of large lands, were to be buried in a tomb near his. The entrance to the Tomb of 4 Kings has been found and miraculously is in great condition even when it is 5000 years old. We need you to find a way into the tomb and locate where the God Emperor's tomb lies.

First visual show a lock

A non-interactive mechanism with 4 symbols and metal bars “locking” an obviously movable part. A mural with the 4 kings is on it.

**Puzzle 1**

Immediately completable

Information collection puzzle

Cypher required

Components: Several kings featured around the room, each has one symbol on their crown of an animal. The kings are shown on a mural where one is above the sky symbol and the others are below. There are several statues in the room. Each has a different animal head and on the plaque it has a cartouche inscription.

Input: Enter the answer in a 4 digit roller set. One roller is above the sky symbol, the other three below. Each has 5-6 different cartouches.

Effect: Unlocks one of the main door locks. Opens a new panel (puzzle 4) on a plinth in front of each statue and a tablet in the centre of the room.

**Puzzle 2**

Immediately completable

Math puzzle

Components: A large area of many symbols, but with some large groupings in the center. These show conversion between different amounts. 1 rope is worth 5 houses or something. There are 3 empty bowls in front, each with a symbol inside, and a bag of tokens.

Each statue is holding a bowl containing different counts of different items.

Input: The player must add up the total wealth in each kings bowl for each item, but only using the tokens they have.

Effect: One lock on the main door unlocks. The “worth” list moves, revealing a new set of worths for puzzle 3.

**Puzzle 3 - The weight of kings beneath the sky**

Evenly split the objects between three buckets

Values must be determined with a cypher

Components: A picture on the wall of several buildings, one of which is above the symbol of sky, the rest below. These building symbols also appear on the ownership registries under the statues.

Elsewhere a chart with each king and which buildings they represent.

Elsewhere a chart of building “worth”. These come from completing puzzle 2.

Input: 4 tokens stand on a holder. There are four bowls each with a building inscribed on it. The player places the tokens into the bowls and the correct combination opens the next part. One token should stay on the holder (the one above the sky), and two tokens should go in the same bowl.

Effect: Unlocks one lock on the main door.

**Puzzle 4**

Not visible until Puzzle 2 completed.

Components: Each of 8 moon phases is displayed on the floor as a carving. Along the radius lines, there are 10 markings with different symbols for each of the 8 moon phases, each symbol appearing in 4 different quadrants. Each statue shows a matching symbol on their scepter.

Puzzle 1 makes a tablet available, which shows which moon phase was more important to each king. This should allow players to figure out which symbol fits for each moon phase.

Input: The tablet shows 6 fields, each with a series of dots. The players must fill in the dots with lines to show the correct shapes as depicted by the floor diagram.

Puzzle 5

Requires part revealed after completing all others

Requires some information in the room that was not used in the previous 4 puzzles (revealed to be needed)

Rotation puzzle
