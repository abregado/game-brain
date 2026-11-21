---
title: "Concept - Social Networking Idea V1.1"
source: "Game Stuff/Non-Game Ideas/Concept - Social Networking Idea V1.1"
modified: 2013-06-12
type: pitch
area: non-game
status: "idea"
projects: ["[[Non-Game Projects]]", "[[Game Business & Funding]]"]
concepts: ["SNACE Contact Exchange", "Game business & funding"]
words: 2041
summary: "Concept paper for SNACE, a P2P contact-exchange address book where users control which fields each contact sees and no data is stored by the company."
merged_versions: ["Game Stuff/Non-Game Ideas/Concept - Social Networking Idea"]
tags: ["area/non-game", "project/game-business-funding", "project/non-game-projects", "type/pitch"]
---

Concept

Secure Networking Address-book

Contact Exchange

Drafted by Ben Buckton

**Table of Contents**

Description 3

Goals of the Concept 3

Cost to User 3

Marketing 4

File Transfer protocol 4

Server Requirements 4

Smartphone Integration 4

Service Comparision 4

Uses for the program 4

Release Features 5

Planned Features 5

Potential Problems 5

# 

#  Description

An offline profile, parts of which are shared with other users using P2P file transfer.

Users enter contact details about themselves using a local client and specify who can see which fields. An online server stores the viewers rights, but does not store the information. Other users may make requests to each other for particular information fields to be filled (or access to be granted), which may be grated or denied by the recipient of each request. Information Fields are created by the users and updated on a central database. These updates then filter down to the client as local patches (much like a definition file of a virus scanner).

As users create more and more fields, and share their new data with each other a unique store of information is created on each computer. Users may fill in fields for other people, either for personal use, or to be sent as recommendations to the profile owner. Their personal information is not stored online in any format. Peer to peer file transfer is used to transfer data between users.

The distribution of your information can be tailored to each contact individually or by assigning contacts to “groups”. These distribution rules are only one way, as each user must chose who can see their information.

The client may also interface with a users social networking sites to generate a contact list and to update information. Transfer of permissions will only be available through the official server.

# Goals of the Concept

- Data is never uploaded or stored by the company

  - Less liability

  - More security of the data

- Users can add data fields and share them automatically

  - No need to think of all data fields

  - Requirements should emerge from the user groups themselves

  - software gets used for more purposes than originally intended

- Free for personal use

  - If it becomes common for people to use, money is not an issue

  - Clans, Guilds and other small unorganised user groups dont have to pay

  - Larger specific groups pay a small subscription service (provide a service)

- Maximum Usability

  - Increased possible user base

  - more people requesting information from their contacts generates more interest

# Cost to User

Personal licence is free. Anyone may download the client. Businesses and Corporate users must pay a yearly fee. Additional features for businesses should be available on pay only. These “premium users” pay on a per-client account basis. Each premium user may use this account from multiple locations or computers.

Platforms

SNACE will initially be targetted towards a non-professional audience and should be available initially on PC. After deployment, compatibility should be expanded to (in this order)

- Android OS laptops/smartphones (users concerned with web security)

- iOS products (largest market share of users, professional and not)

- Apple OS desktop/laptop products. (professional non-business audience)

- Blackberry. Only if it takes off in other market areas.

# Marketing

Initial target audience is non-professional users who value privacy. Getting the message about the product can be accomplished with direct and viral marketting. “Modern” approaches to direct marketing include Facebook, Twitter and other social networking presence works well for the bulk markets, but transparency throughout devlopment (devblogs, Q&A, community input) appeals to the technically minded market more.

Through current social networking sites. Adding an “App” to facebook that can interface with the client will assuredly increase popularity.

# File Transfer protocol

Any currently available P2P protocol would be best. As information will be transferred between clients directly, updates to information will only be available when the two parties involved are both online. Bittorrent may be worth investigating.

# Server Requirements

(I'm no expert and unsure what to expect in this department). The database would have to keep track of user accounts, their contacts accounts, and access relationships between each contact and information field. Also the P2P address of each client, which would need to be updated each time a client connects.

# Smartphone Integration

Write about smartphones here

# Service Comparision

|                   | SNACE | Google | Facebook | Ect |
|-------------------|-------|--------|----------|-----|
| P2P Data transfer |       |        |          |     |
| Stored Locally    |       |        |          |     |

# Uses for the program

- User groups who utilize phone, email or other communication methods who require contact organising.

- Facebook/Twitter users who would like to keep contact information for offline use

- Small-Medium businesses for keeping track of employee details

- other organisations who need to keep hierarchy information and share it accordingly

- Syncing information through a single PC

- any application where the information stored must be given by the contact (legality/liability)

- Online gaming guilds for organisation and communication between games (a players character names in different games)

# Release Features

- Name, DoB, multiple Phone#s, email addresses, popular social site links, blog links, RL address

- live information requests

- local information addition (not overridden by live updates)

- info field suggestion box (reviewed by devs each week)

- contact groups with grouped permissions

- global primary contact name field selectable by user

- primary contact name field can be set for each group

- sort contacts by group, Primary name, location (perhaps distance from you), and regular sorting types (alpha first name, alpha last night), favourites

- Information is timestamped when it is updated on the local database

- ability to block others from making suggestions to your information

- ability for local info-book to be stored on a portable drive.

- New fields linked to existing fields (instructions for mobile linked to mobile number)

# Planned Features

- Organisation charts

- Relationship to other contacts

- Birthday reminders

- levels of fuzzyness

- group requests

- Google maps integration

- common GPS software integration

- Calendar integration

- Family tree functions/contact relationship tree ect...

# Potential Problems

Getting users to install ANOTHER client

Solutions:

- Ease of install (msi, small client size)

- Client is non-intrusive (shouldn’t this be the case with ALL software)

- Small download size

- Memory and CPU footprint as small as possible

- Install direct to USB key

- Break client in two (notification monitor and addressbook proper)

Targeted data miners collecting data from users (technically not OUR problem)

Solutions:

- Encrypted data (++CPU use)

---

## Differences from other versions

_This document existed in several versions. The text above is the most complete one, unchanged. Below are the lines that appear only in the other versions._

### Only in “Concept - Social Networking Idea” (Non-Game Ideas, modified 2013-06-12)

Description 2
Goals of the Concept 2
Marketing 3
File Transfer protocol 3
Server Requirements 3
Uses for the program 3
Release Features 3
Planned Features 4
Potential Problems 4
