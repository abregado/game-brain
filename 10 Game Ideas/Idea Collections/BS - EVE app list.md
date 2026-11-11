---
title: "BS - EVE app list"
source: "Game Stuff/Game Ideas/BS - EVE app list"
modified: 2020-08-23
type: planning
area: game-idea
status: "idea"
projects: ["[[EVE-like Player Economy]]", "[[Playdate & Small Games]]"]
concepts: ["EVE-like player economy", "EVE App Ideas", "Rookiehunter", "Targeted Killboard", "MyTradeHub WebApp", "Phone Spaceships", "Flocking Algo Fights", "EVE Progression Viewer", "RiskRunner CombatCourier", "Design: Streak Rewards"]
words: 7635
summary: "Large collection of EVE Online third-party web app ideas using the EVE API/SSO: donation and killboard tools, bounty/targeted killboard, Rookiehunter 1v1 rookie-ship deathmatch, MyTradeHub market app, ZoneRecruit, progression viewer, corp tooling, plus game-ish prototypes (flocking-fight ships, phone spaceships with screen lists)."
tags: ["area/game-idea", "project/eve-like-player-economy", "project/playdate-small-games", "type/planning"]
---

# Flocking algo fights

Ships are predesigned:

- Choosing three hull segments

- Stats

  - Cargo slots

  - magazine/charges

  - Top speed

  - Acceleration

  - Engine efficiency

  - Turn rate

  - Engine efficiency

  - Hitpoints

  - Size

  - Energy gen/storage

- Active options

  - Weapons

    - Aim

      - Low rof

      - High accuracy

    - Burst

      - High rof

      - Low accuracy

    - Lead

      - Low rof

      - Mid accuracy

      - High range

  - Shields

    - Passive

      - No recharge

      - No cost

    - Low

      - low cost/recharge

    - Max

      - High cost/recharge

  - Engine Mode

    - Overdrive

      - More energy cost

      - Higher top speed

      - Lower accel

      - Lower turning

    - Dodge

      - Mid energy cost

      - Lower top speed

      - High accel

      - High turning

    - Chase

      - Low cost

      - Mid top speed

      - High accel

      - High turning

# Phone spaceships

Scanning minigame

Three sliders. Values 0-9. Each signature has a value for each. If one value is the same then it shows in the list. If two values are the same then it shows type. If three, then it sticks as warpable.

Ships are predesigned:

- Choosing three hull segments

- Stats

  - Cargo slots

  - magazine/charges

  - Top speed

  - Acceleration

  - Engine efficiency

  - Turn rate

  - Engine efficiency

  - Hitpoints

  - Size

  - Energy gen/storage

- Active options

  - Weapons

    - Perfect range

    - Accuracy

    - Damage

    - Rof

  - Shields

    - Points

    - Energy cost

    - Cooldown

  - Overdrive

    - Cost per second

    - Bonus

    - Cooldown

1 ship type

1 enemy type

Small system map

3 types of combat location

- 1 enemy at a time

- 2 enemies at a time

- 3 enemies at a time

1 type of salvage location: abandoned loot

Three loot items

Sell loot items for money, price based on distance to main station

Buy ships with money

Ammo item, bought with money

Jump, scan, fight, loot, sell repeat

Resources

- Always have two uses

- Come from two places

- Each place only gives one resource type

Loop

- Travel to system

- Sca

# Screens

Combat screen

- Current energy Regen and percent

- Hitpoints at bottom

- Weapons on right

- Targets/friends on left

- Flee button at top

Loot screen

- (When last enemy destroyed)

- Clickable boxes to load into ship

- Each player chooses one or skips

- Button for next room/encounter

Travel screen

- (When all missions in system complete)

- Buttons on left and right to show destinations

- Station in the middle

  - Stations with item marked

- Autopilot at bottom

  - Nearest mission

  - Nearest station

Station screen

- Ship in middle

- Fitting button

- Inventory button

- Character screen

- Ship selection

Inventory screen

- Items shown as boxes

- \+ Box on end with buy

- Click loot to open

- Bottom button row

  - Sell, load, buy more, scrap

- Top bar

  - Shows cargo capacity of ship

  - Cargo value

Fitting screen

- Left hand side

  - Weapons slots

  - Utility

  - Hardwired

  - Hull slots (effect bonus and slot layout, like Stellaris)

- Right hand side

  - Statistics

  - Equipment selection when a slot selected.

    - Shows all equipment options, and which you have in storage.

Ship selection

- Left list

  - All owned ships

  - Current ship at top

- Right shows stats

- Bottom right

  - Construct/buy new ship

New ship screen

- Each hull segment can be selected and compared

- Three buttons in list on left half

- Stats shown on right

- Slots shown per segment

Character screen

- Experience for this hull

- Current skills in list

- Skills which effect this ship at top

- Each skill only has one level

- Each skill costs money and takes time to set in.

- Learning a skill increases XP cost of others.

- Better skills cost more money

- Only pay once and you can use the skill multiple.times.

# EVE API Challenge

Chunks (Pick one)

- Proper certificates per fit

- Log in to check off the current system. Collect badges and shit for completeing constellations and regions. High score list for players. Bonus list for wormholers. Systems visited in last 30 days. 14 day challenge winners.

- SSO check corp member wallets for ammo consumption and collate reimbursements based on killmails Damage Dealt.

- Donation Checker Microservice: user logs in and has their Wallet Transactions checked. List donors based on rolling time period. Player can choose Personal Wallet or Corp Division to check. Create output as a html, or add option to make a widget (fetching API keys) that can be added to any html page, or accessed by any player. style as microservice.

- Donation Prestige Advertising: Read a wallet of “service owner” and list all parties who have donated, in order of total amount per day (rolling per 30 days). Use as automated corp Advertising. If those parties log in with SSO they can edit a link, image and description to be displayed.

- Online Location Checker: multiple users can use SSO to login. List all users who are logged in and in space (using Player Location API). DIsplay this list to all players, including which system they are in. Bonus points for autopilot setter.

- Ship Checker: using Dogma, display the ship of the user when they log in with SSO. Check user character points. Display other logged pilots with similar SP and ship class.

- Local Outlaws: Use current location with SSO to read common killers in the surrounding systems. Find matching lossmails from outlaws to display common ship fit/type.

- Killgame Logic: Players can log in with SSO. No real link to EVE. Press button to “kill” other online target. More points for higher SP than yours. Superuser shows payout needed to be given to each participant.

- Killmail trawling: Find all killmails involving two newbie ships. Rank players who were involved and display in a list on website. Requires no SSO login. We can send EVE-mails/isk to those we discover to have been active with this fight method.

Put it all together (Tinder style PVP locator).

- Users sign in with SSO. Can change their setting from Visible to Invisible (takes 10 minutes to be effective)

- Detect that the player is online in client (using Player Location)

- When visible and online, check if player is in a Rookie Ship (using Dogma checks)

- If all checks then display them in the public list

- Players who pass all checks can see the public list

- Public list includes location and SP count (displays points for a kill)

- check registered players for killmails, calc score and show in scoreboard

- show ‘all time points’, weekly and daily rolling highest

#  

# RiskRunner/CombatCourier

Actually two sites running from the same database.

One site (Courier Duty) tracks players who accept cargo contracts from a “Dummy Pilot”. When a contract is accepted the Accepting Pilots start and end locations are listed publicly on the other site (Blockade Duty). If a pilot kills the target it will be detected by the server via killmail and that pilot is added to the list of pilots who need to be paid out.

Couriers pay an acceptance fee for the contract

Blockaders receive a cut of this fee as bounty if they destroy the target while the contract is open (first kill only, and only if the package is in the killmail).

Adjust the acceptance fee % of cargo to ensure that the site always makes a small profit.

BAD IDEA: Easy to get around by accepting a contract with an alt and using your main to transport the goods. All routes must go through lowsec. Easy to game and still requires constant attention.

# ZoneRecruit

A Meteor app/corp webpage which tracks members timezones by comparing their system time and the server time. When non-logged in viewers arrive at the site they are greeted with a Recruitment page and the name of the recruitment officer for that timezone.

The new player can see four time periods. Above it says : “I play in the morning, during the day, during the evening, or late at night” It shows the number of players for each timezone who have logged in lately.

The server regularly checks APIs of corporation members to see if they are still members. Activity is based on market and kill data.

Other public information could include:

- profit per day/week/month based on all players

- kills per day/week/month

- losses per period

- towers destroyed per period

- rats killed per period

- missions run per period

- isk traded on market per period

These stats can be calculated across the whole corp to be used as advertising.

# Zone Purplechecker

As ZoneRecruit except anyone can sign up. Fleet Commanders (admins) can specify a time slot in which a fleet was run and then all kills by or against signed up players are allocated to activity.

Public viewers can see when fleets have been run compared with their own timezone over the last period (week/month/day).

Fleet kills/losses are also based on location (Fleet Commander specifies a marshalling area) and can also schedule events in advance.

Fleet kill/losses are also associated with the Fleet Commander and top Fleet Commanders are shown to Public viewers. FCs get accredited with all kills made, and all losses, by points (based on hull type).

Public users can sign up to get notification of fleets, and to add their pilots to the list of fleet members, or if they want to be a Fleet Commander.

Bonus Points: FCs can link to a Fleet-Up Doctrine.

# Incentivizer

Tracks members who complete corp contracts and who make donations to the corp wallet. Lists pilots in a leaderboard.

# MemberTraker

set taxation %overall, or fixed per time period.

detect payments automatically.

checks the accountants API, checks Corp list for members

Can accept Api from multiple different corp accountants for Alliance level taxes

Flag members who are inactive

Email leaders an update 7 days before tax due and on due date

# AAR-KillBlogger

A blog which is linked to kills. The Site shows activity and asks you which encounters you want to blog about. You can have multiple authors, and it will ask involved parties to blog. The largest blog for an event is the main piece, and other smaller blogs and comments are shown in a newspaper style column, or as inserted comments.

The public can add comments, text and images as suggestions. The authors can flag suggestions to be automatically added in.

# Targeted Killboard - Crowdsourcing Mercenary Contract Work

Aim-increase isk destroyed in highsec pvp by increasing visibility of targets and providing rewards which are donated by other players.

**How does it work?**

Any player can donate with isk towards a corporation by sending money in game to the organizer, with a corp id number as the reason.

All other donations will be accepted, but will subtract from the senders corp, as protection money.

each month, the corporations with the most isk donated towards it are the Targets.

At the end of the month, The top players with the most solo kills against these corps, in highsec wins half the pot prize, up to the amount destroyed in his accredited kills.

Left over pot goes to the next highest scorer

The target corporations earn double points against each other, but the payout is the same.

------------

Make donating to your own corp worthwhile if you want people to fight you.

Weekly Special ship type rewards: One on one kills with particular ship types.

Special offers for kills in certain systems.

Unused/unpopular weapon systems?

How to detect logistics intervention?

The targetted corp will get a lot of wardecs that month. This creates an investment in success.

Pay isk to be excluded from selection? Protection racquet

how do we advertise this?

- inform killed players thier death helped someone from our site

- inform corps when they are nominated

- inform unregistered killers that their kill is worth something

- forum

- pro-pvp groups

- rivalries

why would players donate?

- they want someone to get blown up

- they want more players to attack them

- they want imfamy

- they want to be protected

- for the lols

have corps pay to stay out, or to stay in.

take 10% for organising, aim for 6bil per month to cover a Plex for the main account.

40% saved for next month? like a jackpot?

price to stay out goes up, based on how many kills you have on the killboard, or based on isk donated to nominated last month.

Maybe, the amount a corp pays to itself counts as negative to its nominative status?

slowing down pilots gaming the system

maximum payout to one player is equal to the destroyed value of all kills?

how to keep target counts up?

- add corps until there are minimum 500 targets

- winner is whoever gets most kills against any of these targets

- this also means that a corp might get targeted even tho someone only donated 1 isk. The reward for fighting them will be much higher (based on the total pot)

- minimum three corps on the list

- if not enough nominations, select random corporations

This idea ties into the wardec and bounty systems very well.

Our app will only store kills from target corps, and doesn't need to store the data forever.

Dont show how much you need to donate to get on top, at most, show how much has been donated for the next period.

Only kills in Low and High are accepted for the campaigns

AWOX kills are not accepted

Only targets that have been in the corp for longer thn one month?

Same corp damage and rats are stripped out

offer a sum of isk for a corp key of anyone who is in a nominated corp. Perhap cover all losses during that period.

should POS kils count even if multiple involved parties? Separate website for pos cleaning. Reward solo POS kills?

Another copy of this app just for POS

Offer isk for corp asset Api keys

list known POS from each corp

record only the basic details and link to a real killboard

killers are individuals, not corp entities

**Site Design**

The landing page only really needs to list the target corps, thier size and the pot prize. Clicking the corp shows sightings, operatinal area, links to evekill and eve info.

Next, total paid out so far, total kills

Next the current highest killers are shown

Scrolling down, the viewer can read a short description of what the site is.

Detail shown: How to get corps nominated, how to stay safe, check if your target is protected, date of the next nominations, that we donate 50mil each month to the pot to cover wardecs, selection process

**Steps to Creation**

'empty' python app running on server

python app serves a webpage with static data

app connects to api and fetches the financial data of a specified character, stores as object, read reason text as variable.

display data on website.

app fetches data on corporations based on financial data

displays top nominated corps on site

totals for a corp can be positive or negative based on reason (decide on keywords)

app recalculates on a weekly (adjustable period) basis, based on financial data during this time.

displays next period start on site

app fetches kill logs on an adjustable period basis

separates losses from nominated corporations

remove same corp and rat damage

remove kills with more than one agressor

add agressor to scoreboard

display scoreboard on site

keep a list of all involved parties and corps, email the organizer the list so they can evemail the participants.

Website once over - release sample html and ask for css styles

Website detail and how to info

release and start first period

# MyTradeHub WebApp

Players in EVE go to a trade hub because everything is available. Setting up a Trade hub means every SKU needs to be available, or consumer confidence will be lost.

Also all orders need to be in the same station, which often doesn't happen when several competing groups place orders in the same system.

### phase one: buyers do everything

**Expected User Outcome:** Groups of Market Players can organise their buy/sell orders so they dont conflict. They can also collaborate to create a new trade hub with good sku coverage. Players are given suggestions as to products, buy/sell price and where to buy new stock. Individual players will open the App, read their notifications, make changes in game, then move on to other content, or play Space Trucker. Group organizers can control what their members see, and decide on a range of settings.

**Use cases:** Jita traders who want to collaborate and not compete with one another.

Highsec Traders who what to trade in groups outside the major hubs without the hassle of checking prices against Jita.

Nullsec Organizations who want to have organised TradeHubs with all items available.

**Features**:

Account Type, Senior Buyer. Can create trade hubs

Account Type, Buyer. Can join a hub and select how many orders to dedicate, and how much capital they have to use.

Account Type, Indie Buyer. Is suggested areas to set up Hubs based on a number of factors. Also is shown profitable trades for other buyers.

Initial Hubs are the normal Eve hubs. These are "run" by the App

Create a new TradeHub Instance, choosing a system to create it in, and if buy and/or sell orders are required.

Which station is selected by the App. All hubs will be in this station. Algorthim should take into account Station Facilities, ease of standings gain. Senior Buyers can pay to change the station in a system if they are the first to set up a hub here. Ths reverts of all hubs are closed.

Add APIs for each trader character in your Buying Coalition

Select “Divide requirements”

System pulls market information and discovered holes in market

System checks current local prices against Jita

System detects local exports (cheap sell orders)

System calculates a batch of highest profit items and divides them out amongst all Buyers

Buyers are notified which items they need to offer for sale. Buy and Sell prices are suggested, based on purchase price, regional average, jita best and mineral price.

tracking of buyers and sku's

- items sold, price, margins, average items per week

- buyers profits including tax, performance index, reaction time based on purchase cost.

purchases based on Jita cost

### phase two: competition or not

each hub can be set to cooperate, remain neutral or compete with others in the system.

Cooperate means the system will not suggest items already covered by other Hubs. If another Hub is also set to cooperate it will suggest the less sucessful Hub stop trading (and offer a buyout price). It will also suggest closing orders if others set to Compete are stocking the same items.

Compete mean the system will suggest items that you are not currently stocking, that others already are, if they are profitable.

Hubs can now set parts of their profile to public, which allows them to display items they are stocking, their Compete/Cooperate ratings.

Hubs can set Category Priority. This effects which items they are offered.

Profiles can be created for a hub and can be flagged for recruitment.

### phase three: suppliers and Distribution Centres

Create new Location- Distribution Centre, these are based on Reprocessing and manufacturing bonuses in a system and so might be different to suggested trade hubs. Again the station can be changed.

works like a hub with only buy orders, but with extra logic.

Suggests buy orders based on local manufacturing costs and Jita sell prices. Also takes nearby Hubs into account.

Hubs in Distro systems will prioritize Mineral and Ingredient items unless the Hub Owner selects a Category Priority.

To supply mineals, set up a TradeHub in the same system.

Theoreticaaly a Buyer can set up lucrative buy orders for local manufacturers to fill, and then sell the goods at Jita. Manufacturers hve an easier time selling goods without travel, and can focus on the new Teams system.

## phase four: logistics

this system allows a user to sign up as an Independant Space Trucker.

The App will suggest buy-sell pairs for the user, based on region, distance,sec status and cargospace.

Option for Hub group owner to select frequency of deliveries, and distribution centre, from which goods come from. This will effect trucker offers. Major trade hubs (Jita,Rens,Amarr,Dodixie)

stocks on each order are now calculated based on delivery frequency and average sales. Decreasing frequency will increase load size, and thus create more likelyhood that truckers fill your orders.

Truckers want to arrive at a location, buy from a list, travel and then sell all, knowing they will make an easy profit.

## phase five: usability and extras

better visability for Opportunities

Public Opportunities every hour as trial

map showing public trade hubs and distros

contract intergration to save tax

skill suggestions (5 more opportunites profitable if you train Acounting 4)

external TradeHub profile page options

notifications when new Hubs open in your systems.

notification when buy orders are available fr stored goods

accounts can place product recommendations at a hub

## phase six: something for manufacturers

New Grop' Consortium. A group of manufactuers. Based in a system.

Builders also base out of one system and select a speciality

players may join to build items.

The App divides up manufactuing responsibility amonst players, based on skill and proit margin.

Suggests younger plauers make lower tier goods

Shows which blueprints are owned by who at which location. Suggests sale price when not on use.

Makes predictions on quantiies required at various locations and distros.

Distros and Hubs can offer contracts to Consortiums to cover periodical orders.

Contract assistant to Hub/Distro owners.

Mfgers of different items need to move around to find the best location.

Consortium get prewarning of what is needd at each distro/hub

They can have the goods in position before the Buyers are notified.

## not worth it: government rule

this is where we start to replace the current corporation system.

When a hub is created it has one CFO. The CFO can raise others to the level of Senior Buyer, and can at this point become a Senior Buyer. If there are two or more Senior Buyers then both must agree on changes and recruitment from now. A CFO has a veto vote, and can make changes without asking. Senior Buyers can start a vote to chage a setting, add or remove Buyers, add or remove Seniority.

This system has minimal value. Instead each group can only have one CFO who can make changrs and give CFO to someone else. If you have a disagreement you can start a new Trade Hub an compete.

EVE App ideas

# Kills per Hull Tracker

Perhaps we could track the number of kills that pilots get per hull..

# EVE Progression Viewer ISIS

Goal. To create a visual representation of a new players suggested progress through EVE Online. The Progression Viewer will guide new players in their skill training and ship choice so they become valuable PvP members of Sefem Velox. We want new players to specialize, not only because it is good for us, but because it will increase retention due to the player being more effective. We also want to promote the use of the few good PvP ships in each racial bracket.

The Progression Viewer should also be usable by players who have not yet made an account for EVE Online so they can see the effects of their choices before they make them.

Visuals

The Progression Viewer should look quite similar to the ISIS screen. Ship icons set apart by connecting lines. The display shows ships the player has currently unlocked and links to ships that are next in the progression tree.

Progression Fields

There will be one View per Racial variety: Caldari, Minmatar, Gallente, Amarr. Players can still decide which of the racial ships they wish to pilot as we will provide suggestions for each.

Progression is based around ship hulls and fittings. Each hull has a number of fits rated Minimum, Good, Better, Best. All ships that a player can fly and fit at the Minimum level are clustered in the centre of the view. Other ships are shown in a ring around this cluster, with links showing which of the currently available ships have similar skills.

Each ship in the inner cluster has a segmented ring display to show how effective the pilot is with the currently highest ranked fit. A symbol or icon is used to denote how many of the fits have been unlocked by this characters skills.

Suggested Ships for Each Race

Caldari

- Condor - Blap

- Crow - Tackle

- Griffin - Ewar

- Keres - Ewar

- Heron - Scanning

- Buzzard - Scanning

Minmatar

- Slasher - Blap

- Rifter - Tackle

- Wolf - DPS

- Thrasher - DPS

- Vigil - Ewar

- Probe - Scanning

Gallente

- Atron - Blap

- Incursus - DPS

- Navitas - Logi

- Exqueror - Logi

- Algos - DPS

- Enyo - DPS

- Ishkur - DPS

- Imicus - Scanning

Amarr

- Executioner - Blap

- Punisher - Tackle

- Retribution - Tackle

- Inquisitor - Logi

- Sentinal - Ewar

- Magnate - Scanning

- Augorer - Logi

# Additional Information

When a ship is clicked on the player can see the top suggested fit for them and can swipe through to the other fits. Expected stats are shown for each as well as a quick strategy guide. The guides show other players as colored TAGs.

# Rookiehunter - Constant Rookieship 1v1 Deathmatch

**Rookiehunters: What is it?**

tldr: a new way to shoot people in the space face for people in all timezones.

Some time ago CCP gave the player of EVE-Online a fantastic feature: Consentual Player Duels. Finally the Capsuleers of New Eden could shoot each other in the face without the police getting involved.

But how do you find other people who want to Duel? How do you know which pilots will give you a fair fight?

This is where Rookiehunters comes in. It shows you other pilots that are looking to fight one-on-one with you.. in Rookieships!

**Why Rookieships?**

tldr: They are cheap and fun

This variety of ship was also buffed recently. It is accessible to players of all ages and skill levels, and can be outfitted in a variety of interesting ways.

Most of all, they are cheap! In order to keep Rookiehunters accessible to new players I wanted to minimize the expense of losing a ship.

Before you ask, there are plans to bring Rookiehunters to all frigate hull classes. Be patient!

\<link to ships page\>

**Why one-vs-one?**

tldr: Teach them to walk before they have to run for thier lives

Solo combat is an integral part of EVE Player versus Player culture, but mostly I wanted Rookiehunters to be accessable to day one (brand new) players. Sadly, new players lack the most important resource in EVE-Online, Contacts.

There are plans to bring small fleet fights to Rookiehunters.

**Prizes you say?**

tl:dr Isk paid to the most active players

YES! Pilots who are involved in Rookiehunters get rewarded for taking part! At the end of each week, a portion of the prizepool is paid out to the pilots who were the most active. Both kills and losses count toward this total, the idea being to compensate new players for having a go.

Veterans who are ISKhappy may opt to forgo their winnings, meaning the prize pool will grow faster and attract more combatants.

\<Winners page\>

**Where is this prize money coming from?**

tl:dr Player Donations

The initial prize pool will come from my own wallet. Future additions to the prize pool will come from player sponsorships.

The Rookiehunters interface allows you to sign up as a Sponsor, or to become a Veteranhunter(tm). Player Donations to our CEO are automatically tracked and added to our database.

Our Interface and webpage displays the current Top 15 Sponsors. Sponsors may log in and update thier advertisment, chosing between thier Capsuleer Portrait or a Corporation Logo. The top advertisments also may have one line of hover text and a url leading anywhere they like.

The top 15 are calculated at the end of each week, so If you make a big donation, you will be seen for at least this long.

All sponsors will be listed on our Sponsors website, as are all Veteranhunters who have forgone at least 1 isk of winnings.

\<link to Sponsors\>

**How are the scores tallied?**

tldr: only killmails between two participating Rookieships count.

This is why you must provide an API granting access to your killmail data. We download and check each of your kills to see if only you and other Hunters were involved. Kills that only involved two hunters are added to our database and used for scoring.

At the end of each week the scores are tallied and the winners in a number of fields are listed on our website. The pilots who were most active receive a portion of the Prize Pool. We may also, at our discretion give prizes for other fields.

\<tips and tricks\>

**How can I get involed?**

tldr: Give us stuff or help as a Tester.

If you are Isk heavy and want to help new players get into PvP, then sign up as a Sponsor. If you wish to remain anonymous you can still donate without signing up.

No Isk? We also need testers for new features, and Javascript coders for math heavy problems.

\<link to R&D\>

Rookiehunter Sessionstates

#### Infopage

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 84%" />
</colgroup>
<thead>
<tr class="header">
<th>Occurs:</th>
<th>when viewing the page from a non-IGB browsers</th>
</tr>
<tr class="odd">
<th>Content:</th>
<th><p>information about Rookiehunter and the devs</p>
<p>current stats (signed up users, total kills, total damage, kills/damage this week) - see Inactive Gamemode</p>
<p>sponsor links</p>
<p>simple html, responsive format page</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

#### Trust Request

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 84%" />
</colgroup>
<thead>
<tr class="header">
<th>Occurs:</th>
<th>when viewing the page from the IGB without trust</th>
</tr>
<tr class="odd">
<th>Content:</th>
<th><p>Rookiehunter logo</p>
<p>trust request label</p>
<p>trust request alert</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

#### Signup Screen

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 84%" />
</colgroup>
<thead>
<tr class="header">
<th>Occurs:</th>
<th><p>when viewing on IGB</p>
<p>when character name is not known to the db</p></th>
</tr>
<tr class="odd">
<th>Content:</th>
<th><p>Disclaimer - you are signing up to compete in Rookiehunter</p>
<p>link to suggested API key</p>
<p>Form</p>
<ul>
<li><blockquote>
<p>Username - prefilled with character name</p>
</blockquote></li>
<li><blockquote>
<p>email address - for password recovery</p>
</blockquote></li>
<li><blockquote>
<p>API key</p>
</blockquote></li>
<li><blockquote>
<p>API vCode</p>
</blockquote></li>
<li><blockquote>
<p>password</p>
</blockquote></li>
<li><blockquote>
<p>password again</p>
</blockquote></li>
<li><blockquote>
<p>submit button</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

#### Login Screen

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 84%" />
</colgroup>
<thead>
<tr class="header">
<th>Occurs:</th>
<th><p>when viewing on IGB</p>
<p>when character is known to the db</p>
<p>when user associated with character is not logged in</p></th>
</tr>
<tr class="odd">
<th>Content:</th>
<th><p>Rookiehunter logo</p>
<p>Pilot name</p>
<p>password input text box</p>
<p>Login button</p>
<p>password recovery button</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

#### Inactive Gamemode

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 84%" />
</colgroup>
<thead>
<tr class="header">
<th>Occurs:</th>
<th><p>when viewing on IGB</p>
<p>when character and user are logged in</p>
<p>when character is not in a rookie ship OR in a station</p></th>
</tr>
<tr class="odd">
<th>Content:</th>
<th><p>current stats for current stats (signed up users, total kills, total damage, kills/damage this week)</p>
<p>sponsor links (5 large, 10 small)</p>
<p>Instructions for changing to active gamemode</p>
<ul>
<li><blockquote>
<p>one line instruction label</p>
</blockquote></li>
<li><blockquote>
<p>one square div, red if in wrong ship, green if in rookie ship</p>
</blockquote></li>
<li><blockquote>
<p>another square div, red if in station, green if in space</p>
</blockquote></li>
</ul>
<p>Pilot stats</p>
<ul>
<li><blockquote>
<p>Pilot Name</p>
</blockquote></li>
<li><blockquote>
<p>Career kills:deaths</p>
</blockquote></li>
<li><blockquote>
<p>Career lost:destroyed</p>
</blockquote></li>
<li><blockquote>
<p>Rookieskill (once implimented)</p>
</blockquote></li>
<li><blockquote>
<p>Weekly K/D</p>
</blockquote></li>
<li><blockquote>
<p>Weekly L/D</p>
</blockquote></li>
</ul>
<p>Update now button</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

#### Active Gamemode

<table>
<colgroup>
<col style="width: 15%" />
<col style="width: 84%" />
</colgroup>
<thead>
<tr class="header">
<th>Occurs:</th>
<th><p>when viewing on IGB</p>
<p>when character and user are logged in</p>
<p>when character is in space AND in a rookieship</p></th>
</tr>
<tr class="odd">
<th>Content:</th>
<th><p>Inactive Gamemode intel</p>
<p>Update now button</p>
<p>Active Game intel</p>
<ul>
<li><blockquote>
<p>systems containing Hunters -</p>
</blockquote>
<ul>
<li><blockquote>
<p>sorted by distance</p>
</blockquote></li>
<li><blockquote>
<p>setDest links for each</p>
</blockquote></li>
<li><blockquote>
<p>colored by sec status</p>
</blockquote></li>
</ul></li>
<li><blockquote>
<p>each hunter shown as name and portrait</p>
</blockquote>
<ul>
<li><blockquote>
<p>colored by Rookieskill</p>
</blockquote></li>
<li><blockquote>
<p>flags if they had kills in the last hour</p>
</blockquote></li>
<li><blockquote>
<p>links to bio</p>
</blockquote></li>
</ul></li>
</ul>
<p>Killboard</p>
<ul>
<li><blockquote>
<p>quake style kill notifications</p>
</blockquote>
<ul>
<li><blockquote>
<p>Killer [method] Victim</p>
</blockquote></li>
<li><blockquote>
<p>show method as weapon system icon</p>
</blockquote></li>
</ul></li>
<li><blockquote>
<p>unbonused value of kill shown</p>
</blockquote></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

RookieHunter Mini Projects

- five inital states:

  - Detected player name in accounts list,not logged in, ask for login pass. Show number of currently logged in players, total accounts signed up.

  - Detected player name in accounts, Logged in, show logout, show shiptype and station/system verifiers.

  - Detected player in acc, logged in, in space, in rookie ship, show logout, show other player locations, show recent killboard.

  - Did not detect player name in accounts, create button -\>offer to make new account (Email, API key, vCode, Password), floating frame

  - Did not detect eve_trusted, tell the user to use IGB, display link to Rookiehunter.info

- signup using igb header, api key,email and password

  - verify character name from API

  - store api key as invite code

  - associate IGB header and api key to login session.

  - associate current IP address with character

- signin using igbheader and password

  - no need to verify API as killmails come from CREST

  - auto gamemode start?

- User account and character Collections

- Character Collection Variables

  - user_id associated

  - name {string,id}

  - system {name,id}

  - kills {victim,system,weapon, time/date}

  - skill {1-5 stars}

  - 

- Manual update location button (refresh?)

- Update details loop while logged in

- Only add unique Pilots to the list, and only if they are in space AND in a Rookie Frigate (Velator, Ibis, Reaper, Impaler)

- Only display the list if you are in the list

- client auto refresh every few minutes

- links to system names and Set destination button

- show plist by systems, sorted by distance or population

- analyse character sheet and catagorize frigate skills

- access and storage for API killmails, strip unwanted data

- detect rookieship kills, pull list from CREST and search for relevant kills.

- display recent kills on plist, including the killers weapon type

- big red button to activate game mode for 24hrs, only if you are in space and in a rookieship.

- Prizepool system

  - detection of prizepool from new character wallet API

  - detection of payouts, comparing payments to expected payouts

  - detection of donations to prizepool

  - display of character or corporations based on donations

  - top 5 donations have larger advertisement display with custom hover and link

  - next 10 top donators have character link and portrait

Rookiehunter scoring

What do we want to reward?

- New player PvP

- Activity

- Risk taking

- Accepting fights regardless of opponent

- Fighting opponents that have more skillpoints

- fitting actual modules to their ships

- Reward as many players as possible

How do we do that

- Bonus points for kills in lowsec and wormholes (+1/+2)

- Take top 10 in each category?

- Weekly bonus, get a kill with ‘X’ weapon

- Bonus points for losing against pilots with more skillpoints

- Reward players who lose the most ships per week (easy to game), bonus per ship they killed

- Reward most dropped value and most destroyed value

- Reward all players who participated

- 5 character skill levels. Lvl1 killing a Lvl5 gets 5x the points

###  

### "Fun generator"

Pilots can register as interested in activity.

Pilots interested in leading a group can request a mission.

The system shares the location of mission leaders only with those who join up.

Matches catagory, location and skill level.

To begin with, only bespke pilots can request missions (boolean). Later pilots can earn standings and eventually lead thier own squads.

Pvp missions could include shooting pocos, stations, or ratting in small gangs of frigates. Pvp for newbies could include highsec small fleet combat in newbie ships.

### Small item collection agency.

Offer to move small cargos to popular trade hubs for very little.

Offer these jobs to players, moving the items to the nearest trade hub

operate constant transport runs between major trade hubs

seed fake transport contracts into the system to mitigate risk

cost per m3 charged to the user fluctuates based on amount transferred weekly. More volume means cheaper or everyone.

cost paid to the trukker per m3 moved is 30-45% of the cost to the user and is modified by weekly completed volume and speed of the transfers.

collateral is fixed as a multiple of the end user cost (changes weekly). This risk is taken completly by the trukker, but is kept low so that some risk is still taken by the end user.

to be automated, this requires CREST access to setting contracts

### Information we can gather from the API

pilot location

pilot skill level in different areas

pilot contracts (read only)

pilot buy/sell orders

pilot isk transfers

pilot isk receipts

detect killmails

pilot assets

Proof of concepts

- Core Functionality

  - Pilot visits a site in the IGB

  - sites asks for specific APIkey

  - pilot gives APIkey

  - website reports pilot name, location and displays on screen

- Skill Summary

  - summary breakdown on skills

  - calculate SP that effects frigate control (including core skills)

- Location Tracker

  - collect location data from IGB

  - refresh every 60 seconds

  - send data to server

  - server generates list of connected pilots to return

  - display list of connected pilots (Name, distance)

- Rookieship Hunter

  - same as location tracker

  - also check current ship

  - if current ship is a rookieship then server returns list of other pilots in rookieships

  - on update, check for killmails including rookie ships and send to server

  - on data send, return list of pilot names who made kills (cache last 10-20 kills)

  - display to player as a Deathmatch kill notification

  - record daily kills, reset at downtime

  - additional options to join group chat

- Rookieship Hunter Bloat

  - Users can donate isk to the prizepool

  - each week payouts are made to anyone who is in the top 50% of kills and deaths (still needs to be manually handled)

  - 30% of the last weeks prizepool goes to killers and 15% to killed

  - then the new donations are added to the prizepool

  - additional option to add prize money to yourself, higher relative extra bounty makes your name shaded red to other players (more fight offers).

- Squadhunter

  - registration of team leader

  - team leader can invite team members (up to 5), and selects a racial team, and Team Name

  - pilots can accept invites

  - killmail detection involving only members of two teams, and only t1 frigates of the selected racial type (all of team 1 participants were flying team 1 race ships)

  - distribute 30% of prize pool to team leaders as per Rookiehunter

  - teams are listed in the scoreboard by their team name

- Squadhunter Rookiestyle

  - as Squadhunter but only with Rookieships

  - transitional gamestyle

  - validated 1v1 killmails count for personal Rookiehunter score AND team score

Salvage Calc and tracker

Corp organiser and heirarchy tracker

Corp transaction tracker/budget/member donation tracker

Fleet designer and pilot suggestor

Trade hub order divider

Map tool showing your market orders and range, corp orders and assets, other non-evemap stuff.

Only detect corp contracts , to add accountability, and ease of use (500 contracts)

Create contract screen, sorted the same way as eve, with confirmation button. Sales list is still taken from contracts API.

Check my sales: loads your contracts and checks them against your catalogue.

Sales list: sort by distance, size, price. Display jita price. Only verified fits that match their catalogue get listed.

Corporations can use their own naming conventions? Or enforce our own part numbers?

Jita/other hub comparison. Compare m3\*jumps for a fit between two trade hubs.

Only one corp api needs to be registered, then anyone with corp contract access can post.

Same system could be used for recycling buyback. Buyers enter prices for raw materials and stations they will collect from. Sellers can search for best price or closest. Both must give contract api information. Webapp verifies price and station based on contracted purchaser. Buyers who are tardy in accepting contracts lose standings, sellers who enter the wrong price lose standings. Standings are listed in the app as a warning.

Anti-price-competition.

All sellers can use all part numbers?

Price must match to be verified?

Limited number of active partnumbers per seller?

Aim:promote inventive and popular fits, rather than offering every option!

Healthy SKUs

Meteor Key names

"host":"localhost:3000",

"connection":"keep-alive",

"eve_shipname":"GOGOMOBILE",

"eve_stationid":"60005239",

"eve_solarsystemid":"30002049",

"accept":"application/xml,application/xhtml+xml,text/html;q=0.9,text/plain;q=0.8,image/png,\*/\*;q=0.5",

"eve_corpname":"Harin Intellegence Services",

"eve_constellationid":"20000302",

"eve_shipid":"957658735",

"eve_constellationname":"Barvigrard",

"eve_corprole":"9223372036854775807",

"eve_charid":"114966273",

"eve_shiptypename":"Minmatar Shuttle",

"eve_shiptypeid":"11132",

"eve_corpid":"467341830",

"eve_solarsystemname":"Uttindar",

"eve_regionname":"Metropolis",

"eve_regionid":"10000042",

"eve_trusted":"Yes",

"eve_serverip":"87.237.38.200:26000",

"eve_charname":"Leisa Harin",

"eve_stationname":"Uttindar V - Moon 17 - Minmatar Mining Corporation Mining Outpost",

"accept-encoding":"gzip,deflate",

"accept-language":"en-us,en",

"accept-charset":"iso-8859-1,\*,utf-8",

"x-forwarded-for":"127.0.0.1",

"x-forwarded-port":"3000",

"x-forwarded-proto":"http",

"x-ip-chain":"127.0.0.1,127.0.0.1"}}\</script\>

Mud style pvp games

player characters generated from eve apis

connection only through the igb and only when in space in a shuttle.

characters bonuses based on eve implants and attributes

each realm has rooms and is set in one constellation

rooms contain avatars(players) and interactibles

players fight eachother using a variety of weapons and drones

the longer a player stays connected, the more information is available about its location.

players can defeat thier enemies by finding and killing thier pods in space.

if a player is detected docking or being outside the target system then they die in the minigame and must start again.

pilots pay isk to attempt a "breach". If they fail then they lose their money.

cost to connect is based on failue rate and amount of money being paid out.

players who are doing well in the minigame are visable to the public (including location) and begin to get bounties on thier heads.

opportunities to cash out (withdral from the game, keeping winnings) are offered with decreasing regularity, and cost a %of winnings.

items can include equipment for the next playthrough, or eve commodities and isk.

positional strategy over ablative numbers game. players have single digit hp, and get warnings against attacks.

each room has strategic locations which can block a number of attacks from other locations.

enemies tht will attack show yellowbox with \[!\]. this means they will attack next turn.

attacking takes 2 or 3 turns based on weapon type (short or long).

firing at the same target again only takes one turn.

to move to the next area, players need to spend turns opening the blast doors between areas.

general game flow: enter room, assess enemies, select locations to move to, take out enemies near the exit you want, move to exit, defend until door open, exit room.

killing everything is not recommended, unrequired and actually dangerous.

clearing a room gives a break but then a harder wave will spawn.

players can shoot eachother as well.

each character class has one unlimited skill with cooldown, and a limited charge per dungeon skill and an attribute bonus.

The Parts that require Automation and Coding

# Rewards

What behaviors do we want to promote?

- pvp activity, not just kills and losses

- helping others

- donating to the corp

- squad commanding

What metrics can we use?

- pvp activity is viewable on the killboard

- helping others can be measured inversely, reward volunteers by lowering rent based on how many jobs they volunteer for.

- donations can be counted, simply see how much more rent they pay per month.

- squad commanding. Use diminishing return streak rewards on running and organising events.

The diminishing return streak rewards gives players status badges or public medals for completing tasks in a streak. These streaks get longer for each level so are exponentially longer if broken.

Example: run a weekly event, run a weekly event for three weeks in a row, 7 in a row, 15 in a row.

These badges should be public, perhaps using the in game medal system, or with titles.

This is also a good way to reward KB actvity, as the rewards are not infinite, but the final goals are not easy to reach.

Example: 10 kills in one week, 10 kills two weeks running, 8 weeks, 6 months. (need to determine what is the minimum to ne considered active)

other reward ideas:

- efficiency over %

- top damage on kill over 1bil per week

- events attended per month over 1 year

- recruitment

- being a question answerer

- events organised

- reaching skill training goals quickly (how to measure)

- flying logi or specialist roles

squad goals

- squad with highest activity (kills+deaths)

- fully active for x weeks

The possibly of having a detailed reward structure in the corp relies on the automation of reward detection. If suitable means cannot be found to scan pilots for rewarding behavior, then I would suggest going without non-event driven rewards.

# Simplifying Taxation

EVEs taxation system only taxes PvE content of the game, and even then most of the expected income for our pilots will come from Sleeper Loot. While there is some value to setting a low (3-5%) tax rate simply to collect a little isk from lowsec belt rats, I dont think its really worthwhile.

New players see taxation as a negative point. It is highly visible to pilots looking for a corp to join and may lead to some choosing another corp.

Instead, collecting tax from players once per month may be a better idea. This is how it is currently done in Sefem Velox (30mil per month).

Sefem Ortus would have a much smaller rent payment (~5mil), which can be reduced by taking on responsibilities (See: [<u>Positions of Responsibility</u>](https://docs.google.com/document/d/1L59SFr3oqnPuZy6fmDF99T95xDxXrUW0MNB-OC-X86g/edit#heading=h.opmgc117w5s))

This could be simplified by creating an application that lists players who have not transferred isk to the corp wallet in the last rent period. Directors could use this application to quickly determine who still needs to pay rent, and to notice players who are donating extra to the corporation each month.

The application could be equally useful to Sefem Velox, so should be prioritized for development
