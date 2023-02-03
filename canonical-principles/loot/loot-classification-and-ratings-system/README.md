# Loot Classification & Ratings System

In the following pages, we present a detailed look at the hidden classification and ratings system derived from the original Loot contract.  A summary is presented first below. &#x20;

{% hint style="success" %}
All of the statistics below can be evaluated at the item-level, or summed up to the bag level.
{% endhint %}

## Each item in a Loot bag has:

* **A** [**`Greatness`**](greatness.md) **score:**&#x20;
  * This is an evenly distributed random number from 0-20
  * In the code, this determines whether the item gets an Order appended at Greatness 15 ("Of \_\_\_"), and then a Name Prefix prepended at Greatness 19, and then a "+1" appended at Greatness 20. \

* **An** [**`Item Type`**](item-types.md)**:**
  * For Weapons — Bludgeons, Blades, Books and Wands
  * For Armor — Metal, Hide, Cloth\

* **A** [**`Specialty`**](character-classes-specialties/) **(known as "Character Class")**
  * These specialities map the item types, and fit into 3 groups.
  * The community has adopted three groups to define these three specialties: "[Warriors, Hunters & Mages](character-classes-specialties/character-classes-mages-hunters-warriors.md)"\

*   **A "**[**`Level`**](item-levels/)**"**

    * 5 is the highest, to 1 is the lowest&#x20;
    * While Loot gives no specific language pertaining to power, strength, agility, dexterity, the "Level" rankings of the items are quite clear, and can be applied to any other interpretation of each item's specialty and purpose.


* **A** "<mark style="color:orange;">**`Rating`**</mark>"
  * An item's "Rating" is simply = `Level` x `Greatness`\
    ``
  * **For Weapons and Armor items** (6 items per bag)
    * **Max Rating** = 5 x 20 = `100`
    * **Min Rating** = \[any level] x 0 = `0`\
      ``
  *   **For Jewelry** (2 items per bag)

      * **Max Rating** = 3 x20 = `60`
      * **Min Rating** = \[any level] x 0 = `0`


  * **For a bag** (8 items)
    * **Max Rating** = \[6x100] + \[2x60] = `720`
    * **Min Rating** = \[6x0] + \[6x0] = `0`

## Item "Ratings = Greatness x Level"

![](<../../../.gitbook/assets/image (32).png>)

**Direct link to Ratings table** —  [https://docs.google.com/spreadsheets/d/124OUErQjvkaQSjRR1Fc0RmmOI6NA3NKhmRiH-Ga9kyM/edit#gid=781147563](https://docs.google.com/spreadsheets/d/124OUErQjvkaQSjRR1Fc0RmmOI6NA3NKhmRiH-Ga9kyM/edit#gid=781147563)&#x20;
