---
title: "My Pi project"
source: "Game Stuff/Non-Game Ideas/My Pi project"
modified: 2016-01-10
type: notes
area: non-game
status: "unknown"
projects: ["[[Non-Game Projects]]", "[[Minecraft & Voxel Building]]"]
concepts: ["Raspberry Pi Notes", "Minecraft ideas"]
words: 170
summary: "Raspberry Pi command notes: setup, installing Cuberite Minecraft server and LOVE, plus a list of Minecraft server plugin ideas."
tags: ["area/non-game", "project/minecraft-voxel-building", "project/non-game-projects", "type/notes"]
---

opening terminal (ctrl-Alt-f4 type ‘lxterminal’)

sudo shutdown -Ph now

unplug replug (dont startx)

sudo raspi-config

type password

Expand Filesystem

Advanced-\>Hostname

startx

opening geany from terminal

choose a theme

shortcuts - alias mc=’minecraft-pi’

echo statement “drop the boss” - Welcome message

ls -1 (list no info)

ls -l

alt-f2 is run in LXDE

cat \[document\] \| less

sudo shutdown -Ph now

sudo apt-get update

sudo apt-get espeak

man espeak

cd /home

mkdir Cuberite

cd Cuberite

wget [*https://builds.cuberite.org/job/Cuberite%20Linux%20raspi-armhf%20Master/lastSuccessfulBuild/artifact/Cuberite.tar.gz*](https://builds.cuberite.org/job/Cuberite%20Linux%20raspi-armhf%20Master/lastSuccessfulBuild/artifact/Cuberite.tar.gz)

tar xf Cuberite

cd Server/

./Cuberite

LOVE install

sudo apt-get install libsdl2-dev

sudo apt-get install libopenal-dev

sudo apt-get install libmodplug-dev

sudo apt-get install libvorbis-dev

sudo apt-get install libtheora-dev

sudo apt-get install libphysfs-dev

sudo apt-get install libluajit-5.1-dev

Hunger on death plugin

Starting Items plugin

Ideas

Cooldown in Spectator mode on death

Detect Beacon and block combos

Class Inventory System (Warrior, Tank, Ranger, Firelord, any item set you can think of, Diver)

Bat Placement Item

Bat Detector

Build control - Placing Heads

Per player World borders

Chunk resource stacking score system

tp system

jail

Freeze

ORM
