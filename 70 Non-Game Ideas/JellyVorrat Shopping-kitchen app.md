---
title: "JellyVorrat Shopping-kitchen app"
source: "Game Stuff/Non-Game Ideas/JellyVorrat Shopping-kitchen app"
modified: 2023-01-11
type: design-doc
area: non-game
status: "designed"
projects: ["[[Non-Game Projects]]"]
concepts: ["Kitchen Stocktake App", "Design: Tinder-style Shopping List"]
words: 440
summary: "Design for JellyVorrat, a swipe-based kitchen stocktake and shopping list app with photo items, monetization via tips and account-less list sharing."
tags: ["area/non-game", "project/non-game-projects", "type/design-doc"]
---

Shopping/kitchen app

# UX Modes

## Add item/Onboarding mode

The user adds each item using the camera or a text field.

- Enter all the ingredients in your kitchen. Photo or name. In order.

- Confirm ordering of items in a drag drop list.

## Stocktake mode by location

The user is shown each item and swipes to confirm if it is present or not

- Select location

- Show objects in order one at a time

- Swipe left or right

## Stocktake mode by shop

The user is directed to all locations and asked to check for items that come from a specific shop

- Direction to go to location

- Tap to continue

- Show items one by one

- Swipe left/right to change item status

## Shopping list Tinder mode

User arrives at the shop and gets shown a list of needed items that come from here.

- Select which supermarket you are at

- Show missing items one by one in Supermarket order

- Swipe left/right to Check off (or ignore) as you get them in the trolly

#  

# Data structures

**Items/Objects**

- Photo

- Name

- Location name

- Location order

- List of supermarkets

- Supermarket order for each supermarket

**Locations**

- Name

**Shops**

- Name

#  

# Development

## Monetization

If the MVP functions well, add in an option to add a price to each item. This price is shown when the user sees the item image at the supermarket.

If an item is purchased often, then when doing stocktake ask the user if they want to tip us the value of the item. “Is JellyVorrat worth as much as this item?”.

If a user tips, then they get a badge in one of the corners to show they are a supporter.

## Marketing

This is the sticking point. How do you get this product to be seen when it is specifically offline. Advertising on data awareness communities and other esoteric online locations will not get us very far.

## List sharing without accounts

Utilise messenger app share buttons to allow users to send each other images that show the items that are needed. Encode item data into the images that can be read by the JellyVorrat app.

If users want to synchronise their lists, then generate a hyperlink that can be opened by the JellyVorrat app, which will give the user the option to add the data to their lists. How the users send this to each other is not our issue.

NFC could also be used to sync lists, or encryption keys if we wanted to do encrypted data.
