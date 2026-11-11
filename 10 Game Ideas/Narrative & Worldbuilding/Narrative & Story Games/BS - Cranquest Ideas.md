---
title: "BS - Cranquest Ideas"
source: "Game Stuff/Game Ideas/BS - Cranquest Ideas"
modified: 2022-04-09
type: design-doc
area: game-idea
status: "idea"
projects: ["[[Narrative & Story Games]]"]
concepts: ["Cranquest", "Design: Interactive Story Choices", "Design: Scrolling Text Effects"]
words: 682
summary: "Design notes for a short interactive story played by scrolling/cranking (Playdate-style crank), covering story themes, text presentation effects, choice philosophy and six alternative choice-implementation ideas."
tags: ["area/game-idea", "project/narrative-story-games", "type/design-doc"]
---

**Story Ideas**

- Themes?

  - Light hearted

  - Non-serious

  - fight/action scene

- Tropes

  - Lovable idiot wanderer

  - Recurring side character

  - multiple biomes

- Genres

  - Fantasy (portals)

  - Scifi (ships)

**Non-Bloat Features**

- Left.Right Choice box

- Scrolling text flat x5

  - Star wars text

  - Papyrus scroll (animated top and bottom)

  - Left right animated effect next to text

  - Left window image text scrolling on right (vice versa)

  - Parallax effect animations

  - Panicked in the dark effect

  - Old phone whatsapp convo style

  - Block text come-stay-go

- Animated gif forward/back when in centre of screen

**Player Choice philosophy and design**

- In a single short story of 6000 words.

- the player will be presented with an important, story changing, choice twice.

- Perhaps other choices can be added which do not affect the story. eg:// pronoun choice, character name, minor outcomes.

- No choice will be given at the end, the latest a choice can happen is midway through.

- There are no “failstates”, every path is a win of sorts.

- No flashbacks/forwards

**Other Choice ideas**

- Have the choices affect the world, not the character. Instead of “The character goes left”, instead say “The left path is blocked”

- The character should still make their own choices, just like in a book.

**Choice implementation ideas**

Each solution needs to solve meeting a choice “from the top” as is the case the first time, and “from the bottom” as when the player scrolls back from below.

**Idea 1**

Top: Player uses the left and right arrows to toggle the default choice “direction”. While scrolling down the choices are made automatically based on this setting, which can be changed at any time.

Bottom: By scrolling back up and then down again, while the setting is in the other direction, a choice can be changed.

Pro: Player can pre-choose a direction if they already know what they want to do

Con: Choices might become invisible, more UI requirements

**Idea 2**

Top: When reaching a choice, the player's scrolling stops until they press either the A or B button. Then this unlocks the scrolling to continue down that path.

Bottom: Scrolling back up is never blocked, but when the player scrolls back down, the scrolling is stopped at the choice like normal.

Pro: Makes choices more visible

**Idea 2.5**

Top: Choice blocks have a consistent graphical styling. Stop if the choice is “in neutral”. Once a gear is selected, you can continue cranking

Bottom: Scrolling past doesn't stop you. Scrolling back down doesn't stop you because the choice is already “in gear”.

**Idea 3**

Top: Choices require a button press, as in Idea 2

Bottom: Player cannot scroll up beyond their last choice. Starting again is the only way to change your mind.

Pro: Simple

Con: No going back removes options for play and also increases stress.

**Idea 4**

Top: As Idea 2 but after making a button selection, the crank increased a timer before continuing. The button choice can be changed at any time during this timer sequence.

Bottom: When scrolling up, the timer is not shown, so the player can scroll directly past.

Con: Timers are stressful

Pro: Makes choices more visible

**Idea 5**

Top: Choices are hidden when they are reached. The player must crank to reveal possible options and then crank back to the one they want. Use A and B iconography when a valid choice is available.

Bottom: Player cranks back to “start” of the choice sequence, then forward to reveal and select a choice.

Pro: More interactivity, more options for playful interactions.

Con: It might not be clear there is a choice to be made.

**Idea 6**

Top: As idea 5 but the choices cycle around. The player knows there is a choice because the two or three options keep repeating on the screen.

Bottom: When reaching the choice, the choices are displayed backwards once and then the text from before the choice begins to rewind.

Pro: More obvious you are in a choice sequence

Con: More complicated rewind logic.
