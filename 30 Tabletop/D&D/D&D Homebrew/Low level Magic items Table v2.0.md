---
title: "Low level Magic items Table v2.0"
source: "Game Stuff/Low level Magic items Table v2.0"
modified: 2022-08-14
type: homebrew-rules
area: dnd
status: "designed"
projects: ["[[D&D Homebrew]]"]
concepts: ["D&D homebrew items"]
words: 6556
summary: "Homebrew D&D 5e system for generating low-level magic items with rarity, effect and penalty tables, activation rules, charges, example items and further item ideas."
tags: ["area/dnd", "project/d-d-homebrew", "type/homebrew-rules"]
---

**Generation Method**

1.  Consult the item rarity table

2.  Roll on effect table a number of times

3.  Roll on the Penalty tables, rerolling until you have no duplicates.

4.  Increase item level

5.  Recalculate/simplify charges. Items always start with 4 charges.

6.  Decide which kind of item, weapon or armour it will be.

7.  Add price to weapon or armour value, or see Jewellry size price.

8.  Give the item a fitting name and descriptive flare.

**When are effects active? When can I trigger effects?**

**Passive**. The effect is always active, as long as the item is touching the attuned user.

**Passive when held**. The effect is always active as long as the item is being touched by an attuned users hand.

**Free action (unspecified).** You can use this effect at any time, and as many times as you like, on your turn.

**Free action, when \[trigger\].** You can use this effect at any that corresponds to the trigger, regardless if it is your turn or not.

**Reaction (unspecified).** You can use this effect at any time, and as long as you can spend your reaction.

**Reaction, when \[trigger\].** You can use this effect at any that corresponds to the trigger as long as you can spend your reaction.

**Bonus Action.** On your turn, at any time before, after or in the middle of movement, as long as you can spend your bonus action.

**Bonus Action, when also \[specific action\].** On your turn, at any time before, after or in the middle of movement, as long as you can spend your bonus action and already declare your intention to use your Action on the specified action.

**Action**. On your turn, at any time before, after or in the middle of movement, as long as you can spend your Action

**Ritual \[time\]**. Takes a number of minutes to complete outside of combat as given by the time. Can be completed during any rest without interrupting the rest.

**When do items recharge?**

By default, items regain all of their charges at the end of a long rest. Some abilities might change this.

| **Item Price** | **Size**    | **Description**                                                     |
|----------------|-------------|---------------------------------------------------------------------|
| 200            | Tiny, Worn  | Ring, Earring, Brooch, Amulet on chain, Bracelet                    |
| 100            | Small, Worn | Bracer, Helm, Gauntlet, Greaves, Boots, Belt, Pauldron, Cape, Cloak |

| **Item rarity** | **Price**          | **Rolls** | **Bonus Effects** |
|-----------------|--------------------|-----------|-------------------|
| Uncommon        | 200 + item price   | 1         |                   |
| Rare            | 2,000 + item price | 2         | 1                 |
| Very Rare       | 15,000-30,000      | 3         | 2                 |
| Legendary       | 150,000-300,000    | 4         | 3                 |

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 30%" />
<col style="width: 30%" />
<col style="width: 30%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>D6</strong></th>
<th><strong>Effect Jewellery</strong></th>
<th><strong>Effect Weapon</strong></th>
<th><strong>Effect Armour</strong></th>
</tr>
<tr class="odd">
<th>1</th>
<th><p>1 Jewellery effects and a weak effect now, and one Penalty at end.</p>
<p>Reroll if the item already has a penalty.</p></th>
<th><p>weapon effect + weak effect and one Penalty at end.</p>
<p>Reroll if the item already has a penalty.</p></th>
<th><p>armour effect + weak effect and one Penalty at end.</p>
<p>Reroll if the item already has a penalty.</p></th>
</tr>
<tr class="header">
<th>2-4</th>
<th>Jewellery effect</th>
<th>Weapon Effect</th>
<th>Armour Effect</th>
</tr>
<tr class="odd">
<th>5-6</th>
<th>Roll extra bonus at end if this is the second roll, otherwise Jewellery effect.</th>
<th>Roll extra bonus at end if this is the second roll, otherwise Weapon effect.</th>
<th>Roll extra bonus at end if this is the second roll, otherwise Armour effect.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

| **Damage level** | **Damage formula** | **Damage types**   | **Conditions/Effects**                                 |
|------------------|--------------------|--------------------|--------------------------------------------------------|
| 1                | 1                  | Fire, Cold, Poison | Prone, Poisoned, Deafened, Grappled, Moved unwillingly |
| 2                | d4                 | Lightning, Acid    | Restrained, Frightened, Blinded, Charmed, Stunned      |
| 3                | d6                 | Radiant, Necrotic  | Paralyzed, Petrified                                   |
| 4                | d8                 | Psychic, Force     |                                                        |
| 5                | d10                |                    |                                                        |
| 6                | d12                |                    |                                                        |
| 7                | 2d6                |                    |                                                        |
| 8                | 3d6                |                    |                                                        |

| Level | **Saving throw bonus**   | **Skill check bonus** | **Attack roll bonus** | **Spell/slot type** |
|-------|--------------------------|-----------------------|-----------------------|---------------------|
| 1     | Reroll 1’s/20’s          | Reroll 1’s            | Reroll 1’s            | Cantrip             |
| 2     | +/- d4                   | +d4                   | +d4                   | Level 1 spell       |
| 3     | advantage/disadvantage   | advantage             | advantage             | Level 3 Spell       |
| 4     | Immunity to/Auto failure | Expertise             | Expertise             | Level 5 Spell       |

<table style="width:100%;">
<colgroup>
<col style="width: 18%" />
<col style="width: 27%" />
<col style="width: 27%" />
<col style="width: 27%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th><strong>Jewellery Weak Frequent</strong></th>
<th><strong>Jewellery Normal</strong></th>
<th><strong>Jewellery Strong Infrequent</strong></th>
</tr>
<tr class="odd">
<th>Skill bonus, specific skill</th>
<th>Passive: Skill bonus level 1</th>
<th>Free action: Spend two charges. Level 2 skill bonus to next check.</th>
<th>Action: Spend 4 charges. Level 3 skill bonus to next check.</th>
</tr>
<tr class="header">
<th>Hit dice for spell slots.</th>
<th>Reaction when you cast a level 1 spell: Spend a hit die instead of a level 1 spell slot.</th>
<th>Action: Spend a hit die to gain a level 1 spell slot.</th>
<th>Ritual: Spend 4 charges, convert any number of hit dice into level 1 spell slots.</th>
</tr>
<tr class="odd">
<th>Damaging Hit dice for spell slots.</th>
<th>Reaction when you cast any spell: Roll a number of hit dice equal to the spell level and suffer the damage. The spell is considered one level higher.</th>
<th>Free action: Roll up to [item level] hit die and suffer the damage. Recharge one level 1 spell slot per dice rolled.</th>
<th>Bonus action: Spend 4 charges, Roll any number of hit dice and suffer that much damage. Recharge spell slots equal to the dice rolled + 1.</th>
</tr>
<tr class="header">
<th>Spell level boost</th>
<th>Reaction when you cast a spell: Spend a charge. Boost a spell slot by one level.</th>
<th>Reaction when you cast a spell: Spend two charges. Boost a spell slot by two levels.</th>
<th>Reaction when you cast a spell: Spend four charges. Spend a spell slot three levels lower.</th>
</tr>
<tr class="odd">
<th>Spell slot modification</th>
<th>Action: Spend a charge. Upgrade a spell slot one level.</th>
<th>Action: Spend two charges. Upgrade your lowest spell slot by two levels.</th>
<th>Action: Spend four charges. Upgrade your lowest spell slot by three levels.</th>
</tr>
<tr class="header">
<th>Spell duration</th>
<th>Reaction when you cast a spell with duration: Increase the duration by one round.</th>
<th>Reaction when you cast a spell with duration: Spend two charges. Increase the duration by one minute.</th>
<th>Reaction when you cast a spell with duration: Spend 4 charges. Double the duration.</th>
</tr>
<tr class="odd">
<th>Saving throw, specific ability</th>
<th>Passive: Level 1 saving throw bonus for one type.</th>
<th>Reaction: Spend 2 tokens. Level 2 saving throw bonus for one type.</th>
<th>Reaction: Spend 4 tokens. Level 3 saving throw bonus for one type.</th>
</tr>
<tr class="header">
<th>Saving throw, specific aggressor</th>
<th>Passive: Level 2 saving throw bonus against effects causing one condition/creature.</th>
<th>Reaction: Spend 2 tokens. Level 2 saving throw bonus against effects causing one condition/creature.</th>
<th>Reaction: Spend 4 tokens. Level 3 saving throw bonus against effects causing one condition/creature.</th>
</tr>
<tr class="odd">
<th>Gain temporary hit points from hit dice</th>
<th>Reaction when hit with an attack: Spend a charge. Gain temporary hit points equal to your level, after the attack is resolved.</th>
<th>Action: Spend a hit die and two charges. Gain temporary hit points equal to twice the rolled amount.</th>
<th>Spend any number of hit dice to gain temporary hit points equal to twice the total rolled, until your next rest.</th>
</tr>
<tr class="header">
<th>Tactical sense, specific creature.</th>
<th>Passive: Detects when one creature type is within 60ft of you.</th>
<th>Part gains Advantage on initiative against one creature type, twice per long rest.</th>
<th>Party is immune to being surprised by one creature type, once per long rest.</th>
</tr>
<tr class="odd">
<th>AC transfer</th>
<th>Bonus action: Transfer 1 level of AC until the start of your next turn.</th>
<th>Bonus action: Spend a charge. Transfer 2 levels of AC until the start of your next turn.</th>
<th>Bonus action: Spend two charges. Transfer 3 levels of AC until the start of your next turn.</th>
</tr>
<tr class="header">
<th>Remove conditions</th>
<th>Reaction: Remove a specific level 1 condition. Your speed is zero until the end of your next turn.</th>
<th>Free action, at the end of your turn: Spend two charges. Remove a specific level 1 condition.</th>
<th>Reaction: Spend 4 charges. Immediately remove a specific level 1 condition.</th>
</tr>
<tr class="odd">
<th>Hit dice modification</th>
<th>Passive: Reroll 1’s on when you roll a hit die.</th>
<th>Free action: Spend 2 charges. The next hit die spent rolls maximum.</th>
<th>Action: Spend 4 charges. Roll any number of hit die. Heal the amount rolled.</th>
</tr>
<tr class="header">
<th>Spell skill bonus</th>
<th>Passive: Choose a spell you know. Level 1 skill bonus when casting that spell.</th>
<th>Bonus action: Choose a spell you know. Level 2 skill bonus when casting that spell.</th>
<th>Action: Choose a spell you know. Level 3 skill bonus when casting that spell.</th>
</tr>
<tr class="odd">
<th>Environmental Resistance</th>
<th>Passive: Resistance to one elemental environmental damage.</th>
<th>Passive: Immunity to travel penalties from one environment type.</th>
<th></th>
</tr>
<tr class="header">
<th>Spell range</th>
<th>Reaction: Increase the next ranged spell cast by 5ft.</th>
<th>Bonus Action: Increase the next ranged spell cast by 15ft.</th>
<th>Action: Double the range of the next spell cast.</th>
</tr>
<tr class="odd">
<th>Spell Damage type</th>
<th>Reaction: Change the damage type of one cantrip to another damage type of the same level.</th>
<th>Action: Spend 2 charges. Change the damage type of one level 1 spell to another damage type of the same level.</th>
<th>Ritual: Spend 4 charges. Change the damage type of one spell to another damage type of the same level until your next rest.</th>
</tr>
<tr class="header">
<th>Darkvision</th>
<th>Passive: 15ft darkvision</th>
<th>Bonus Action: Spend 1 charge. Darkvision 30ft for 10 minutes.</th>
<th>Ritual: Spend 2 charges. Darkvision 60ft for 1 hour.</th>
</tr>
<tr class="odd">
<th>Ally save advantage</th>
<th>Reaction: Grant an ally within 5ft level 1 bonus on a saving throw.</th>
<th>Reaction: Spend a charge. Grant an ally within 5ft level 2 bonus on a saving throw.</th>
<th>Action: Spend 4 charges. Grant an ally within 5ft level 3 bonus on the next saving throw they make.</th>
</tr>
<tr class="header">
<th>Casts cantrip</th>
<th>Stores 1 cantrip. Costs nothing to cast.</th>
<th>Stores 2 cantrips. Spend 1 charge to cast any of them.</th>
<th>Stores three cantrips. Spend 2 charges to cast any of them.</th>
</tr>
<tr class="odd">
<th>Stores spell</th>
<th>Stores up to 4 cantrip uses. Drains at the start of any long rest. Anyone can store. Attuned can cast as if they were the storer.</th>
<th><p>Stores one level 1 spell.</p>
<p>Drains at the start of any long rest. Anyone can store. Attuned can cast as if they were the storer.</p></th>
<th>Stores one level two spell. Drains as soon as you cast a spell. Only Attuned can store and cast.</th>
</tr>
<tr class="header">
<th>Reaction casting</th>
<th><p>Reaction when hit by an attack: Cast a cantrip that can target your attacker.</p>
<p>Cantrip chosen when attuning.</p></th>
<th>Reaction when hit by an attack: Spend 2 charges. Cast an instantaneous level 1 spell that uses a Bonus action, and does not require concentration.</th>
<th>Reaction when hit by an attack: Spend 4 charges. Cast any spell that uses an action. You gain a level 2 condition until the end of your next turn.</th>
</tr>
<tr class="odd">
<th>Stealth reroll for condition.</th>
<th>Reaction, when you roll a Stealth check: Gain a level 2 condition and reroll the result.</th>
<th>Reaction, when you roll a Stealth check: Spend 2 charges. Reroll the result. Gain a level 1 condition.</th>
<th>Reaction, when you roll a Stealth check: Spend 4 charges. Maximise the result. Gain a level 2 condition</th>
</tr>
<tr class="header">
<th>Ammunition recovery.</th>
<th>Passive: +2 to ammunition recovery rolls.</th>
<th>Action: Create level 2 dice of ammunition for a weapon you have by touching a non-magical weapon. The touched weapon disintegrates.</th>
<th>Ritual: Create 3x level 2 dice pieces of ammunition for a weapon you have by touching a non-magical weapon. The touched weapon disintegrates.</th>
</tr>
<tr class="odd">
<th>Class resource to Spell slot.</th>
<th>Free action: Spend your [class resource/Channel Divinity] to gain a level 1 spell slot.</th>
<th>Action: Spend your [class resource/Channel Divinity] to gain a level 2 spell slot.</th>
<th>Ritual: Spend your [class resource/Channel Divinity] to gain a level 3 spell slot.</th>
</tr>
<tr class="header">
<th>Spell Concentration</th>
<th>Reaction: Spend a charge. Level 2 bonus on a Concentration check you are about to make.</th>
<th>Reaction: Spend two charges. Reroll a failed Concentration check.</th>
<th>Free action: Spend 4 charges. Gain level 3 bonus on Concentration checks for the duration of the next spell you cast.</th>
</tr>
<tr class="odd">
<th>Casting components</th>
<th>Free action: Spend two charges. The next spell you cast does not require one of its Somatic or Verbal components.</th>
<th>Reaction: Spend a charge. The next spell you cast does not require one of its Somatic or Verbal components.</th>
<th>Free action: Spend 4 charges. The next spell you cast does not require both its Somatic and Verbal components. It is also completely undetectable.</th>
</tr>
<tr class="header">
<th>Language knowledge</th>
<th>Passive: You can understand and read one language you did not know before.</th>
<th>Free action: Spend a charge. For 10 minutes you can understand, speak, read and write one language you did not know before.</th>
<th>Ritual: Spend 4 charges. For 1 hour you understand, speak, read and write one language that you have in front of you during the ritual.</th>
</tr>
<tr class="odd">
<th>Heal yourself when you help others</th>
<th>Passive: Level 1 damage healed when casting a spell on a friendly target..</th>
<th>Passive: Level 2 damage healed when casting a spell that heals a target.</th>
<th>Free action, when you heal a target: Spend 4 charges. You heal the same amount as the target.</th>
</tr>
<tr class="header">
<th>Temporary hit points for yourself when you help others</th>
<th>Passive: Level 2 damage temporary hit points gained when casting a spell on a friendly target. These last until your next rest.</th>
<th>Passive: Level 3 damage temporary hit points when casting a spell that heals a target. These last until your next rest.</th>
<th>Free action, when you heal a target: Spend 4 charges. You gain double the temporary hit points that the target healed. These last until your next rest.</th>
</tr>
<tr class="odd">
<th>Attack roll bonus</th>
<th>Passive: Level 1 bonus to [spell,melee,ranged] attack rolls when held.</th>
<th>Passive: +1 to [spell,melee,ranged] attack rolls when held.</th>
<th>Free action, when you take the Attack action: Spend 2 charges. All attack rolls gain a +2 bonus.</th>
</tr>
<tr class="header">
<th>Protection against affected creatures</th>
<th>Passive: +2 AC against attacks from creatures under the effect of one of your spells.</th>
<th>Passive: Level 3 save bonus on saving throws against creatures under the effect of one of your spells.</th>
<th>Passive: creatures under the effect of one of your spells trigger AoO when moving into melee range of you.</th>
</tr>
<tr class="odd">
<th>Teleport when you cast</th>
<th>Passive: You can teleport 5ft every time you expend a spell slot.</th>
<th>Reaction when you cast a spell: Spend 2 charges. Teleport 10ft to a point you can see.</th>
<th>Reaction when you cast a spell: Spend 4 charges. Teleport 20ft to a point you have seen recently.</th>
</tr>
<tr class="header">
<th>Power over affected creatures</th>
<th>Passive: Creatures already under the effect of one of your spells suffer a level 2 penalty to their AC when you attack them.</th>
<th>Passive: Creatures already under the effect of one of your spells suffer a level 2 penalty to their Saving throws from spells you cast.</th>
<th>Passive: Creatures already under the effect of one of your spells cannot move out of your threat range without using the disengage action.</th>
</tr>
<tr class="odd">
<th>Hit dice</th>
<th></th>
<th>Passive: Reroll any spent hit dice once.</th>
<th>Passive: Regain one charge or one hit die during a short rest while attuned to this item.</th>
</tr>
<tr class="header">
<th>Initiative Bonuses</th>
<th>Passive: +1 to initiative rolls</th>
<th>Free action, after Initiative order has been calculated: Swap initiative count with one other willing player.</th>
<th>Free action, before rolling Initiative: Spend 2 charges. Your initiative score is 18 + item level.</th>
</tr>
<tr class="odd">
<th>Item charge transfer</th>
<th>Passive: While attuned to this item, your other items have their max charge increased by 1.</th>
<th>Action: Spend two charges. Another item you can touch recharges 1 charge.</th>
<th>Ritual: Transfer as many charges from this item to other items, 1-to-1.</th>
</tr>
<tr class="header">
<th>Insight extra information.</th>
<th>Free action, when you make an Insight check: Spend 1 charge. Learn the target’s name. Fiends must make a DC 10 Charisma saving throw. On a failure you learn their true name. If you learn a true name, the item disintegrates.</th>
<th>Free action, when you make an Insight check: Spend 2 charges. Learn the primary emotion the target is feeling right now.</th>
<th>Free action, when you make an Insight check: Spend 2 charges. You automatically pass the Insight check, but the target knows that you know.</th>
</tr>
<tr class="odd">
<th>Disengagement changes</th>
<th>Passive: when you take the Disengage action: You may move through spaces containing creatures.</th>
<th>Bonus action, when you take the Disengage action: Spend a charge. Also take the Dash or Dodge action.</th>
<th>Free action when you take the Disengage action: Spend 4 charges. All your movement this round is considered teleportation.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

|                      | **Any Weak**                                                        |                                                                                                                            |                                                                       |
|----------------------|---------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|
| Attunement           | Passive: Attunement cannot be stolen.                               | Passive: Attunement is not lost from the item being more than 100m away, unless it is taken to another plane of existence. | Item does not need an attunement slot, but still requires attunement. |
| Inventory properties | Ritual: Change the items form into one other type of the same size. | Passive: Item does not take any inventory space as it follows you on its own.                                              | Passive: Item cannot be removed without consent.                      |
| Cantrips             |                                                                     | Cantrip stored, cast twice per day. Anyone can use it.                                                                     | Two Cantrips stored, cast one, once per day. Anyone can use it.       |
| Visual effects       | The item casts Prestidigitation on itself constantly.               | The item can change how its surface looks at will.                                                                         | Passive: You do not need the correct proficiency to use this item.    |

<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 26%" />
<col style="width: 26%" />
<col style="width: 26%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th><strong>Weapon Variant 1</strong></th>
<th><strong>Weapon Variant 2</strong></th>
<th><strong>Weapon Variant 3</strong></th>
</tr>
<tr class="odd">
<th>Attack roll bonus</th>
<th>Free action when making an attack roll. Spend a charge: +2 to attack roll.</th>
<th><strong>Passive: +1 to attack rolls when using this weapon.</strong></th>
<th>Free action when making an attack roll. Spend four charges: +5 to attack roll.</th>
</tr>
<tr class="header">
<th>Passive good elemental</th>
<th>Passive: +1 damage level of a choice between two level 2 damage types against a specific creature type.</th>
<th><strong>Passive: +1 damage level of an level 2 damage type</strong></th>
<th>Passive: +2 damage levels of a level 2 damage type when you have advantage on your attack roll.</th>
</tr>
<tr class="odd">
<th>Passive elemental damage.</th>
<th>Passive: +1 damage level of a choice between two basic elemental types</th>
<th><strong>Passive: +2 damage level of an basic elemental type</strong></th>
<th>Passive: +3 damage levels when you have advantage on your attack roll.</th>
</tr>
<tr class="header">
<th>Passive elemental, conditional</th>
<th>Passive: +1 damage level of two basic elemental types against creatures suffering from a level 1 condition.</th>
<th>Passive: +2 damage level of a basic elemental type against creatures suffering from a level 1 condition.</th>
<th>Passive: +3 damage levels against creatures suffering from a level 2 condition.</th>
</tr>
<tr class="odd">
<th>Passive Elemental, creature type.</th>
<th>Passive: +2 damage level of a choice between two basic elemental types but only against one type of creature.</th>
<th><strong>Passive: +3 damage level of a basic elemental type, but only against one type of creature.</strong></th>
<th>Passive: +4 damage levels against creatures but only against one named creature type.</th>
</tr>
<tr class="header">
<th>On demand elemental damage, free action</th>
<th>Free action, on a hit: Spend a charge. +3 damage levels elemental damage.</th>
<th>Free action on a hit: Spend two charges. +4 damage levels elemental damage.</th>
<th>Free action on a hit: Spend four charges. +5 damage levels elemental damage.</th>
</tr>
<tr class="odd">
<th>On demand elemental damage, reaction</th>
<th><strong>Reaction on a hit: +3 damage levels elemental damage.</strong></th>
<th>Reaction on a hit: Spend a charge. +4 damage levels elemental damage.</th>
<th>Reaction on a hit: Spend two charges. +5 damage levels elemental damage.</th>
</tr>
<tr class="header">
<th>On demand elemental damage, free action, creature specific</th>
<th>Free action, on a hit: Spend a charge. +4 damage levels elemental damage. but only against one type of creature.</th>
<th>Free action on a hit: Spend two charges. +5 damage levels elemental damage. but only against one type of creature.</th>
<th>Free action on a hit: Spend four charges. +6 damage levels elemental damage. but only against one type of creature.</th>
</tr>
<tr class="odd">
<th>Wielding changes</th>
<th><strong>Free action: Wield or sheath this weapon.</strong></th>
<th><strong>Passive: Wielding the item does not take up a hand.</strong></th>
<th><strong>Passive: Weapon cannot be disarmed</strong></th>
</tr>
<tr class="header">
<th>Thrown weapon returning</th>
<th><p>Passive: Returns to your hand at the end of your next turn when thrown, or sheathes itself if your hand is not free.</p>
<p>or</p>
<p>Thrown (10ft/20ft)</p></th>
<th><p>Reaction, after resolving an attack: Thrown weapon returns immediately.</p>
<p>or</p>
<p>Add Thrown (10ft/20ft)</p></th>
<th><strong>Bonus action: Item returns to your free hand if it is within 300ft.</strong></th>
</tr>
<tr class="odd">
<th>Effective against special target</th>
<th>Passive: Weapon counts as silvered.</th>
<th>Passive: Weapon can deal damage to Ethereal targets.</th>
<th>Passive: For one damage type this weapon does, Immunity is downgraded to resistance.</th>
</tr>
<tr class="header">
<th>Melee reach extension</th>
<th>Free action: Spend a charge. Increase reach of the weapon by 10ft for the next attack.</th>
<th>Passive: Increase reach of weapon by 5ft.</th>
<th><strong>Reaction: Increase reach of the weapon by 10ft for the next attack.</strong></th>
</tr>
<tr class="odd">
<th>Ranged weapon increase</th>
<th><p>Passive: Ignore penalty for long range.</p>
<p>Gains Thrown (15/30) if a melee weapon.</p></th>
<th>+30ft/+60ft range. Gains Thrown (15/30) if a melee weapon.</th>
<th>Action: Spend 4 charges. A melee weapon you are holding gains Thrown (30/60). Make a ranged attack with that weapon.</th>
</tr>
<tr class="header">
<th>Range weapon adjacent target bonuses</th>
<th>Passive: No disadvantage for attacking adjacent targets.</th>
<th>Passive: Can make attacks of opportunity with this ranged weapon.</th>
<th>Passive: You may roll melee attack rolls with this melee weapon.</th>
</tr>
<tr class="odd">
<th>Attack of Opportunity changes</th>
<th>Free action: Spend two charges. Make an attack of opportunity without expending your reaction.</th>
<th>Reaction when a creature moves within 5ft of you: Spend a charge. Make an attack of opportunity against that creature.</th>
<th>Reaction: Spend 4 charges. Make an attack of opportunity against a disengaging target.</th>
</tr>
<tr class="header">
<th>Wounded target cannot heal</th>
<th>Passive: When you wound with this weapon, the target may not heal until your next turn begins.</th>
<th>Free action, When you wound with this weapon: Spend two charges. the target may not heal for the next 10 rounds.</th>
<th><strong>Reaction, When you wound with this weapon: Spend a charge, the target may not heal for the next 10 rounds.</strong></th>
</tr>
<tr class="odd">
<th>Heal on wound</th>
<th>Reaction, on a wounding hit: Spend a charge. Heal 2 damage level.</th>
<th>Free action, on a wounding hit: Spend two charges. Heal 2 damage level.</th>
<th>Passive: Heal 2 damage level when rolling a critical hit.</th>
</tr>
<tr class="header">
<th>Inventory changes</th>
<th><strong>Passive: Weapon size reduced to Tiny when sheathed.</strong></th>
<th><strong>Passive: Item weighs 0.5lb when sheathed.</strong></th>
<th><strong>Action: Item is sheathed to an extradimensional space or unsheathed from that space.</strong></th>
</tr>
<tr class="odd">
<th>Spend hit die for damage</th>
<th>Reaction when hitting a target: Spend a hit die to cause that much damage to the target. Damage must be of a type caused by this weapon.</th>
<th>Free action when hitting a target: Spend a charge. Spend a hit die to cause that much damage to the target. Damage must be of a type caused by this weapon.</th>
<th>Action: Spend 4 charges and as many hit dice as you want. The first attack that lands on your next turn causes additional damage equal to the hit dice used.</th>
</tr>
<tr class="header">
<th>Spend hit die for healing</th>
<th>Reaction when hitting a target: Spend a hit die to heal that much damage.</th>
<th>Free action when hitting a target: Spend a charge and a hit die to heal that much damage.</th>
<th>Ritual: Hit dice used for healing roll maximum if you expend one charge for each.</th>
</tr>
<tr class="odd">
<th>Change weapon Type</th>
<th>Bonus action: Spend 2 charges. Weapon changes into another weapon type, determined when the item is created.</th>
<th>Action: Weapon changes into another weapon type, determined when the item is created.</th>
<th>Ritual: Change the weapon into another type that you have seen before.</th>
</tr>
<tr class="header">
<th>Target must take test or suffer condition, effective</th>
<th>Free action on a hit: Spend a charge. Target takes a DC 13 saving throw or suffers level 1 condition for 1 minute. Test at end of turn to remove.</th>
<th>Reaction on a hit: Target takes a DC 13 saving throw or suffers level 1 condition for 1 minute. Test at end of turn to remove.</th>
<th>Bonus action: Spend a charge. The next attack that hits, Target takes a DC 15 saving throw or suffers level 1 condition for 1 minute. Test at end of turn to remove.</th>
</tr>
<tr class="odd">
<th>Target must take test or suffer condition, powerful</th>
<th>Free action on a hit: Spend a charge. Target takes a DC 10 saving throw or suffers level 2 condition for 1 minute. Test at end of turn to remove.</th>
<th>Reaction on a hit: Target takes a DC 10 saving throw or suffers level 2 condition for 1 minute. Test at end of turn to remove.</th>
<th>Bonus action: Spend a charge. The next attack that hits, Target takes a DC 12 saving throw or suffers level 2 condition for 1 minute. Test at end of turn to remove.</th>
</tr>
<tr class="header">
<th>Target must take test or suffer condition, sticky</th>
<th>Free action on a hit: Spend a charge. Target takes a DC 8 saving throw or suffers level 1 condition for 2 rounds. The condition cannot be removed before then.</th>
<th>Reaction on a hit: Target takes a DC 8 saving throw or suffers level 1 condition for 2 rounds. The condition cannot be removed before then.</th>
<th>Bonus action: Spend a charge. The next attack that hits, Target takes a DC 10 saving throw or suffers level 1 condition for 2 rounds. The condition cannot be removed before then.</th>
</tr>
<tr class="odd">
<th>Weapon Trait modification</th>
<th>Passive: Ignore the Loading trait of the weapon, or add the Versatile trait.</th>
<th>Passive: Ignore the Heavy trait of the weapon, or add the Light trait.</th>
<th>Passive: Add the Finesse trait to the weapon.</th>
</tr>
<tr class="header">
<th>Critical quality chance</th>
<th><strong>Free action: Once per turn, reroll a failed attack roll.</strong></th>
<th><strong>Passive: Reroll fumbled attack rolls once.</strong></th>
<th><strong>Passive: Causes critical hits on a 19 or 20.</strong></th>
</tr>
<tr class="odd">
<th>Effect on miss</th>
<th>Free action, after you miss with a strike: Spend a charge. Attacks made against you by that target are at disadvantage until the start of your next turn.</th>
<th><strong>Free action, after you miss with a strike: Gain +1 to hit and damage on the next strike which hits. When you deal damage, this bonus resets to zero.</strong></th>
<th>Reaction, after you miss with a strike: Gain advantage on the next attack roll you make with this weapon.</th>
</tr>
<tr class="header">
<th>Effect on kill</th>
<th>Free action, when you kill a target: Gain 1 damage levels of temporary hit points.</th>
<th>Reaction, when you kill a target: Regain 1 hit dice of your choice.</th>
<th><strong>Reaction, when you kill a target: Spend a charge. Gain 3 damage levels of temporary hit points.</strong></th>
</tr>
<tr class="odd">
<th>Normal weapon damage.</th>
<th>Free action: Spend one charge. The weapon damage is increased by three levels. If the weapon has the Versatile trait, it also increases by three levels.</th>
<th>Passive: The weapon damage is increased by two levels. If the weapon has the Versatile trait, it also increases by one level. The item gains the Heavy trait.</th>
<th>Free action: Spend two charges. The weapon damage is increased by six levels. If the weapon has the Versatile trait, it also increases by six levels.</th>
</tr>
<tr class="header">
<th>Effect when you dodge</th>
<th>Reaction, when a melee attack against you fails: Spend a charge. The target moves into your space and you move 5ft. Neither move provokes attacks of opportunity.</th>
<th><strong>Reaction, when an melee attack against you fails: Move 5ft without provoking attacks of opportunity.</strong></th>
<th><strong>Reaction, when an melee attack against you fails: Gain advantage on your next attack against the target.</strong></th>
</tr>
<tr class="odd">
<th>Backstab effects</th>
<th><strong>Passive: Reroll damage dice of 1 when attacking a target that cannot see you.</strong></th>
<th>Reaction, when you hit a target while hidden: Roll the damage twice and choose which result you want.</th>
<th>Reaction, when you hit a target while hidden: Swap all the damage done to one level 1 damage type.</th>
</tr>
<tr class="header">
<th>Disable special states</th>
<th>Reaction, when you hit a target with a melee weapon: DC 10 Strength saving throw or become disarmed.</th>
<th>Reaction, when you hit a target with a shield: The target cannot add the AC bonus for the shield until the start of its turn.</th>
<th>Reaction, when you hit a target that is immaterial: The target becomes solid until the start of its turn.</th>
</tr>
<tr class="odd">
<th>Action economy changes</th>
<th>Passive: You may make an offhand attack without taking the Attack action. Weapon gains the Light property.</th>
<th><strong>Passive: When you take the Dodge action, you may still make one attack roll with this weapon.</strong></th>
<th><strong>Free action, when you take the Dash action: Spend a charge. Make one attack roll with this weapon against a valid target.</strong></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

|                                     | **Armor Variant 1**                                                                               | **Armor Variant 2**                                                                                                                                    | **Armor Variant 3**                                                                                                                        |
|-------------------------------------|---------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| Action economy changes.             | Passive: When you take the Dodge action, you may still make one attack roll.                      | Action: Spend two charges: Take the Dash and Attack action this turn.                                                                                  | Free action: Spend 2 charges. Take the disengage action.                                                                                   |
| Reaction to Resistance              | Reaction when hit: Spend two charges. Resistance to one damage type until the start of your turn. | Reaction after taking elemental damage: Spend four charges. Resistance to one damage type until your next rest.                                        | Reaction when hit: Spend one charge. Resistance to one damage type for this hit.                                                           |
| Grapplers take damage               | Passive: Grapplers take +2 piercing damage level damage at the start of your turn.                | Passive: Grapplers take +1 elemental damage level damage at the start of your turn.                                                                    | Action: Grapplers take 3 levels of elemental damage.                                                                                       |
| Defence against Grapples and shoves | Passive: level 1 bonus against Shoves.                                                            | Passive: level 1 bonus against Grapples.                                                                                                               | Action: Spend a charge. Roll to escape a grapple with a level 3 bonus.                                                                     |
| Strength bonuses                    | Passive: level 2 bonus on all Str saves                                                           | Passive: Level 3 bonus on Strength tests to move objects.                                                                                              | Passive: Level 3 bonus on Constitution checks for exhaustion.                                                                              |
| Agility Bonuses                     | Passive: level 2 bonus on all Dex saves                                                           | Passive: level 3 bonus on saves to halve damage.                                                                                                       | Passive: Use a different attribute for saving throws to halve damage.                                                                      |
| Inventory changes                   | Passive: Double carrying capacity.                                                                | Bonus action: Don/Doff this armour.                                                                                                                    | Action: Don/Doff this armour to an extradimensional space.                                                                                 |
| Skill tests, situational            | Passive: level 3 bonus on checks for climbing.                                                    | Passive: level 3 bonus on checks for swimming.                                                                                                         | Passive: level 3 bonus on checks for jumping.                                                                                              |
| Stealth bonuses                     | Passive: Ignore stealth disadvantage of the armour                                                | Passive: Level 2 bonus to Stealth when in bright sunlight                                                                                              | Passive: Level 2 bonus to Stealth when in total darkness                                                                                   |
| Dangerous terrain bonus             | Passive: Resistance to one elemental damage from terrain.                                         | Passive: One type of Difficult terrain counts as normal.                                                                                               | Passive: level 3 bonus on checks for landing safely in dangerous terrain.                                                                  |
| AC bonus                            | Increases max Dex bonus by one level. None-\> +2, +2 -\> unlimited.                               | Passive: +1 AC when worn.                                                                                                                              | Reaction when hit: Spend a charge. +2 AC until the start of your turn.                                                                     |
| AC bonus, creature specific         | Reaction when hit by a specific creature type: Spend 2 charges. +5 AC to this hit.                | Passive: +2 AC against attacks by one creature type.                                                                                                   | Reaction when hit by a specific creature type: Spend a charge. +3 AC until the start of your turn against creatures of that specific type. |
| AC bonus, attack specific           | Passive: +2 AC against melee attack rolls                                                         | Passive: +2 AC against ranged attack rolls                                                                                                             | Passive: +2 AC against spell attack rolls                                                                                                  |
| Dodging                             | Passive: +1 AC against attacks by Fiends                                                          | Reaction after you take damage: Spend two charges. Take the disengage action and make an additional 5ft teleport.                                      | Action: Spend a charge. You may cast the Shield spell against the next appropriate attack without expending a spell slot.                  |
| Wielding changes                    | Free action: Drink a potion you have in your inventory without needing a free hand.               | Free action: Spend a charge. Swap the item in your hand with another that you have on you.                                                             | Bonus action: Retrieve a thrown weapon that you can see within 60ft. It comes to your hand or sheaths itself, your choice.                 |
| Reaction, retaliate                 | Reaction when hit by a melee attack: Spend a charge. Make a shove action against the target.      | Reaction when hit by a melee attack: Spend a charge. Make a grapple action against the target.                                                         | Reaction when hit by a ranged attack: Spend a charge. Make a single ranged attack against that target.                                     |
| Buy healing                         | Free action: Spend 1 charge and a hit die. Regain the amount rolled in hitpoints.                 | Bonus action: Spend 1 charge and a hit die. Gain triple the amount rolled in temporary hit points.                                                     | Reaction, when you take damage: Spend a charge. Half the damage taken is added as temporary hit points.                                    |
| Healing bonuses                     | Reaction: when you gain hitpoints, gain an additional 2 levels of healing                         | Reaction: when you gain hitpoints, gain 3 levels of temporary hit points.                                                                              | Passive: when you gain hitpoints, gain an additional 1 levels of healing                                                                   |
| Protection from movement            | Passive: When you use the Dash action, your speed cannot be reduced by any means.                 | Passive: You cannot be moved unwillingly by non-magical means.                                                                                         | Reaction: Spend a charge. Prevent an unwilling move by any means.                                                                          |
| Protection from critical hits       | Free action when hit crically. Spend one charge. Downgrade the hit to a regular hit.              | Free action when hit crically. Spend two charges. Ignore the hit completely.                                                                           | Reaction, when hit critically: Ignore the hit completely. You gain the Petrified condition until the end of your turn.                     |
| Protection from conditions          | Passive: You cannot unwillingly gain a level 1 condition.                                         | Reaction, when you gain a condition: Spend 4 charges. Lose that condition.                                                                             | Action: Spend 2 charges. Remove one level 2 condition condition.                                                                           |
| Condition charge up                 | Passive: Deal an extra 1 damage level damage for each condition affecting you.                    | Reaction when a creature you can see gains a condition that you are not currently suffering from: Spend 1 charge. Transfer that condition to yourself. |                                                                                                                                            |
| Movement speed                      | Passive: Double jump distances                                                                    | Passive: +10ft walking speed.                                                                                                                          | Free action: Spend 2 charges. +20ft movement speed for 1 minute.                                                                           |
| Protection from Death               | Passive: Critical success on death saving throws if you roll a 19 or 20.                          | Passive: level 1 bonus on death saving throws.                                                                                                         | Passive: When you make a death saving throw you must roll a hit die if you can. The result is added to the saving throw.                   |
| Usable Cantrips                     | Passive: Item provides 1 level 1 spell slot.                                                      | Passive: Learn one cantrip while wearing this armour.                                                                                                  | Free action: Spend a charge. Use one of two cantrips                                                                                       |
| Protection from spells              | Passive: level 1 bonus to all saves against magic.                                                | Passive: Ignore the effects of one spell you have seen, chosen when attuning to the armour.                                                            | Passive: Ignore the effects of two spells you know, chosen when attuning to the armour.                                                    |

|     | **Penalty Effect (has charges)**                                                                                   | **Penalty Effect (no charges)**                                                                  |
|-----|--------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| 1   | **Lazy**: Roll for each charge when recharging. 50% it recharges.                                                  | **Fickle**: Active effect fails on a 6. Roll for Passive effects after each Long Rest.           |
| 2   | **Picky:** Spending charges on the same effect twice in a row costs an extra charge.                               | **Bored:** Passive effects stop working if you stand still.                                      |
| 3   | **Draining**: Being attuned to the item when it recharges causes an Exhaustion level.                              | **Draining:** Attuning or reattuning to the item causes a level of Exhaustion.                   |
| 4   | **Hollow:** When the last charge is spent, roll a d10. On a 1, the item turns to dust. If the item has no charges, | **Fragile:** roll a d20 every time a bonus is invoked. On a 1 the item turns to dust.            |
| 5   | **Jealous:** You may only attune to one jealous item at a time.                                                    |                                                                                                  |
| 6   | **Hungry:** Each charge requires materials with a value of 50g to recharge.                                        | **Greedy:** You must spend 50g of materials during each long rest to keep the effects available. |
|     |                                                                                                                    | **Shy:** Attuning to the item does not reveal its properties.                                    |

<table>
<colgroup>
<col style="width: 13%" />
<col style="width: 43%" />
<col style="width: 43%" />
</colgroup>
<thead>
<tr class="header">
<th></th>
<th><strong>Bonus Effect (has charges)</strong></th>
<th><strong>Bonus Effect (no charges)</strong></th>
</tr>
<tr class="odd">
<th>1</th>
<th><p>Add 8 more charges. Roll an extra Penalty.</p>
<p>Reroll if the item already has a Penalty.</p></th>
<th><p>Roll another effect and power goes up 1. Roll an extra Penalty.</p>
<p>Reroll if the item already has a Penalty.</p></th>
</tr>
<tr class="header">
<th>2-3</th>
<th>Add 4 more charges.</th>
<th>Roll another effect.</th>
</tr>
<tr class="odd">
<th>4-6</th>
<th>Power: Item level goes up 1</th>
<th>Power: Item level goes up 1</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

**Examples**

**Hoardfrost. Uncommon Handaxe. 200gp**

Reaction on a hit: +d6 damage levels cold damage.

Cast either the Frostbite or Gust cantrip once per day.

Greedy: You must spend 50g of materials during each long rest to keep the effects available.

**Weavepouch. Uncommon Satchel (Medium, Worn). 250gp.**

Stores one level 1 spell.

Drains at the start of any long rest. Anyone can store. Attuned can cast as if they were the storer.

Ritual: Change the items form into one other type of the same size (eg// belt, cloak, hat, shoes).

**Personality (Fragile)** Roll a d20 every time Spell is used. On a 1 the item turns to dust.

Armour of Knotted Sinew. Uncommon Studded leather. 245gp

Passive: +d4 bonus on all Strength saving throws.

Ritual: Change the item into a cloak or back into a Studded leather armour.

**Personality (Bored)** Passive effects stop working if you didn’t move last round.

**Orcvenom Sword. Uncommon longsword 215gp**

Passive: +d6 poison against Orcs.

**Periapt of Effective rest. Uncommon amulet. 400gp.**

Passive: Reroll any spent hit dice once per dice.

**Swashbucklers Leathers. Uncommon Padded Leather, 245gp**

Passive: When you take the Dodge action, you may still make one attack roll.

**Voidlever. Rare Maul. 2000gp**

Passive: The weapon damage increases to 3d6.

Bonus Action: Item is sheathed to an extradimensional space or unsheathed from that space.

**Charged Ring of Suffering. Rare ring, 2200gp**

Passive: Creatures already under the effect of one of your spells suffer a d4 penalty to their Saving throws from spells you cast.

Reaction when you cast a spell: Spend one charge. Spend a spell slot three levels lower than the cast spell.

2 charges.

**Stablemind. Rare Breastplate. 2400gp**

Free action: Spend 1 charge and a hit die. Regain the amount rolled in hitpoints.

Action: Spend 2 charges. Remove the Charmed condition from yourself.

**Personality (Lazy)** Roll for each charge when recharging. 50% it recharges.

12 charges.

**Paincensor. Rare Flail, 2000gp**

Reaction: Weapon gains Reach(15ft) for the next attack.

Passive: When you wound with this weapon, the target may not heal until your next turn begins.

Free action on a hit against a Humanoid: Spend a charge. Cause an extra d10 Acid damage.

Has 1 charge max.

**Cloak of Dessication. Rare cloak (medium, worn), 2000gp**

Passive: Immunity to fire damage caused by the environment.

Bonus action: Spend 1 charges, Roll any number of hit dice and suffer that much fire damage. Recharge spell slots with value equal to the dice used +2.

1 charge max.

**Verdantbend. Rare Padded leather, 2000gp**

Passive: +d4 to all saving throws against magic.

Reaction, when you gain hitpoints: Gain an additional d6 hit points

Other item ideas

**Attunement**

Eyes of Minute seeing

Goggles of night

Gem of Brightness

Glamoured Armor

Shapeshifting Weapon

Immovable rod

Shield of Missile attraction

Chime of Opening.

Brooch of Rebuffing. Automatic pass first charm attempt per week.

**Non-attunement**

Decanter of endless water

Pot of Porridge. 10 servings of hot Porridge per day. 10 days for 1 silver.

Quill tokens

Driftorb

Folding Boat

1d4 balls of silence in a bag
