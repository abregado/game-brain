---
title: "HLC+ - Kitchen Stocktake App"
source: "Game Stuff/Non-Game Ideas/HLC+ - Kitchen Stocktake App"
modified: 2021-11-10
type: design-doc
area: non-game
status: "designed"
projects: ["[[Non-Game Projects]]"]
concepts: ["Kitchen Stocktake App", "Design: Recipe Driven Critical Stock"]
words: 1078
summary: "Detailed design doc for a phone app that tracks kitchen stock by location and reorders the shopping list by supermarket layout, with expansions (recipes, prices, multi-shop, tipping, sync)."
tags: ["area/non-game", "project/non-game-projects", "type/design-doc"]
---

## Define the Problem

Before I go shopping I take a piece of paper, go to each storage location in my kitchen, and make notes of the levels of each item. Anything that is empty goes on the list. The first problem is that empty items are simply not detectable, since empty space is invisible. If there is an empty space reserved for something, sometimes I don’t know what lives in that space.

The second problem is that after I have made my list and go to the shop, the order of the items does not match the order in which they appear in the supermarket. This often leads to me forgetting to buy an item, or zig zagging across the supermarket.

Enter the “Use my phone as a list that changes its order” app.

## Goals and Metrics

Simple to develop (Ben is a noob)

User has total stock of their kitchen while at the supermarket

Stocktake is simpler and more complete

Missing items can be seen during Stocktake

When shopping, list items are less seldom forgotten

Data is stored on the device

## Business logic

Go to kitchen -\> take stock at each location -\> go to supermarket -\> view list of discrepancies by supermarket location -\> tick objects as they are added to trolley -\> come home

## Technology

Ionic or Flutter? The inventory data does not need to be stored online. Preferably everything runs locally on a single device.

##  

## Screens

**View all items screen**

All positions are listed, with kitchen position, supermarket position.

Long press on an item opens the item edit screen.

**Stocktake screen**

All items are listed.

Items are sorted by location, then by position in location.

Button at top to “finish stocktake”. This updates all the item states.

List is broken up by headings of the kitchen positions

An add item here button is at the bottom of each kitchen position area.

Stock Level button/Indicator

- Each item has a button with three states, showing stock level

- Levels represent empty, partial and full

- State shown with three circles

- Pressing the button changes the future state, shown by a ring around the circle

Stock item name

- Long pressing on the name toggles the item between critical and non critical.

- Non-critical items are greyed out but can still have their stock level changed

**Shopping screen**

Critical Items with less than full status are listed here

Items are listed in Supermarket position order

The list is broken up with headers of the supermarket position

Each item has a checkbox, which marks it as purchased

Long pressing an item allows you to change its position in the list (in case you find the order is wrong)

Finish Shopping button

- Updates item states

- At top of list so it cant be accidentally clicked

**Edit position/item screen**

Name

Stock level (three circles)

Dropdown for kitchen and supermarket position

Number field for index inside that position

Critical item toggle

**Settings screen**

Set all stocks to zero button (with confirmation dialog)

Kitchen and Supermarket area editing

- Buttons to delete, and add new areas

##  

## Expansion ideas

### Handle Multiple shopping/house locations

Items to support multiple Supermarket Locations.

Stocktake tab now has no list, but instead two buttons

- “Start stocktake”, which opens a dialog for the user to select a house area.

- “I’m planning to go to”, which opens a dialog for the user to select a shop.

Stocktake list then shows items which have a shop position for that shop.

Shopping tab now has a button “Start shopping” which opens a dialog for the user to select the shop they are at.

Shopping list only shows items which have positions in that shop.

Settings area editing can add new shops.

New shops have a default “Unknown” location.

Shop areas can be ordered but default to the same index.

House container for different areas. Kitchen becomes child of this.

New house areas can be

### Recipes

New data entity, Recipe

New screen: Recipe list/Critical stock

A recipe contains a list of Ingredients which are required.

Each Ingredient contains a list of items which would fulfil it

Item Critical status is determined by which enabled recipes are in the recipe list.

**Recipe list screen**

Shows each recipe, with expansion option to see ingredients

Button on each to activate/deactivate it

Long press to edit a recipe

Recipes which are fulfilled are highlighted green.

### Price data

Each item has a list of recent prices

The average of these is shown next to the item in the shopping screen

When finalizing a shopping screen, the user is asked if they wish to enter pricing information. Clicking this begins the quickfire screen

**Enter price data quickfire screen**

Shows one item, and asks for you to type in a value. Pressing enter moves to the next item

Buttons on screen for skip and go back.

When finished, add prices to items, keep only the latest 5.

**Enter price data screen**

Select a shop

List all items from that shop

Average price is listed beside each item

Click an item to enter a new price

At bottom, a button to finalize price entry.

### Two player shopping mode

New button on Shopping screen: Start multiplayer. Pressing asks for how many players

Generates a link or image to send to someone for each player

Divides the shopping list into equal parts, formats the items into a list that is ordered by section.

Use mobile share option for each player, send image or link based on the app shared to.

Main user needs to tick items at the end of the run.

### Tip the Developer an Item

Requires the price expansion first

Option in the Settings menu to Tip the Developer

Opens a screen listing all your items

Select an item you have a price on

Opens a Venmo or other donation link with the value selected

Adds the Item name as the donation description “Johnny is sending you a bag of rice!”

App is free apart from that.

### Synchronize Data with someone

Generate a link which can be sent to someone

When clicked with the app installed, load the data into your app.

For those “Shit, Honey I am on my way to the store, can you tell me what we need?” phone calls.

### Rewe App Integration

Have a photo of each item's barcode for use with the Rewe ordering app.
