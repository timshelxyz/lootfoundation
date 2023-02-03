# Item "Name" Prefixes

## What are Name Prefixes? <a href="#block-82e6b0a0afa54331ba2ce1e8567d6e8f" id="block-82e6b0a0afa54331ba2ce1e8567d6e8f"></a>

In the Loot contract, some items are given a "namePrefix" and "nameSuffix."

Example:

![](<../../../.gitbook/assets/Screen Shot 2022-02-20 at 1.42.30 PM.png>)

## There is Order and Structure in the Name Prefixes

At first, it appeared that the assignment of Names to Items was random and haphazard — it turns out it is not. 🤯

The name prefixes have a particular structure and order, hidden inside the logic of the OG Loot contract:

1. <mark style="background-color:yellow;">**There are three distinct "sets" of Names for items.**</mark>
   * These sets are mutually-exclusive, collectively-exhaustive, and clearly follow a pattern
   * See [three-sets-of-names.md](three-sets-of-names.md "mention")\

2. <mark style="background-color:yellow;">**There exists a set of constraints for how "Names" can be used**</mark> \ <mark style="background-color:yellow;">****</mark>
   * **Some names, though they are in the contract code, are never used on actual Loot items**
     * See [the-missing-name-prefixes.md](advanced-name-constraints/the-missing-name-prefixes.md "mention")\

   * **Some names can only be assigned to some Items**
     * See [constraint-names-less-than-greater-than-items.md](advanced-name-constraints/constraint-names-less-than-greater-than-items.md "mention")\

   * **Some names can only be assigned to some Orders**
     * See [constraint-names-less-than-greater-than-orders.md](advanced-name-constraints/constraint-names-less-than-greater-than-orders.md "mention")

****

****
