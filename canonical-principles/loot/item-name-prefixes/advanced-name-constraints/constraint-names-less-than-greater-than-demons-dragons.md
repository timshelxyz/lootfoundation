# Constraint: Names<>Demons/Dragons

## **Each of lores A, B and C contain among their namePrefixes the name of a mythical creature:**

* Lore A: Dragon (also referenced as an adjective in some loot items: Dragonskin and Dragon's)
* Lore B: Demon (also referenced as an adjective in some loot items: Demonhide and Demon's)
* Lore C: Phoenix

## **Named items partition in two groups:**&#x20;

The implementation of "names"  in the contract has two direct consequences on names actually generated:

* Half the combinations of namePrefixes and nameSuffixes are impossible (when the index is an odd number for namePrefixes for example, it cannot be both odd and even fo nameSuffixes), hence the 276 combinations out of 552 observed in OG loot items
* The possible combinations part in two separate groups: those when the initial random number is odd and those when it is even.

## **All "named" items partition evenly in Demon and Dragon groups**

By crossing the Demon and Dragon groups of names with the item "name" prefixes, we observe that for each item type (e.g. weapon, chest, head, etc.), for each item class (e.g. hunter, etc.), items partition between Demon and Dragon groups.&#x20;

## **Demon and Dragon are split into two groups:**

| Prefixes \ Suffixes | Bender-Bite-Peak-Grasp-Moon-Shout | Roar-Sun-Whisper-Glow-Root-Tear |
| ------------------- | --------------------------------- | ------------------------------- |
| Demon group         | 3100                              | 0                               |
| Dragon group        | 0                                 | 2957                            |

We observe that half the namePrefixes and half the nameSuffixes actually generated relate to a group containing the Demon namePrefix, the other halves to a group containing the Dragon namePrefix (and the third, undiscovered for now, to a group containing the Phoenix namePrefix).

## For example for Chest items:

| Character Class | Items that can get "Demon" in their name Prefix | Items that can get "Dragon" in their name Prefix |
| --------------- | ----------------------------------------------- | ------------------------------------------------ |
| **Hunter**      | Demon Husk, Hard Leather Armor                  | Studded Leather Armor                            |
| **Warrior**     | Ornate Chestplate, Ring Mail                    | Holy Chestplate, Chain Mail                      |
| **Mage**        | Linen Robe                                      | Silk Robe, Shirt                                 |
