---
title: "Transmission Force Ideas"
source: "Game Stuff/Game Ideas/Transmission Force Ideas"
modified: 2015-07-27
type: planning
area: past-project
status: "prototyped"
projects: []
concepts: ["Transmission Force", "Design: Daily Seed and Leaderboards"]
words: 985
summary: "Development notes and roadmap for Transmission Force, a colour-matching lane/receiver arcade game: MVP release plan, scoreboard server, graphics phases, story, tutorial and bloat features."
tags: ["area/past-project", "type/planning"]
---

### 

### Thinking about TF again

I played again today. It is very addicting. New Minimum viable release idea.

- Daily seed

- Daily Scoreboard

- score upload

- Options menu: Score name, and upload scores checkbox

- Level change based on wave finishing

- levels become deterministic

### 

### Next Gameplay Phase

- level change bug fix: colorscale colors don’t match object colors

- local save of highest level

- resume from the start of any level up to the highest one you have beaten (always replay the last level you beat)

- no score, but highest level completed

- generate levels procedurally (limitless levels) based on the same seed (everyone plays the same levels)

### Next Graphics Phase

- lanes have background data to show which colors are coming up next, and those already in the lane

- break lanes into sections, each section only has one color deployed to it

- bumpers are invisible and animate a beam when catching

- bumper connects to same colored lanes and visibly cuts others

- sliders now show a muted low saturation version of color until pressed, then they glow

### Next Integration Phase

- BG score server

- gets sent an entry every time a player loses a level

- entry includes IP, platform, score, levels played and time elapsed

- returns a % of entries that failed this score

- stores local score info of your highest score

- updates your highest score % better than each time you send a new score

### Cool Quick Ideas

- guage in the middle to fill up

- road effect in bg

- objects follow a path down

### What needs to be done to make it saleable

- option to replay the same level of difficulty

- save game on quit, option to restart or continue

- perhaps save on quit, keep last three games

- ~~change points and goal to a bar that fills up~~

- scoreboard server and local high scores (displays which version you have)

- hyper modes (peak hour, color flip, ect)

- highscore just about which level you reached

- more interesting tempo variations

- ui graphics

- object graphics

- particle effects

- shorter levels but more intense

- autosave or start from a set level

- hardcore mode, start from start, play for highscore (infinite mode)

- infinite mode stores your score when you increase the progress bar, instead of changing level

- levels with different combinations of difficulty (loads of colors, loads of objects, speed variation)

- objects trace non-straight lines down before spawning

- bumpers are invisble and animate a beam when catching

- bumper connects to same colored lanes and visibly cuts others

- silders now show a muted low saturation version of color until pressed, then they glow

- objects with other colors come into the level but you dont lose score for letting them go past if you dont have that color

- start tut levels with one lane

- lanes can have a variable number of roads

- roads brighten as you catch objects on them, and dim slowly over time

&nbsp;

- 
- 

### Story

- In the year 3289 humans have spread across the known universe

- not just to different planets, but also to other dimensions

- taking capitalism and uncommon sense with them

- Transmission Force Inc is a corporation that specializes in multidimensional public transport and as an Expert Commute Router, it is your job to see that all these people make it home in a timely manner

- Why use humans to do this repetitive task?

- something about what happened last time with the Artificial Intelligences

- ...and Consumer Confidence

### Tutorial

- 23 Objects fall from the top of the screen inside the two lanes

- 24/25 touching/clicking on a lane will activate the bumper at the bottom

- 26 you get points for hitting Objects with the same colored bumper

- 27 you lose points for using the wrong color

- 28 when your score is high enough, you will progress to the next level

- 29 harder levels have more colors, objects and faster pacing

- 30 Objects will now come in 3 colors

### Maybe-Laters (new bloat minitasks)

- code rework: paddle placement based on lane direction

- autoscreenshot on game over

- save game after level victory

- removal of objects that have been destroyed

- code rework: runs with one or two lanes

- code rework: spawns happen over time, not all at once

- objects still falling outside lanes, must be fully inside lanes

### 

### Gameplay Summary

Transmission Objects falling from top and rising from bottom (or moving left and right)

slide finger on side of screen to change the color of the “receiver bar”

Transmission Objects have a color

If they collide with the receiver bar when the same color, you get points

Get enough points to unlock the next level

If they collide when the wrong color, lose points (but less than if you got it right)

Speed increases as progress is made

A few minutes per level

### Critical Objects

~~Resolution detection on load or 1024x768~~

~~Touch control~~

~~Gamestate Color Array - must handle more or less colors~~

~~Gamestate that can handle level transitions~~

~~Notifications of level change~~

~~Menu State with PLAY~~

~~Game Objects~~

- ~~receiver bar~~

- ~~transmission objects (velocity)~~

- ~~UI display (points, level goal, color picker bar)~~

~~Shape or sprite renderer(?)~~

~~Placeholder sounds~~

~~Placeholder graphics~~

~~Highscore screen displaying score for screenshot~~

### Bloat Features

Fancy Sound

Fancy Graphics

Multiple game modes (single direction, 4 way, up/down/left/right)

More colors in each level

Different colors on each side

Tweening graphics between colors

Capture juice animations

Procedural levels so gameplay is infinite

PEAK HOURS: speed and quantity of transmission objects changes slowly over time, but sometimes there is a rush in one direction
