---
title: "Corp Tax Pseudocode"
source: "Game Stuff/Non-Game Ideas/Corp Tax Pseudocode"
modified: 2014-11-06
type: design-doc
area: non-game
status: "designed"
projects: ["[[EVE-like Player Economy]]"]
concepts: ["EVE Corp Tax Tool", "EVE-like player economy"]
words: 270
summary: "Pseudocode for a tool that tracks EVE Online corporation member tax payments via API and produces an in-game-browser report."
tags: ["area/non-game", "project/eve-like-player-economy", "type/design-doc"]
---

Globals

taxationPeriod = 30 (days)

taxationAmount = 20000000 (isk)

Member Object

paymentList

lastTaxedStamp

lastPayedStamp

balance

joined

active

function Update

loadData from file

checks for new members from corp api

adds missing corp members, setting their join date as the tax start date

checks each existing member, setting their status as idle if no longer a member, or reactivating them if now a member again

get latests transactions

for each transaction do

check if it is a player-corp transfer

if yes then addPayment

for each member, calculateTaxation

set the lastUpdateTime to be now, so that transactions dont get added more than once

backupData to file

prepareReport

function addPayment(amount, member, paymentTimestamp)

check the payment has not already been added, using timestamp

add the payment to the members payment list, including timestamp)

update the members balance attribute

update members lastPaid

if the member was flagged inactive, reactivate them (obviously active now they made a payment)

function addCharge(amount, member, timestamp)

check the charge has not already been added, using timestamp

add the charge to the members payment list, including timestamp

update members lastTaxed

update the members balance attribute

function calculateTaxation(member,newTimestamp)

check when the member was last taxed

if member is active

caluclate the time difference

calculate the taxation amount

addCharge

prepareReport

find members who are behind on payments and who have not made a payment for the TaxPeriod

these members should be shown at the top of the report, sorted by time since last payment

other members are listed below, showing number of outstanding days paid

sort by outstanding days

write to html local file

viewable in the IGB

simple color scheme and css
