---
title: "Flutter App ideas"
source: "Game Stuff/Flutter App ideas"
modified: 2024-09-04
type: idea
area: other
status: "idea"
projects: ["[[Board & Card Games]]"]
concepts: ["Deck App", "Tom Steamroller Creep"]
words: 171
summary: "Concept for an open-source, local-first card/deck app in Flutter with Tables, Piles, Cards and Schemas shared via QR codes."
tags: ["area/other", "project/board-card-games", "type/idea"]
---

Flutter App ideas

**Deck App.** Open source, user content based, generic enough for most deck setups.Decks shareable via QR code. Data all stored locally. No User accounts.

A **Table** is a single page of Piles. It controls the layout and size of Piles. Tables are plaintext json documents and can contain links to Schemas.

**Piles** contain Cards. They control the interaction with cards in them.

**Cards** are generated from Schemas and held in Piles. Cards remember which Pile they started in, and which Schema they came from.

**Schema** are collections of card setup descriptors, containing a number of card images, quantities of each card, card back image. Schemas are plaintext json documents.

A user can scan a QR code pointing to a plaintext document.

If it registers as a schema json then the schema and corresponding images are downloaded to the local device.

If it registers a Table json, then it adds the table to your App, and downloads any linked Schemas.

Tom Steamroller Creep

Hardware devices instead?

NFC card transfer
