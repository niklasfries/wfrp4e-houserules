# Houserules Main Document

## Combat

### Tests

In combat, opposed tests are replaced with a "player rolls" system, which now also applies to ranged attacks. Additionally, skills are replaced with **Attack Skill Bonuses** (ASBs) and **Defence Skill Bonuses** (DSBs). ASBs are the skill used for the attack divided by 10 and rounded down. There are three types of DSBs, which are computed the same way, and have the following uses:

* **Melee Defence Bonus:** Computed from the relevant Melee Skill. Used to oppose Melee attacks, or Ranged attacks if you have a Shield with rating at least 2.
* **Dodge Defence Bonus:** Computed from the Dodge Skill. Used to oppose Melee and Ranged attacks, and Spells with the Magic Missile property.
* **Spell Defence Bonus: **Computed from the Willpower Characteristic. Used to oppose Spells including those with the Magic Missile property.

If multiple DSBs apply, the defender may choose which one to use.

The result of the test is computed as follows:

1. The player rolls a D20 and a D100, where the D20 is used to determine hits and the D100 is used to determine Critical Hits and Hit Location.
2. The player computes the **Player SL** (PSL) by taking the relevant ASB or DSB, adding 10, and subtracting the D20 value.
3. The **Enemy SL** (ESL) is the relevant ASB or DSB of the enemy.
4. The **Opposed SL** (OSL) is the attacker SL minus the defender SL, and the attack hits if the OSL is greater than 0. If the OSL is 0, whoever rolled wins the test.
5. If the D20 roll was 1 or 20, the player wins or loses the test by at least 0 OSL, respectively. Additionally, if the roll was 1 or 20 and the attack misses, the attack is also a Fumble.
6. If the D100 roll was a double and the attack was a hit, the attack is also a Critical Hit.
7. The straight D100 value is used to determine hit location.

For PvP and EvE, treat the computation as if the attacker is the player.

*Example: Anders attacks an orc. His Melee Skill is 63, which means his effective ASB is 6. The orc defends with its Melee skill of 47, which means the DSB is 4. Anders rolls 11 on the D20 and 53 on the D100. The PSL is PSL + 10 - D20 = 6 + 10 - 11 = 5, and the OSL is PSL - ESL = 5 - 4 = 1. This means the attack hits with 1 SL, and the hit location is 53 which is the ork's body.*

### Defenceless

A Defenceless character cannot have a DSB higher than 0. Blinded, Prone, Stunned and Surprised targets are Defenceless against Ranged Attacks, as are targets that cannot clearly see the attacker. Unconscious targets are Defenceless against all Attacks. Defenceless targets cannot benefit from Shields.

### Spells

Spell casting is separated into two Tests: a Language (Magick) Test to determine whether the spell is successfully cast, and an attack test to determine if the spell hits. The attack test is performed as for mundane attacks, but does not affect spell damage.

1. The spellcaster performs an Unopposed Language (Magick) Test, modified by -10 for each effective CN of the spell. The spell is successfully cast if the Test is successful.
    1. Any counterspelling attempt is performed as an Opposed Test to this Language (Magick) Test. Note that this Opposed Test is resolved with two separate D100 rolls.
2. Any Overcast effects are chosen, including additional targets.
3. If the spell is successfully cast, the spellcaster nominates targets and performs an attack against each target. The ASB is based on the Language (Magick) Bonus of the spell caster, modified by the SL of the Language (Magick) Test in step 1. The DSB is based on Dodge or Willpower for Magic Missiles, and Willpower for all other spells.
    2. Willing targets are automatically hit. Targets with the Magic Resistance Talent may never be willing targets, and must oppose the cast with their Spell Defence Bonus if it is higher than their Dodge Defence Bonus.
    3. Unconscious targets may only defend with Willpower, but do not count as Defenceless.

*Example: Günther has 80 Language (Magick) and casts Bolt with CN 4. He rolls 23, which is 2 SL after CN, and adds 1 target and 1 damage (WoM p. 23). Next, he rolls to attack the two targets: The first roll is 12, for a PSL of ASB + SL + 10 - D20 = 8 + 2 + 10 - 12 = 8. The second roll is a 15, for a PSL of 5. The first target defends with its DDB of 6, and the second target with its SDB of 4. Both targets are hit, and since Günther has 5 WPB, they both take 10 Damage.*

### Other opposed Tests [Changed, försök komma ihåg och fundera på igen]

In combat, opposed tests are resolved the same way as Attacks, i.e. a Skill Bonus is derived from the Skills used by the attacker and defender, and the result is resolved with a D20 roll.

*Example: Aaron tries to stun an orc boy with the Strike to Stun Talent. After having hit the orc in the head, they resolve an Opposed Strength/Endurance Test. For this test, their effective Skills are 70 and 60, respectively. Aaron rolls a 9, and the Opposed SL of the Test is ASB - DSB + 10 - D20 = 7 - 6 + 10 - 9 = 2. This means Aaron won the Opposed Test with 2 SLs, and the orc receives a Stunned condition.*

### Advantage and Disadvantage

Combat difficulty modifiers no longer apply. Instead, various situations give **Advantage **or **Disadvantage **to a Test. If a Player has Advantage on a Test, they roll the D20 twice and pick result. If they have Disadvantage, they roll twice and pick the worst result (or GM picks). If they have neither or both, they roll only once. If an Enemy has Advantage or Disadvantage on a Test, the Player gains Disadvantage or Advantage, respectively.

| Advantage                                                                 | Disadvantage                                                                                                                                                                                                                              |
|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| - Shooting at Point Blank Range: at most 10% of the weapon range.         | - Shooting at Long Range: up to double weapon range.                                                                                                                                                                                     |
| - Shooting a target that's Large or larger.                               | - Shooting a target in medium cover, or a target concealed by darkness or weather.                                                                                                                                                       |
| - Melee attacks against an opponent you outnumber at least 2 to 1.        | - Shooting a rapidly moving target, e.g., riding or flying.                                                                                                                                                                              |
| - Shooting when you spent your last Action aiming.                        | - Shooting a target that's Little or smaller.                                                                                                                                                                                            |
| - Defending with a skill you went Defensive with as your last Action.     | - Called shot to a specific hit location.                                                                                                                                                                                                |
|                                                                           | - Attacking with a weapon in your off-hand is -2 SLs.                                                                                                                                                                                     |
|                                                                           | - Close combat in darkness, weather, or arduous terrain (if both attacker and defender are hampered, neither gets disadvantage).                                                                                                          |
|                                                                           | - Attacking while having the Blinded or Prone condition.                                                                                                                                                                                  |
|                                                                           | - Defending against Melee attacks when affected by the Blinded, Broken, Entangled, Prone, Surprised, or Stunned conditions.                                                                                                               |
|                                                                           | - Using a Melee skill to defend against a Melee attack from a target at least two steps larger.                                                                                                                                           |
|                                                                           | - Attacking with a weapon you are not allowed to use according to vanilla. Note that you can never gain Advantage while getting Disadvantage for this reason, so the roll will always be at Disadvantage unless you spend a Fortune Point. |

Fortune points are combined with Advantage and Disadvantage according to the following table:

| Advantage or Disadvantage? | Roll?                           |
|----------------------------|---------------------------------|
| Neither                    | Roll D20 twice, pick result.   |
| Advantage                  | Roll D20 thrice, pick result.  |
| Disadvantage               | Roll D20 once.                |
| Both                       | Roll D20 twice, pick result.   |

Note that the GM can override any Advantage/Disadvantage computation in special circumstances.

### Grappling [TODO]

### Weapon Length and In-fighting [Changed]

Weapon Lengths do not confer any combat difficulty modifiers. In-fighting only applies when at least one combatant has the Talent In-fighter.

### Momentum [formerly known as Advantage]

Advantages are replaced with Momentum, which works as follows. In combat, you gain one Momentum whenever:

* You perform a Charge.
* You win an Opposed Test you initiated against an enemy combatant.
* You inflict Damage on an enemy combatant, or give an enemy combatant a Condition.
* You assess the situation, using e.g. Leadership, Intuition or Perception to acquire a tactical advantage. This Test must achieve something concrete, e.g., you learn something about the situation, or rally a Broken ally. TODO kom ihåg (This action may generate more than 1 Momentum, depending on the amount of snacks fed to the GM.)

You can only gain a single Momentum per Action, typically designated by a separate Test. You no longer lose Momentum whenever you lose an Opposed Test or take damage, but you still lose 1 Momentum at the end of your Turn if you didn't earn a Momentum on your Turn.

When you perform an Attack, you may spend Momentum to gain a skill bonus of +10 to your attacking skill per spent Momentum. You may also spend momentum to Disengage, see Disengaging.

Momentum can also be used to gain the temporary benefit of some Talents. On your turn, you can spend your Move, your Action, and 2 Momentum to use the active component of one of the following Talents, but with 0 levels:

* Disarm.
* Dual Wielder.
* Strike to Stun.
* TODO fler

#### Actions with Momentum [TODO]

* knuffas

### Sprinting

During combat, you may use your Action to move as if you had two Moves.

### Disengaging [Changed]

If you Walk or Run out of the Weapon Reach of a hostile character, this character may perform a free Melee Attack against you, opposed with Dodge. If the attack hits, you take Damage as normal and are forced to remain within the reach of the attacker's weapon. A character may only perform such an attack once per Round, and never with a Slow weapon.

For your Action, you may instead attempt to Dodge out of combat. This works the same way, but if you lose the Opposed Test you do not take a Melee hit.

You may also use your Move to move your Movement Rating (3 for dwarfs and halflings, 4 for humans, 5 for elves) away from an opponent without them being able to stop you. However, you still count as Engaged with this opponent until the end of their next Turn. TODO utvärdera

Finally, if you have more Momentum than every Engaged opponent, you may spend all of them to be able to Move out of Weapon Reach without risking an attack.

### Zones of Control [Changed]

Once per Round, if someone passes you close enough that you can reach them with a drawn melee weapon that does not have the Slow property, you may attack them for free. If you hit, you deal damage as normal, and they have to stop where they were when you hit them. Note that larger targets usually ignore Zones of Control.

### Fortune Points

Your three options are:

* Spend a Fortune Point before a test to be able to make it twice and pick the result. For Opposed Tests in combat, see Advantage and Disadvantage.
* Spend any number of Fortune Points before an Unopposed Test to gain a bonus of +10 for each, or before an Opposed test to gain a bonus of +1 SL for each.
* At the start of the Round, choose when to act in that Round, disregarding Initiative order.

Fortune and Resolve points are restored by 1 at the start of each session, and fully restored at the start of each story arc. Luck and Strong-minded increases replenishment by 1.

### Swapping weapons [Changed]

Drawing or sheathing a weapon or shield can be done once per turn as a Free Action. Any more swapping will normally require either a Move or an Action. Dropping a held item can be done any number of times. Picking up an item from the ground counts as an Action.

### Critical Wounds [TODO]

## Conditions

#### Ablaze [Changed]

When you first act in a Round, if you have any Ablaze Conditions, perform a (+0) Cool Test with -10 for each Ablaze Condition. If you fail, you must use your Action to attempt to remove the Ablaze Conditions. If you fail the test by at least 6 SLs, you also gain a Broken Condition, although your Action must still be used to remove the Ablaze Conditions.

One Ablaze Condition can be removed with a successful Athletics Test, with each SL removing an extra Ablaze Condition. The Difficulty for this Test is modified by circumstances: it’s much easier to put out a fire rolling around on sand than it is in the middle of an oil-soaked kitchen.

At the end of your Turn, lose 1d10 Wounds plus 1 for each Ablaze Condition, modified by Toughness and Armor Points. If you end your Turn with 0 Wounds, consult the Deadly Conditions section.

#### Bleeding [Changed]

At the end of your Turn Lose 1 Wound for every Bleeding Condition. Next, perform a (+0) Endurance Test modified by -10 for each Bleeding Condition, and remove 1 Bleeding on Success. If you end your Turn with 0 Wounds, consult the Deadly Conditions section.

A Bleeding Condition can be removed with a successful Average (+20) Heal Test, with each SL removing an extra Bleeding Condition, or with any spell or prayer that heals Wounds, with 1 Bleeding Condition removed per Wound healed. Also see the rules for Bandages on WFRP, page 309.

Whenever you are exposed to Festering Wounds, Minor Infection, or Blood Rot, you suffer a penalty of –10 to any Tests to resist for each Bleeding Condition (WFRP, page 186).

(Mostly the same as UiA p80.)

#### Blinded [Changed]

You suffer a –10 penalty to all Unopposed Tests involving sight, gain *Disadvantage* when attacking, *Disadvantage* when defending against Melee Attacks, and count as Defenceless against Ranged Attacks.

One Blinded Condition is removed at the end of every Round.

#### Broken [Changed]

You get *Disadvantage* when defending against Melee attacks. On your turn, your Move and Action must be used to run away as fast as possible until you are in a good hiding place beyond the sight of any enemy; then you can use your Action on a Skill that allows you to hide more effectively. 

You cannot Test to rally from being Broken if you are Engaged with an enemy (see page 159). If you are unengaged, at the end of each Round, you may attempt a Cool Test to remove a Broken Condition, with each SL removing an extra Broken Condition, and the Difficulty determined by the circumstances you currently find yourself: it is much easier to rally when hiding behind a barrel down an alleyway far from danger (Average +20) than it is when three steps from a slavering Daemon screaming for your blood (Very Hard –30). 

If you spend a full Round in hiding out of line-of-sight of any enemy, you remove 1 Broken Condition.

#### Deafened [Changed]

You suffer a –10 penalty to all Unopposed Tests involving hearing, and gain *Disadvantage* when countering spells.

One Deafened Condition is removed at the end of every Round.

#### Entangled [Changed]

On your turn, you may not Move, and all your Unopposed Tests involving movement of any kind suffer a penalty of –10. You suffer *Disadvantage* when defending. 

For your Action, you can remove an Entangled Condition if you win an Opposed Strength Test against the source of the entanglement, with each SL removing an extra Entangled Condition.

If you are one step larger than the source of the Entangle condition, you may attempt to remove the Entangle with your Move. If you are at least two steps larger, you may attempt to do so as a Free Action.

#### Fatigued [Changed]

You suffer a -10 penalty to all Tests, and all Combat Skill Bonuses are reduced by 1 for every Fatigued Condition. 

#### Poisoned [Changed]

At the end of your Turn, you lose Wounds equal to your number of Poisoned Conditions. Next, perform a Challenging (+0) Endurance Test modified by -10 for each Poisoned Condition, and remove 1 Poisoned Condition on Success. If you end your Turn with 0 Wounds, consult the Deadly Conditions section.

#### Prone [Changed]

On your turn, your Move can only be used to stand up or crawl at half your Movement in yards (note: if you have 0 Wounds remaining, you can only crawl). You suffer a –20 penalty to all Unopposed Tests involving movement of any kind, and gain *Disadvantage* when attacking, *Disadvantage* when defending against Melee Attacks, and count as Defenceless against Ranged Attacks.

#### Stunned [Changed]

You are incapable of taking an Action on your turn and are only capable of half your normal movement. You get  *Disadvantage* when defending against Melee Attacks, count as Defenceless against Ranged Attacks, and may not counter spells.

At the end of each Round, you may attempt a Challenging (+0) Endurance Test. If successful, remove a Stunned Condition, with each SL removing an extra Stunned Condition.

#### Surprised [Changed]

You do not get to act on your Turn, gain *Disadvantage* when defending against Melee Attacks, and count as Defenceless against Ranged Attacks. You lose the Surprised Condition at the end of the Round.

#### Unconscious [Changed]

You can do nothing on your Turn and are completely unaware of your surroundings. You are Defenceless. You are Defenceless when defending against Melee attacks; or, if the GM prefers, any Melee hit simply kills you.

#### Deadly Conditions [New]

If you end your turn with any Deadly Conditions (Ablaze, Bleeding, Poisoned) and 0 Wounds, make a Challenging (+0) Endurance Test, modified by -10 per Deadly Condition, and receive the Unconscious Condition upon Failure. If you end your turn with the Unconscious Condition and any Deadly Conditions, you have a 10 % chance of dying per Deadly Condition. For example, if you have 1 Ablaze and 2 Bleeding, you would die on a roll of 71-100 on a D100.

## Weapon Properties

#### Accurate

Same as book (p. 297).

#### Blackpowder [Changed]

Same as book (p. 297).

Attacks with Blackpowder weapons cannot be opposed with Dodge or standard shields, i.e., the defender counts as being Defenceless with a DSB of at most 0.

#### Blast (Rating)

Same as book (p. 297).

#### Damaging

Same as book (p. 297).

#### Defensive [Changed]

Your Melee Defence Bonus is increased by 1 if you defend yourself with an item with this property. Multiple sources of Defensive do not stack.

#### Distract

Same as book (p. 297).

#### Entangle

Same as book (p. 297).

#### Fast [Changed**]**

Every Round, you may spend your Action to perform a Melee Attack with this weapon outside the normal Turn order. You may not perform this Attack during another character's Turn.

#### Hack [Changed]

As your Action, you may target the opponent’s shield. Perform a Melee Attack, if you win the opposed test you reduce the rating of the opponent’s shield with 1, plus 1 for every 3 SL of the Opposed Test. This attack does no damage to the opponent.

#### Impact

Same as book (p. 297).

#### Impale

Same as book (p. 297).

#### Penetrating [Changed]

This weapon ignores half of non-magical Armor Points, rounded up.

#### Pistol

Same as book (p. 297).

#### Precise [Changed]

(Ta bort, öka damage med 1.)

#### Pummel [Changed]

If you score a Head hit with a Pummel weapon, attempt an Opposed Strength/Endurance test against the struck opponent, modified by the Opposed SL of the Attack. If you win the test, your opponent gains a Stunned Condition.

#### Repeater (Rating)

Same as book (p. 297).

#### Shield (Rating) [Changed]

Same as book (p. 298).

Standard shields cannot be used to oppose Blackpowder weapons i.e., the defender counts as being Defenceless. Defenceless targets cannot benefit from Shields.

#### Trap Blade [TODO]

#### Unbreakable

Same as book (p. 297).

#### Wrap [Changed]

If an attack with this weapon hits and the unit die is a 0, the attack hits the head location.

#### Dangerous

Same as book (p. 299).

#### Imprecise [Removed]

#### Reload (Rating) 

Same as book (p. 299).

#### Slow [Changed]

You always act last in a Round. If multiple characters have a weapon with the Slow property, their internal Turn order is resolved as normal.

#### Tiring

Same as book (p. 299).

#### Undamaging

Same as book (p. 299).

#### Long [New for two-handed spears, pikes]

This weapon is long enough to hit large, fast-moving targets in melee. You may attack Disengaging enemies even if they are larger than you, but you may not prevent them from Disengaging.

#### Hook [New for halberds]

Once per Round, when a mount with a rider no larger than you Disengages, you may attack the rider as per the regular Disengaging rules. If you hit, you may perform an Opposed Strength Test modified by the Opposed SL of the attack. If you win, you pull the rider off the mount, the mount keeps moving, and the rider takes fall damage and becomes Prone.

Additionally, Hook allows you to use the Disarm Talent against foes one step larger than you.

#### Brace [New for two-handed spears, pikes, halberds]

You may use your Action to Brace until the beginning of your next Turn. If you do, and you get Charged by an enemy larger than you, during the Charge you count as having one extra level of the Reaction Strike Talent against the larger enemy, and your weapon gains the Damaging quality. If it already has Damaging, replace it with Impact. You may only benefit from Brace once per Round.

Note that if you already have the Reaction Strike Talent, you may target the rider of a mount that's larger than you, even if the rider is not. In this case, you don't get an extra level in Reaction Stike, but you still get the bonus damage.

## Armor Properties

#### Flexible

Same as book (p.300).

#### Impenetrable [Changed]

You ignore the Impale quality for hits on locations where you have armor with the Impenetrable property.

#### Partial [Changed]

Armor with this property has its AP reduced by 1 (Mail Coif, Open Helm).

#### Weakpoints [Removed]

## Craftsmanship

#### Practical/Unreliable [Removed]

## Creature Traits

#### Champion (Rating)

Same as book (p. 338). A creature can only deal damage this way Rating times per Round.

#### Size [TODO]

Vill vi göra steget mellan Large och Enormous lite mindre, antingen göra Large farligare eller Enormous lite mindre farligt?

Note: RAW har Enormous både Damaging och Impact och dubbel damage mot Average, det har vi aldrig spelat med vad jag minns.

eeemil verkar planera att spela en karaktär med Small, vilket gör detta extra intressant

## Endeavors

### Unusual Learning

Experience Points are only deducted on Success, and the test will Typically be Average (+20).

## Multiclassing

A character has a *Primary Career Tier*, which is used to determine Status, and Trappings required for that Status. Additionally, a character will have any number of *Implicit Career Tiers* if the following requirements are fulfilled:

* The character would be considered to have completed the Career Tier, i.e., it has 5/10/15/20 advances in 8 skills from that Career Tier or previous ones for Tiers 1/2/3/4, and one Talent from each of the current and previous Career Tiers.
* The character could be considered to belong to the Career Tier for narrative purposes, e.g., the character performed tasks similar to what a character in that Career Tier would do.

*Example: Jürgen is a Tier 2 Hunter, and has 10 advances in Charm Animal, Climb, Endurance, Outdoor Survival, Perception, Ranged (Bow), Melee (Basic) and Stealth (Rural). In addition, he has the Rover and Seasoned Traveller Talents. This means that he would have completed Tier 2 of Scout if he belonged to that Career. Since Jürgen used his Hunter skills for scouting purposes, he has Tier 2 of Scout as an Implicit Career Tier, and gets access to all Talents accessible by someone who belongs to that Career Tier.*

A character can advance

* any Characteristic;
* any Skill or Talent accessible to characters belonging to the Primary Career Tier, or any Implicit Career Tier of that character;
* any Skill they used during the last session.

Note that characters may advance Talents from previous Career Tiers.

During downtime, a character can change their Primary Career Tier to any Career Tier if:

* the new Career Tier can be considered an Implicit Career Tier for the character,
* or the new Career Tier is the first tier of a Career,
* and the new Career is a fit for the character for narrative purposes.

TODO with the amount of endeavors available maybe use RAW endeavor for career change?

*Example: Günther has completed Squire, i.e. the first tier of Knight, and would want to advance to the second tier: Knight. But he is not allowed to do so since he has not yet proven himself in battle, and thus his peers would not consider him a proper Knight. On the other hand, he can change career to Recruit, i.e. the first tier of Soldier, since the army is happy to take in anyone they don't have to train from scratch.*

If a character has completed their Primary Career Tier, they can advance to the next Career Tier as normal for 100 experience points (see book, p. 48-49).

## Value point Skills

For Lores and Languages, the number of SLs cannot exceed the number of Advances in the Skill divided by 5, rounded down. So with 30 Int 10 Lore (Reikland) A roll of 12 yields 2 SLs, while with 35 Int 5 Lore (Reikland) the same roll yields 1 SL. The number of SLs achieved represent the amount of information recalled, with a low SL providing only the most superficial knowledge or conveyed information. For an auto success, i.e. a toll of 01-05, SLs are computed as normal.

#### Other Intermediary Skills [TODO]

* **Drive:** "Under normal circumstances, if you possess the Drive Skill, there is no need to Test."
* **Melee:** "If you use a weapon from a Group where you have no Advances, you Test your Weapon Skill to hit with the weapon. While you still suffer all the weapon’s Flaws, you cannot use any of its Qualities."
* **Navigation:** "Possessing the Navigation Skill means you know roughly where you are, and can find your way between well-known landmarks without a Test."
* **Ride:** "You’ll only need to make a Test when doing something out of the ordinary, such as racing, dressage, traversing dangerous terrain, or charging into combat. Otherwise, if you have at least one Advance in the Skill, you are presumed to be able to ride around without need of a Test."
* **Row:** "Anyone with the Skill is automatically presumed to be able to scull about a pond, or over a gentle river, without a Test."

#### Advanced Skills

|                     |                |                   |
|---------------------|----------------|-------------------|
| - Animal Care       | - Pick Lock    | - Secret Signs    |
| - Animal Training   | - Play         | - Set Trap        |
| - Channelling       | - Pray         | - Sleight of Hand |
| - Evaluate          | - Ranged       | - Swim            |
| - Heal              | - Research     | - Track           |
| - Perform           | - Sail         | - Trade           |



