---
title: "Mattermost Communications for SS"
source: "Game Stuff/Game Ideas/Big Five/Survival Space Station/Mattermost Communications for SS"
modified: 2017-03-06
type: planning
area: game-idea
status: "idea"
projects: ["[[Survival Space Station]]", "[[Space Station 13-14|Space Station 13/14]]"]
concepts: ["Survival Space Station", "Space Station 13/14", "Design: In-Game Chat Integration"]
words: 384
summary: "Requirements list for using Mattermost as the in-game communications layer for a Space Station 13-style game: missing Mattermost features, game hooks, banned features, and special department channels."
tags: ["area/game-idea", "project/space-station-13/14", "project/survival-space-station", "type/planning"]
---

Survival Space Station Communication using Mattermost

Features Mattermost is currently Lacking

- Ability to join channel as invisible

- Ability to be view only to channel

- Ability to be post only as channel

- Ability to post as different people

- Flag a channel as ‘voice’ or ‘text’ (even though both are voice)

- Automatic setup and removal of channels

- Positional Chat

- Message timeout/fade (to emulate spoken channels)

- Backup final state for archive and public viewing

- Ability to have two channels open at once (i guess more browser windows would do it)

- Multiple api assignable tags for each player @science (all science people) @headofscience is the same as @johnsimpson (if the department head is called John Simpson)

Hooks that the game requires

- Post to channel at location

- Post to channel as

- Post random noise

- Connect player to channel

- Open private dialog to

- Create user

- Create channel

- Remove/create private link

- Reconfigure channels when changing headset

Hooks that Mattermost needs

- Check player location

- Check identity card

- Ability to secretly mute self in this channel

- Add another players tag for notification

- Clickable Links to show you where someone is

- Access player cosmetic information (so when you type it asks the game who you sound like)

- To check if you are connected (still needs to show you that the message was sent, but flag it as invisible)

- Check signal strength and language from game to garble messages.

- Send a direct message to the AI if a player tags another in a channel they cannot view.

Things that need to be be banned

- Free making of private message channels

When the Shift starts, users for each player should be created and a temp pass/username should be sent to that player.

Special channels

- Science

- Command

- Intercom

- Syndicate

- Alien

- Security

- Service

- Engineering

- Supply

- Medical

- Binary (AI/Robots)

- Department Heads

- OOC

- Adminhelp

Department Heads should also have a direct private line open to:

- the Head of Personnel

- Captain

- AI.

- Other Dept Heads

- All of their department members

- Service

AI should be free to open communications with anyone directly
