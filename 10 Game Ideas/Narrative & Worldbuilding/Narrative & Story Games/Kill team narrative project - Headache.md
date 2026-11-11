---
title: "Kill team narrative project - Headache"
source: "Game Stuff/Kill team narrative project_ Headache"
modified: 2026-11-06
type: design-doc
area: wargame
status: "designed"
projects: ["[[Narrative & Story Games]]", "[[Kill Team & 40k Homebrew]]"]
concepts: ["Kill Team Narrative Project", "Kill Team homebrew", "Design: Narrative Choice Systems"]
words: 2026
summary: "Design and technical spec for a Kill Team narrative campaign companion: Ink-style stories on a PWA dashboard with save slots, tabs (narrative, briefing, moments), JSON data format, tags and choices, plus campaign unit-count table and personal reflections on why it feels hard."
tags: ["area/wargame", "project/kill-team-40k-homebrew", "project/narrative-story-games", "type/design-doc"]
---

NB: each three mission campaign results in one new keyword being added to the campaign log. These do not necessarily do anything for now, but do change things if the missions are played in a different order.

Mission 1 and 2 of each series set keywords that are removed at the end of the series.

Campaign base rules

One player is the Protaganist Team

One player is the sidekick team

If a third player joins, they

| Team Size | Protagonist Team | Sidekick Team | Third player |
|-----------|------------------|---------------|--------------|
| 13        | 7 units          | 6 units       | 4 units      |
| 12        | 6 units          | 6 units       | 4 units      |
| 11        | 6 units          | 5 units       | 3 units      |
| 10        | 5 units          | 4 units       | 3 units      |
| 9         | 5 units          | 4 units       | 3 units      |
| 8         | 4 units          | 4 units       | 2 units      |
| 7         | 4 units          | 3 units       | 2 units      |
| 6         | 3 units          | 3 units       | 2 units      |
| 5         | 3 units          | 2 units       | 1 unit       |

Create your Kill Team as normal. Mark each unit on your campaign tracker.

Kill team narrative project

My issue is? Is this just harder than expected? Feels like it should be simple, or like im almost there. Maybe Im lying to myself.

Where do we put the choice?

Who is this for?

What is it:

Stories prepared in Ink language

**Visual novel style?**

**10 Tweet style**

Deployed via a PWA static site on your phone

Read offline once you start

3 missions long campaign for the conclusion of one story

Auto DM coop experience

Choices on board, not after or before

Victory does not matter, story deals with players losing

Choices affect the difficulty and game

Game affects the choices

Each campaign works with a set of teams and 1-2 boxes of enemies

Each mission is for 2 people in coop

“Split forces allocation” - split your force, one half plays this mission, the other plays that mission.

Attrition tracking: If a unit is taken out of action, it is no longer usable for the rest of the campaign turn. Leaders/Heros are the exception.

Formats

win/loss branching

Choice in mission 1 effects setup of mission 2. Choice in mission 1+2 effects setup of mission 3

3 missions, each with an effect on the final mission if not complete. Players can choose which ones to take on in first round. Remainder effect second round.

Presented in a thematic way

Product 1 and how it is used

User is presented with a menu to start a new campaign or load an ongoing campaign

New Campaign flow

Select Campaign from blurb cards

- Blurb cards also show which teams are supported

Select team (from blurb allowed teams)

Select protag name

Narrative briefing screen - also presented in Tab 0 later

Game screen mission 1

An interface with multiple tabs

- Tab0: Narrative briefing

- Tab1: Game Briefing (Setup and rules)

- **Tab2: Unit list**

- **Tab3: VTT**

- Tab4: Moments (containing narrative cards)

The game state is locked to the current scenario and only triggered to move on based on one of the Moments

The two bolded tabs above are not needed for the first iteration

We are making a dashboard to interact with a narrative experience. The dashboard must work on both desktop and mobile. On mobile we use a single scroll layout. On desktop we use a landscape layout. The project will use css, html and vanilla typescript in a way that the dashboard can be deployed as a Progressive web app. The site will be built and then hosted on github pages, where users can save it as a PWA. Build pipeline automation will use github actions.

The overall style of the project is grimdark, but easy to read. Additional styles are provided for various elements based on the story protagonist's team, or the severity of the current situation.

Interactive elements tend to be large card like buttons. Even on desktop, the interactive elements should be oversized.

A sample story with two briefing nodes should be created as well. This will have the following structure:

Two character choices, from two separate teams

One story node of intro text

One story node with a setup and a single choice with continueAfter

A briefing with several sections and two Moments

One moment with a two choices each adding different tags

One moment which gives a choice, and has continueAfter

Then two Story nodes, each with tagRequired based on the possible tags that can be acquired

Then a story node with continueAfter

A briefing with several sections and 4 moments

Three of the moments offer choices with teamRequired or tagRequried and give tags, and they all unlock the kurzel of the fourth moment

Fourth moment with startsVisible: false, which offers choices for each tag that could have been collected in the campaign, and continueAfter: true

Two Closing story nodes

**Main menu/Landing screen**

There are three save slots. If the slot has a game in progress, it shows the blurb card, and a button underneath to delete the save (with a confirmation dialog). If a save slot is empty, then it shows a plus sign and no delete button. Pressing the plus sign on one of the slots will move the user to the story select screen.

**Story select screen**

There is a back button and a carousel that shows blurb cards for each story in a horizontally scrollable list. Each card shows the story name, blurb and which teams are offered.The teams are collated from the list of characters in that story. Selecting a story card will cause a continue button to appear. Clicking this moves the user to the team selection screen.

**Team selection screen**

There is a back button and a card for each team that is playable. Each team card shows at the top a character’s name, then their role in a subtitle. At the bottom of the card is the team name. Selecting a card will cause two buttons to appear, Continue and Choose a Sidekick. Selecting the Choose a sidekick button will lock in the main card choice, cause the continue button to disappear and let the user select a second character card. After that one is selected, then the continue button reappears. Pressing back while selecting a sidekick will abort sidekick selection. Pressing continue moves the user to the intro screen.

**The intro screen**

This is actually just the Narrative tab (see below). Once the user makes a choice that has a continueAfter true, then the user is moved to the game screen with the briefing open.

**Game Screen.**

Has multiple tabs. The number of tabs must be modular because we might want to add tabs in the future. For now there are three tabs: Narrative, Briefing and Moments.

The Narrative tab shows story nodes in a vertical list, with the latest ones at the bottom. Tags that the user has collected are shown in a row at the top of the screen. The choices for nodes are made there.

Choice buttons are shown in a vertical list. They show the choice text and a subtext that says which tags are gained for choosing it. Once one is chosen, the unchosen ones are made invisible and the choices outcome text is shown. If there are no more nodes to be shown, and no briefing tab visible (which means also no moments) the user needs to go back to the main menu (see below)

The Briefing tab shows all briefing sections in order, either in a single column when in portrait view or mobile, or two columns, when in landscape mode on desktop. There are no interactable elements on this screen. A briefing tab is only shown after the user has reached the first continueAfter node, and the briefing tab is removed again after they reach the next continueAfter node. This means the state of the briefing tab can be determined on load based on how many continueAfter nodes have been visited.

The Moments tab displays all of the Moments from the current briefing node. These are displayed as cards, each with the moment kurzel in larger text, and the triggerText inside the card. Once a moment card has been clicked, it is disabled (greyed out) and the user is taken to the Narrative screen, where the story node from the moment is added to the history.

The game screen has the tab selection shown at the top of the screen, with the tabs collected on the left. On the right of this tab bar, there is a button to return to the main menu (with a dialog to confirm, that reminds the user that everything is saved after every story change). There should also be an undo button to remove the last story node added to the history.

**Save state and update**

Each time a Story node is added to the Narrative page, we should update the list of tags and moments unlocked, and the briefing tabs visibility based on the story history. The story history should then be saved to the local storage in its slot.

When loading a story from a slot, We should also recalculate the state of tags, moments and tabs.

Because we will save the entire history, we will need a container object for story nodes (storyNodeHistory?) that stores which choice was made, and if it came from a Moment. I’m not sure on the implementation of this, so give suggestions.

Loading a story that is complete should still work, and just bring the user to the game screen, on the narrative tab.

**Data format and Story organization**

We use a custom data format in json

Each story has a list of characters, each with a name, role, image link and team. We might need first name, last name and short role as well, as these will be used for string substitution in stories. Characters also have a sidekickOnly boolean.

Each story is made up of a number of nodes in a linear list

There are two types of node: briefing and story

Each story node is made up of one text block, a number of choices and a style class name (used for additional css styling)

Each node also has two fields onlyForTeam and onlyForTag, if either of these are set, then the node will be skipped unless the user has the correct team or tag.

A story node can have no choices.

Each choice is a string for its button (choiceText), a string that appears afterwards (outcomeText), a number of tags that are given when this choice is made, and a boolean as to if the story moves to the next node (continueAfter) after this choice is chosen. Each choice also has a field teamRequired, which if filled means this choice only appears if the players chooses a character with the given team. Each choice also has a tagRequired field, which means it only appears if the user has collected the correct tag.

Each briefing node has a number of sections, a name, a list of moments (see below) and a style class name (used for css styling)

There are several types of briefing section: text, image and table.

Each section has a string for a title, and a tagRequired string field which determines if it is shown. If it is blank then it is always shown.

Text sections have a string for a text block that is written in markdown

Image sections just have an image link

Tables have data for a table in json format

Each briefing also has a list of Moments

Each moment has a triggerText, a kurzel (alphanumeric) and a story node. Moments also have a boolean startsVisible as to if the moment can be seen at the start of the briefing. Each has a field “unlockedKurzels” which is a list of kurzel that become visible after this moment has been unlocked. Moments also have a style class name for additional css styling.
