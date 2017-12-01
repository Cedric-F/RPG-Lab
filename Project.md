# Project idea

## RPG Game

### Features:

* JavaScript
  * Objects
    * Characters prototype
    * Monsters
    * Merchants
  * Arrays
    * Inventory
    * Loot table
    * Shops
    * Quests
  * Functions
    * Dice rolls
	    * Math.rand()
    * Events
    * Combat
	    * Exp gain
	    * Death
    * Level up
    * Loot
	    * Maths
	    * Math.rand()
	    * Math.pow()

* Design
  * Template
    * HTML/CSS
        * __Grid layout__
        * __flex box__
        * __CSS Variables__
  * Resources
    * SVG Images
      * game-icons.net
    * .mp3 Audio
  * jQuery
    * Events listeners
    * Game table

---
## General idea

A classic RPG game using Dice rolls to generate random events.
The player has:

* A main character.
* A team ? __Thoughts: Only one customizable character. Others' evolution is based on the main character's__

Character's stats:
* Main
  * Health
  * Mana
  * Stamina

* Strength
  * Increases the damage base.
  * Increases the inventory capacity.
* Agility
  * Reduces the chance of Fail and Critical Fail.
  * Increases the chance of Critical hit.
* Intelligence
  * Increases the Magic efficiency
  * Unlocks new special actions and spells

---


Story:
* Scripted Scenario. __Thoughts: Multiple possible endings__. Likely
  * Quests
    * Main storyline.
    * Sidequests.

 -or-

* Totally random events:
		* Requires a huge "database" of events to avoid redundance. Unlikely.

 -or-

* __Story ? Duck it!__. Very likely

---

Locations:

* Leveled areas
  * Cities
	  * Start village (Tier 1)
	    * Low tier Merchants
	      * Blacksmith
	      * Miscellaneous
	    * Tavern
	  * Hamlets (Tier 2)
	    * Medium tier Merchants
	    * Taverns
	  * Households (Tier 3)
	    * High tier Merchants
	  * Capital (Tier 4)
	    * Extreme tier Merchants
  * PvE
      * Tundra
        * Common: monsters spawns
          * Wildlife
          * Thugs
        * Uncommon: supermonsters spawns
          * Hunting prays
          * Wanted thugs
        * Rare: Outdoor Boss spawns
      * Dungeons
        * Misc: monsters
        * common: supermonsters
        * Boss

---

Inventory system:

* Limited number of item slots.
	* Stackable items such as potions and scrolls.
* Limited weigth:
		* Requires a weigth attribute to each "item" object.
* Unlimited inventory space.

---

Combat system:

* Panel of actions and spells.
    * Timed spawns:
    	* Check player's situation. If in combat, don't spawn another monster. In not in combat => math.rand() => hits a specific number => event.
	* Dice rolls:
		* Hit chances
			* Normal hit: common
			* Fail: common
			* Critical fail: uncommon
			* Critical hit: rare
