---
title: "Factorio Tech progression"
source: "Game Stuff/Game Ideas/Factorio Tech progression"
modified: 2017-11-25
type: design-doc
area: game-idea
status: "designed"
projects: ["[[Factorio mods & ideas]]"]
concepts: ["Factorio mods / ideas", "Design: Tech Trees"]
words: 1740
summary: "Three iterations of a redesigned Factorio tech tree based on color science tiers plus activity nodes (power, vehicle, factory, robots, military), with tech-by-factory breakdown lists."
tags: ["area/game-idea", "project/factorio-mods-ideas", "type/design-doc"]
---

# 

# Tech Tree 1: Color Tier based, Linear

## Design Rules:

- The player choice should be to push “deeper” or “wider” into the tree

- Few, Large Tech Nodes (Expensive, time consuming, lots of contents)

- Bottles tiered like so: Red, Green, Black, Blue, Purple, Yellow, White

- Stick to existing tech costs and theme as much as possible

- Each tier should require all bottles of previous tiers.

## Tech Types

Technology Nodes are split into two types: Color Nodes and Activity Nodes.

Color Nodes unlock a new type of Science Pack (Bottle), and all the recipes/structures that are required to make it. Each Color Node requires the previous Color node to be researched.

Activity Nodes unlock a set of recipes to complete a particular Activity at a given tier (Color).

Activity Nodes are broken into categories based on what the Activity enhances. The categories are: Power, Vehicle, Factory, Robots, Military.

To be unlocked, Activity Nodes require that the previous level of that category be researched, and require bottles of a color one tier higher than the previous Activity Node in the same category.

Activity categories are linear and all Color Nodes are required.

##  

# Tech Tree 2: Color Tiered Based, Split Techs

## Design Rules:

- Large Techs based on Colored Tiers

- Player makes Choice based on intended next activity

- Each Color Tech dependant on previous Color Techs

- Each Activity Tech dependant on previous ones

- Each Activity Tech Level requires a new Color Tech to be unlocked

- High Tech and Production are separate

- Military Tech needs to be separate and optional

## Tech Types:

Technology Nodes are split into two types: Color Nodes and Activity Nodes.

Color Nodes unlock a new type of Science Pack (Bottle), and all the recipes/structures that are required to make it. The Blue Node requires the Green Node, the Purple and Yellow Nodes require the Blue Node, and the White Node requires both the Purple and Yellow Nodes. Colored Nodes require the bottles of the previous Color Node to research.

Activity Nodes unlock a set of recipes to complete a particular Activity at a given tier (Color).

Activity Nodes are broken into categories based on what the Activity enhances. The categories are: Power, Vehicle, Factory, Robots, Military.

To be unlocked, Activity Nodes require that the previous level of that category be researched, and require bottles of a color one tier higher than the previous Activity Node in the same category.

The Military Category Activity Nodes and the Black Color Node are all completely optional, as there is the possibility of players being in Peaceful Mode.

## Node Contents

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Starting Recipes:</p>
<ul>
<li><blockquote>
<p>Red Science</p>
</blockquote></li>
<li><blockquote>
<p>Wooden chests</p>
</blockquote></li>
<li><blockquote>
<p>Burner inserters</p>
</blockquote></li>
<li><blockquote>
<p>Electric poles</p>
</blockquote></li>
<li><blockquote>
<p>Iron axe</p>
</blockquote></li>
<li><blockquote>
<p>Stone furnace</p>
</blockquote></li>
<li><blockquote>
<p>Offshore pump (sans electronic circuits)</p>
</blockquote></li>
<li><blockquote>
<p>Burner miners</p>
</blockquote></li>
<li><blockquote>
<p>Lab</p>
</blockquote></li>
<li><blockquote>
<p>Boiler</p>
</blockquote></li>
<li><blockquote>
<p>Steam engine</p>
</blockquote></li>
<li><blockquote>
<p>Iron Stick</p>
</blockquote></li>
<li><blockquote>
<p>Cog</p>
</blockquote></li>
<li><blockquote>
<p>pipes</p>
</blockquote></li>
<li><blockquote>
<p>Wood Plates</p>
</blockquote></li>
<li><blockquote>
<p>Pistol</p>
</blockquote></li>
<li><blockquote>
<p>Magazines</p>
</blockquote></li>
<li><blockquote>
<p>Assembly Machine 1</p>
</blockquote></li>
<li><blockquote>
<p>Iron/Copper Plate</p>
</blockquote></li>
</ul></th>
<th><p>Blue Node:</p>
<ul>
<li><blockquote>
<p>Engine Units</p>
</blockquote></li>
<li><blockquote>
<p>Electric Miners</p>
</blockquote></li>
<li><blockquote>
<p>Plastic</p>
</blockquote></li>
<li><blockquote>
<p>Fluid tank</p>
</blockquote></li>
<li><blockquote>
<p>Advanced Circuits</p>
</blockquote></li>
<li><blockquote>
<p>Oil Refinery</p>
</blockquote></li>
<li><blockquote>
<p>Oil Derrick</p>
</blockquote></li>
<li><blockquote>
<p>Chem Plant</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Green Node:</p>
<ul>
<li><blockquote>
<p>Electronic Circuits</p>
</blockquote></li>
<li><blockquote>
<p>Assembly Machine 2</p>
</blockquote></li>
<li><blockquote>
<p>Wire</p>
</blockquote></li>
<li><blockquote>
<p>Green Packs</p>
</blockquote></li>
<li><blockquote>
<p>Transport Belts</p>
</blockquote></li>
<li><blockquote>
<p>Splitters</p>
</blockquote></li>
<li><blockquote>
<p>Repair packs</p>
</blockquote></li>
<li><blockquote>
<p>Undergrounds</p>
</blockquote></li>
<li><blockquote>
<p>Iron boxes</p>
</blockquote></li>
<li><blockquote>
<p>Inserters</p>
</blockquote></li>
</ul></th>
<th><p>White Node:</p>
<ul>
<li><blockquote>
<p>Rocket Fuel</p>
</blockquote></li>
<li><blockquote>
<p>Solid Fuel</p>
</blockquote></li>
<li><blockquote>
<p>Control Units</p>
</blockquote></li>
<li><blockquote>
<p>Low Density Structure</p>
</blockquote></li>
<li><blockquote>
<p>Satellite</p>
</blockquote></li>
<li><blockquote>
<p>Concrete</p>
</blockquote></li>
<li><blockquote>
<p>Solar Panels</p>
</blockquote></li>
<li><blockquote>
<p>Accumulators</p>
</blockquote></li>
<li><blockquote>
<p>Assembly Machine 3</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Black Node:</p>
<ul>
<li><blockquote>
<p>Piercing Rounds</p>
</blockquote></li>
<li><blockquote>
<p>Grenaes</p>
</blockquote></li>
<li><blockquote>
<p>Turrets</p>
</blockquote></li>
<li><blockquote>
<p>Steel</p>
</blockquote></li>
<li><blockquote>
<p>Assembly-machine-2</p>
</blockquote></li>
</ul></th>
<th><p>Purple Node:</p>
<ul>
<li><blockquote>
<p>Electric Engine Units</p>
</blockquote></li>
<li><blockquote>
<p>Electric Furnace</p>
</blockquote></li>
<li><blockquote>
<p>Stone Brick</p>
</blockquote></li>
<li><blockquote>
<p>Lubricant</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th></th>
<th><p>Yellow Node:</p>
<ul>
<li><blockquote>
<p>Battery</p>
</blockquote></li>
<li><blockquote>
<p>Processing Unit</p>
</blockquote></li>
<li><blockquote>
<p>Speed Module</p>
</blockquote></li>
<li><blockquote>
<p>Sulfur</p>
</blockquote></li>
<li><blockquote>
<p>Sulfuric Acid</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Power 1 - Requires Green Node</p>
<ul>
<li><blockquote>
<p>Solar</p>
</blockquote></li>
<li><blockquote>
<p>Pumpjack</p>
</blockquote></li>
<li><blockquote>
<p>Steel</p>
</blockquote></li>
<li><blockquote>
<p>Oil Refinery</p>
</blockquote></li>
<li><blockquote>
<p>Solid Fuel (Heavy and Light)</p>
</blockquote></li>
<li><blockquote>
<p>Large Poles</p>
</blockquote></li>
<li><blockquote>
<p>Circuit Stuff</p>
</blockquote></li>
</ul></th>
<th><p>Vehicle 1 - Requires Green Node</p>
<ul>
<li><blockquote>
<p>Train Stations</p>
</blockquote></li>
<li><blockquote>
<p>Signals</p>
</blockquote></li>
<li><blockquote>
<p>Engine Units</p>
</blockquote></li>
<li><blockquote>
<p>Train</p>
</blockquote></li>
<li><blockquote>
<p>Steel</p>
</blockquote></li>
<li><blockquote>
<p>Fluid/Cargo Wagon</p>
</blockquote></li>
<li><blockquote>
<p>Fluid Tank</p>
</blockquote></li>
<li><blockquote>
<p>Pump</p>
</blockquote></li>
<li><blockquote>
<p>Pumpjacks</p>
</blockquote></li>
<li><blockquote>
<p>Rails</p>
</blockquote></li>
<li><blockquote>
<p>Car</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Power 2 - Requires Blue Node</p>
<ul>
<li><blockquote>
<p>Nuclear Reactor</p>
</blockquote></li>
<li><blockquote>
<p>Centrafuge</p>
</blockquote></li>
<li><blockquote>
<p>Heat Exchanger</p>
</blockquote></li>
<li><blockquote>
<p>Heat Pipe</p>
</blockquote></li>
<li><blockquote>
<p>Medium Poles</p>
</blockquote></li>
<li><blockquote>
<p>Steam Turbine</p>
</blockquote></li>
<li><blockquote>
<p>Fuel Rod</p>
</blockquote></li>
<li><blockquote>
<p>Nuclear Processing</p>
</blockquote></li>
</ul></th>
<th><p>Vehicle 2 - Requires Blue Node</p>
<ul>
<li><blockquote>
<p>Tank</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +11%</p>
</blockquote></li>
<li><blockquote>
<p>Tank Shells Both</p>
</blockquote></li>
<li><blockquote>
<p>Explosives</p>
</blockquote></li>
<li><blockquote>
<p>Sulfur/Acid</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Power 3 - Requires Purple Node</p>
<ul>
<li><blockquote>
<p>Reprocessng Nuclear Fuel</p>
</blockquote></li>
<li><blockquote>
<p>Substations</p>
</blockquote></li>
<li><blockquote>
<p>Kovarex Process</p>
</blockquote></li>
<li><blockquote>
<p>Accumulators</p>
</blockquote></li>
</ul></th>
<th><p>Vehicle 3 - Requires Purple Node</p>
<ul>
<li><blockquote>
<p>Shells +50%</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +25%</p>
</blockquote></li>
<li><blockquote>
<p>Uranium Shells</p>
</blockquote></li>
<li><blockquote>
<p>Shells +115%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Power 4 - Requires White Node</p>
<ul>
<li><blockquote>
<p>Lab Efficency</p>
</blockquote></li>
</ul></th>
<th><p>Vehicle 4 - Requires White Node</p>
<ul>
<li><blockquote>
<p>Shells +75%</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +18%</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Factory 1 - Requires Green Node</p>
<ul>
<li><blockquote>
<p>Fast Belts/Splitters/Undergrounds</p>
</blockquote></li>
<li><blockquote>
<p>Long/Fast Inserters</p>
</blockquote></li>
<li><blockquote>
<p>Filter Inserters</p>
</blockquote></li>
<li><blockquote>
<p>Lamp</p>
</blockquote></li>
<li><blockquote>
<p>Steel Furnace</p>
</blockquote></li>
<li><blockquote>
<p>Stone Brick</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod +6%</p>
</blockquote></li>
</ul></th>
<th><p>Robots 1 - Requires Blue Node</p>
<ul>
<li><blockquote>
<p>+20 bonus</p>
</blockquote></li>
<li><blockquote>
<p>+45% bonus</p>
</blockquote></li>
<li><blockquote>
<p>Robot Frame</p>
</blockquote></li>
<li><blockquote>
<p>Construction Robots</p>
</blockquote></li>
<li><blockquote>
<p>Personal Robot Port</p>
</blockquote></li>
<li><blockquote>
<p>RoboPort</p>
</blockquote></li>
<li><blockquote>
<p>Battery/ Sulfur/ Acid</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Factory 2 - Requires Blue Node</p>
<ul>
<li><blockquote>
<p>Stack Inserter</p>
</blockquote></li>
<li><blockquote>
<p>Steel Pick</p>
</blockquote></li>
<li><blockquote>
<p>Stack Filter Inserter</p>
</blockquote></li>
<li><blockquote>
<p>Steel Chest</p>
</blockquote></li>
<li><blockquote>
<p>Landfill</p>
</blockquote></li>
<li><blockquote>
<p>Steel Drums/Canning Recipes</p>
</blockquote></li>
<li><blockquote>
<p>Level 1 Modules</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod + 8%</p>
</blockquote></li>
<li><blockquote>
<p>Concrete/Hazard</p>
</blockquote></li>
</ul></th>
<th><p>Robots 2 - Requires Yellow Node</p>
<ul>
<li><blockquote>
<p>Roboport 2</p>
</blockquote></li>
<li><blockquote>
<p>+10 bonux</p>
</blockquote></li>
<li><blockquote>
<p>+30%</p>
</blockquote></li>
<li><blockquote>
<p>Speed/Cargo/Count Increase</p>
</blockquote></li>
<li><blockquote>
<p>Logistic Robots</p>
</blockquote></li>
<li><blockquote>
<p>+10 bonus</p>
</blockquote></li>
<li><blockquote>
<p>+30% bonus</p>
</blockquote></li>
<li><blockquote>
<p>Steel Chest</p>
</blockquote></li>
<li><blockquote>
<p>Provider/Requester/Storage Chests</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Factory 3.1 - Requires Purple Node</p>
<ul>
<li><blockquote>
<p>Blue Belt/Underground/Splitters</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod +8%</p>
</blockquote></li>
<li><blockquote>
<p>Advanced Oil Prod + Cracking</p>
</blockquote></li>
</ul></th>
<th><p>Robots 3 - Requires White Node</p>
<ul>
<li><blockquote>
<p>+10 bonus</p>
</blockquote></li>
<li><blockquote>
<p>+30% carry/damage/speed</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Factory 4 - Requires White Node</p>
<ul>
<li><blockquote>
<p>Mining Prod +2%</p>
</blockquote></li>
</ul></th>
<th><p>Factory 3.2 - Requires Yellow Node</p>
<ul>
<li><blockquote>
<p>Level 2 Modules</p>
</blockquote></li>
<li><blockquote>
<p>Level 3 Modules</p>
</blockquote></li>
<li><blockquote>
<p>Beacon</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod +8%</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Military 1 - Requires Black Node</p>
<ul>
<li><blockquote>
<p>Steel Armor</p>
</blockquote></li>
<li><blockquote>
<p>Poison Capsule</p>
</blockquote></li>
<li><blockquote>
<p>Slowdown Capsule</p>
</blockquote></li>
<li><blockquote>
<p>Walls</p>
</blockquote></li>
<li><blockquote>
<p>Gates</p>
</blockquote></li>
<li><blockquote>
<p>Stone Brick</p>
</blockquote></li>
<li><blockquote>
<p>Submachine gun</p>
</blockquote></li>
<li><blockquote>
<p>Shotgun</p>
</blockquote></li>
<li><blockquote>
<p>Shotgun shells</p>
</blockquote></li>
<li><blockquote>
<p>Iron armor</p>
</blockquote></li>
</ul></th>
<th><p>Military 3 - Requires Yellow Node</p>
<ul>
<li><blockquote>
<p>Cluster Grenades</p>
</blockquote></li>
<li><blockquote>
<p>Uranium Rounds</p>
</blockquote></li>
<li><blockquote>
<p>Piercing Shotgun</p>
</blockquote></li>
<li><blockquote>
<p>Personal Laser Defence</p>
</blockquote></li>
<li><blockquote>
<p>Discharge Defence</p>
</blockquote></li>
<li><blockquote>
<p>Personal Shield 2</p>
</blockquote></li>
<li><blockquote>
<p>Power Armor</p>
</blockquote></li>
<li><blockquote>
<p>Personal Nuclear</p>
</blockquote></li>
<li><blockquote>
<p>Shooting Speed + 40%</p>
</blockquote></li>
<li><blockquote>
<p>Damage +40%</p>
</blockquote></li>
<li><blockquote>
<p>Atomic Bomb</p>
</blockquote></li>
<li><blockquote>
<p>Battery 2</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Military 2 - Requires Blue Node</p>
<ul>
<li><blockquote>
<p>Flamethrower + Turret</p>
</blockquote></li>
<li><blockquote>
<p>Flame Fuel</p>
</blockquote></li>
<li><blockquote>
<p>Combat Shotgun</p>
</blockquote></li>
<li><blockquote>
<p>Sulfur/ Acid</p>
</blockquote></li>
<li><blockquote>
<p>Laser Turrets</p>
</blockquote></li>
<li><blockquote>
<p>Explosives</p>
</blockquote></li>
<li><blockquote>
<p>Land Mines</p>
</blockquote></li>
<li><blockquote>
<p>Rocket Launcher</p>
</blockquote></li>
<li><blockquote>
<p>Rockets/Explosive Rockets</p>
</blockquote></li>
<li><blockquote>
<p>Modular Armor</p>
</blockquote></li>
<li><blockquote>
<p>Energy Shield</p>
</blockquote></li>
<li><blockquote>
<p>Personal Solar Panel</p>
</blockquote></li>
<li><blockquote>
<p>Night Vision</p>
</blockquote></li>
<li><blockquote>
<p>Shooting Speed + 30%</p>
</blockquote></li>
<li><blockquote>
<p>Battery/Battery Equipment</p>
</blockquote></li>
<li><blockquote>
<p>Damage +30%</p>
</blockquote></li>
</ul></th>
<th><p>Military 4 - Requires White Node</p>
<ul>
<li><blockquote>
<p>Shooting Speed + 30%</p>
</blockquote></li>
<li><blockquote>
<p>Damage +30%</p>
</blockquote></li>
<li><blockquote>
<p>Power Armor Mk 2</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

# Tech Tree 3: Activity Based Breakdown of TT2

## Design Rules:

- Break each Node of TT2 down into specific tasks, and Create new nodes based on those

- Keep existing Nodes as Structure for the Tree

- Make sure that there is no way to skip Color Nodes

#  

- Starter recipes

  - Red Science

  - Wooden chests

  - Burner inserters

  - Electric poles

  - Iron axe

  - Stone furnace

  - Offshore pump (sans electronic circuits)

  - Burner miners

  - Lab

  - Boiler

  - Steam engine

  - Iron Stick

  - Cog

  - pipes

  - Wood Plates

  - Pistol

  - Magazines

  - Assembly Machine 1

  - Iron/Copper Plate

- Build a Green Pack factory

  - Electronic Circuits

  - Assembly Machine 2

  - Wire

  - Green Packs

  - Transport Belts

  - Splitters

  - Repair packs

  - Undergrounds

  - Iron boxes

  - Inserters

- Build a Black Pack Factory

  - Piercing Rounds

  - Grenaes

  - Turrets

  - Steel

- Build a Blue Pack Factory

  - Engine Units

  - Electric Miners

  - Plastic

  - Fluid tank

  - Advanced Circuits

  - Oil Refinery

  - Oil Derrik

  - Chem Plant

- Build a Purple Pack Factory

  - Electric Engine Units

  - Electric Furnace

  - Stone Brick

  - Lubricant

- Build a Yellow Pack Factory

  - Battery

  - Processing Unit

  - Speed Module

  - Sulfur

  - Sulfuric Acid

- Build a Rocket Silo

  - Rocket Fuel

  - Solid Fuel

  - Control Units

  - Low Density Structure

  - Satellite

  - Concrete

  - Solar Panels

  - Accumulators

  - Assembly Machine 3

Robots Line

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><ul>
<li></li>
</ul></th>
</tr>
<tr class="odd">
<th></th>
</tr>
<tr class="header">
<th><ul>
<li></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Blue Level</p>
<ul>
<li><blockquote>
<p>Distractor Bots</p>
</blockquote></li>
<li><blockquote>
<p>+20 bonus</p>
</blockquote></li>
<li><blockquote>
<p>+45% bonus</p>
</blockquote></li>
<li><blockquote>
<p>Robot Frame</p>
</blockquote></li>
<li><blockquote>
<p>Construction Robots</p>
</blockquote></li>
<li><blockquote>
<p>Personal Robot Port</p>
</blockquote></li>
<li><blockquote>
<p>RoboPort</p>
</blockquote></li>
<li><blockquote>
<p>Battery/ Sulfur/ Acid</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Purple Level</p>
<ul>
<li></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Yellow Level</p>
<ul>
<li><blockquote>
<p>Roboport 2</p>
</blockquote></li>
<li><blockquote>
<p>+10 bonux</p>
</blockquote></li>
<li><blockquote>
<p>+30%</p>
</blockquote></li>
<li><blockquote>
<p>Speed/Cargo/Count Increase</p>
</blockquote></li>
<li><blockquote>
<p>Destroyer</p>
</blockquote></li>
<li><blockquote>
<p>Logistic Robots</p>
</blockquote></li>
<li><blockquote>
<p>+10 bonus</p>
</blockquote></li>
<li><blockquote>
<p>+30% bonus</p>
</blockquote></li>
<li><blockquote>
<p>Steel Chest</p>
</blockquote></li>
<li><blockquote>
<p>Provider/Requester/Storage Chests</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>White Level</p>
<ul>
<li><blockquote>
<p>+10 bonus</p>
</blockquote></li>
<li><blockquote>
<p>+30% carry/damage/speed</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

Weapons Line

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Weapons Red</p>
<ul>
<li></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Weapons Green</p>
<ul>
<li><blockquote>
<p>Submachine gun</p>
</blockquote></li>
<li><blockquote>
<p>Shotgun</p>
</blockquote></li>
<li><blockquote>
<p>Shotgun shells</p>
</blockquote></li>
<li><blockquote>
<p>Iron armor</p>
</blockquote></li>
<li><blockquote>
<p>Turrets</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Weapons Black</p>
<ul>
<li><blockquote>
<p>Steel Armor</p>
</blockquote></li>
<li><blockquote>
<p>Poison Capsule</p>
</blockquote></li>
<li><blockquote>
<p>Slowdown Capsule</p>
</blockquote></li>
<li><blockquote>
<p>Walls</p>
</blockquote></li>
<li><blockquote>
<p>Gates</p>
</blockquote></li>
<li><blockquote>
<p>Stone Brick</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Weapons Blue</p>
<ul>
<li><blockquote>
<p>Flamethrower + Turret</p>
</blockquote></li>
<li><blockquote>
<p>Flame Fuel</p>
</blockquote></li>
<li><blockquote>
<p>Combat Shotgun</p>
</blockquote></li>
<li><blockquote>
<p>Sulfur/ Acid</p>
</blockquote></li>
<li><blockquote>
<p>Laser Turrets</p>
</blockquote></li>
<li><blockquote>
<p>Explosives</p>
</blockquote></li>
<li><blockquote>
<p>Land Mines</p>
</blockquote></li>
<li><blockquote>
<p>Rocket Launcher</p>
</blockquote></li>
<li><blockquote>
<p>Rockets/Explosive Rockets</p>
</blockquote></li>
<li><blockquote>
<p>Modular Armor</p>
</blockquote></li>
<li><blockquote>
<p>Energy Shield</p>
</blockquote></li>
<li><blockquote>
<p>Personal Solar Panel</p>
</blockquote></li>
<li><blockquote>
<p>Night Vision</p>
</blockquote></li>
<li><blockquote>
<p>Shooting Speed + 30%</p>
</blockquote></li>
<li><blockquote>
<p>Battery/Battery Equipment</p>
</blockquote></li>
<li><blockquote>
<p>Damage +30%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Weapons Purple</p>
<ul>
<li><blockquote>
<p>Cluster Grenades</p>
</blockquote></li>
<li><blockquote>
<p>Shooting Speed + 30%</p>
</blockquote></li>
<li><blockquote>
<p>Uranium Rounds</p>
</blockquote></li>
<li><blockquote>
<p>Peircing Shotgun</p>
</blockquote></li>
<li><blockquote>
<p>Damage +30%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Weapons Yellow</p>
<ul>
<li><blockquote>
<p>Personal Laser Defence</p>
</blockquote></li>
<li><blockquote>
<p>Discharge Defence</p>
</blockquote></li>
<li><blockquote>
<p>Personal Shield 2</p>
</blockquote></li>
<li><blockquote>
<p>Power Armor</p>
</blockquote></li>
<li><blockquote>
<p>Personal Nuclear</p>
</blockquote></li>
<li><blockquote>
<p>Shooting Speed + 30%</p>
</blockquote></li>
<li><blockquote>
<p>Damage +30%</p>
</blockquote></li>
<li><blockquote>
<p>Atomic Bomb</p>
</blockquote></li>
<li><blockquote>
<p>Battery 2</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Weapons White</p>
<ul>
<li><blockquote>
<p>Shooting Speed + 30%</p>
</blockquote></li>
<li><blockquote>
<p>Damage +30%</p>
</blockquote></li>
<li><blockquote>
<p>Power Armor Mk 2</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

Production

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Production Red</th>
</tr>
<tr class="odd">
<th><p>Production Green</p>
<ul>
<li><blockquote>
<p>Fast Belts/Splitters/Undergrounds</p>
</blockquote></li>
<li><blockquote>
<p>Long/Fast Inserters</p>
</blockquote></li>
<li><blockquote>
<p>Filter Inserters</p>
</blockquote></li>
<li><blockquote>
<p>Lamp</p>
</blockquote></li>
<li><blockquote>
<p>Steel Furnace</p>
</blockquote></li>
<li><blockquote>
<p>Stone Brick</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod +6%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th>Prod Black</th>
</tr>
<tr class="odd">
<th><p>Prod Blue</p>
<ul>
<li><blockquote>
<p>Stack Inserter</p>
</blockquote></li>
<li><blockquote>
<p>Steel Pick</p>
</blockquote></li>
<li><blockquote>
<p>Stack Filter Inserter</p>
</blockquote></li>
<li><blockquote>
<p>Steel Chest</p>
</blockquote></li>
<li><blockquote>
<p>Landfill</p>
</blockquote></li>
<li><blockquote>
<p>Steel Drums/Canning Recipes</p>
</blockquote></li>
<li><blockquote>
<p>Level 1 Modules</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod + 8%</p>
</blockquote></li>
<li><blockquote>
<p>Concrete/Hazard</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Prod Purple</p>
<ul>
<li><blockquote>
<p>Blue Belt/Underground/Splitters</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod +8%</p>
</blockquote></li>
<li><blockquote>
<p>Advanced Oil Prod + Cracking</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Prod Yellow</p>
<ul>
<li><blockquote>
<p>Level 2 Modules</p>
</blockquote></li>
<li><blockquote>
<p>Level 3 Modules</p>
</blockquote></li>
<li><blockquote>
<p>Beacon</p>
</blockquote></li>
<li><blockquote>
<p>Mining Prod +8%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Prod White</p>
<ul>
<li><blockquote>
<p>Mining Prod +2%</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Vehicles Red</th>
</tr>
<tr class="odd">
<th><p>Veh Green</p>
<ul>
<li><blockquote>
<p>Train Stations</p>
</blockquote></li>
<li><blockquote>
<p>Signals</p>
</blockquote></li>
<li><blockquote>
<p>Engine Units</p>
</blockquote></li>
<li><blockquote>
<p>Train</p>
</blockquote></li>
<li><blockquote>
<p>Steel</p>
</blockquote></li>
<li><blockquote>
<p>Fluid/Cargo Wagon</p>
</blockquote></li>
<li><blockquote>
<p>Fluid Tank</p>
</blockquote></li>
<li><blockquote>
<p>Pump</p>
</blockquote></li>
<li><blockquote>
<p>Pumpjacks</p>
</blockquote></li>
<li><blockquote>
<p>Rails</p>
</blockquote></li>
<li><blockquote>
<p>Car</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th>Veh Black</th>
</tr>
<tr class="odd">
<th><p>Veh Blue</p>
<ul>
<li><blockquote>
<p>Tank</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +11%</p>
</blockquote></li>
<li><blockquote>
<p>Tank Shells Both</p>
</blockquote></li>
<li><blockquote>
<p>Explosives</p>
</blockquote></li>
<li><blockquote>
<p>Sulfur/Acid</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Veh Purple</p>
<ul>
<li><blockquote>
<p>Shells +50%</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +18%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Veh Yellow</p>
<ul>
<li><blockquote>
<p>Uranium Shells</p>
</blockquote></li>
<li><blockquote>
<p>Shells +75%</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +18%</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Veh White</p>
<ul>
<li><blockquote>
<p>Shells +75%</p>
</blockquote></li>
<li><blockquote>
<p>Trains Braking +18%</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>Power Red</th>
</tr>
<tr class="odd">
<th><p>Power Green</p>
<ul>
<li><blockquote>
<p>Solar</p>
</blockquote></li>
<li><blockquote>
<p>Pumpjack</p>
</blockquote></li>
<li><blockquote>
<p>Steel</p>
</blockquote></li>
<li><blockquote>
<p>Oil Refinery</p>
</blockquote></li>
<li><blockquote>
<p>Solid Fuel (Heavy and Light)</p>
</blockquote></li>
<li><blockquote>
<p>Large Poles</p>
</blockquote></li>
<li><blockquote>
<p>Circuit Stuff</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th>Power Black</th>
</tr>
<tr class="odd">
<th><p>Power Blue</p>
<ul>
<li><blockquote>
<p>Nuclear Reactor</p>
</blockquote></li>
<li><blockquote>
<p>Centrafuge</p>
</blockquote></li>
<li><blockquote>
<p>Heat Exchanger</p>
</blockquote></li>
<li><blockquote>
<p>Heat Pipe</p>
</blockquote></li>
<li><blockquote>
<p>Medium Poles</p>
</blockquote></li>
<li><blockquote>
<p>Steam Turbine</p>
</blockquote></li>
<li><blockquote>
<p>Fuel Rod</p>
</blockquote></li>
<li><blockquote>
<p>Nuclear Processing</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Power Purple</p>
<ul>
<li><blockquote>
<p>Reprocessng Nuclear Fuel</p>
</blockquote></li>
<li><blockquote>
<p>Substations</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="odd">
<th><p>Power Yellow</p>
<ul>
<li><blockquote>
<p>Kovarex Process</p>
</blockquote></li>
<li><blockquote>
<p>Accumulators</p>
</blockquote></li>
</ul></th>
</tr>
<tr class="header">
<th><p>Power White</p>
<ul>
<li><blockquote>
<p>Lab Efficency</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

- Build a red pack factory

  - Build a wall factory

  - Build an ammo factory

- Build an inserter factory

- Build a transport belt factory

- Build a green pack factory

  - Build a train station

  - Build concrete

  - Build solar

- Build a steel factory

  - Build peircing bullets

  - Build steel armor

  - Build grenades

- Build a black pack factory

- Build oil derricks

  - Build an oil station

- Build oil refinery

  - Build flamethrower

- Build plastic factory

  - Build an explosives factory

  - Build rocket factory

- Build advanced circuits

  - Build modular armor

  - Build robots

- Build assembly machines

- Build engines

- Build blue pack factory

  - Build tank cannon shells

  - Build tank

  - Build nuclear

- Build electronic furnace

- Build electric engines

  - Build robots

- Build assembly machines

- Build purple packs

  - Build better belts

- Build processing units

  - Build power armor

- Build modules

- Build batteries

  - Build accumulators

  - Build lasers

- Build yellow packs

  - Build beacons

- Build structure

- Build rocket fuel

- Build computers

- Build rocket silo

- Build satellite

  - Infinite research
