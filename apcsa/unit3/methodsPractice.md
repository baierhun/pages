## Video Game Project: Player

Create a Java class called `Player` to represent the player character.

Instance variables: `String name`, `int health`, `int level`

Methods to write:

* A constructor to initialize all instance variables

* Getters for all three instance variables

* `isAlive()` — returns whether health is greater than 0

* `takeDamage(int damage)` — decreases health by the damage amount

* `getDescription()` — returns a String describing the player

## Video Game Project: Weapon

Create a Java class called `Weapon` to represent a weapon in the game.

Instance variables: `String name`, `int damage`, `double weight`

Methods to write:

* A constructor to initialize all instance variables

* Getters for all three instance variables

* `calculateDamage(int bonus)` — returns damage plus the bonus

* `isHeavy()` — returns whether weight is greater than 10

* `getDescription()` — returns a String describing the weapon

## Video Game Project: Enemy

Create a Java class called `Enemy` to represent an enemy in the game.

Instance variables: `String name`, `int health`, `int damage`

Methods to write:

* A constructor to initialize all instance variables

* Getters for all three instance variables

* `isAlive()` — returns whether health is greater than 0

* `takeDamage(int damageAmount)` — decreases health by the damage amount

* `getDescription()` — returns a String describing the enemy

<div class="break"></div>

## Video Game Project: Potion

Create a Java class called `Potion` to represent a potion the player can use.

Instance variables: `String name`, `int healingAmount`, `double price`

Methods to write:

* A constructor to initialize all instance variables

* Getters for all three instance variables

* `canAfford(double gold)` — returns whether the player has enough gold

* `calculateHealing(int bonus)` — returns the healing amount plus the bonus

* `getDescription()` — returns a String describing the potion

## Video Game Project: Spell

Create a Java class called `Spell` to represent a magical spell.

Instance variables: `String name`, `int damage`, `int manaCost`

Methods to write:

* A constructor to initialize all instance variables

* Getters for all three instance variables

* `canCast(int mana)` — returns whether the player has enough mana

* `calculateDamage(int bonus)` — returns damage plus the bonus

* `getDescription()` — returns a String describing the spell

## Video Game Project: Treasure

Create a Java class called `Treasure` to represent treasure found in the game.

Instance variables: `String name`, `double value`, `int rarity`

Methods to write:

* A constructor to initialize all instance variables

* Getters for all three instance variables

* `isRare()` — returns whether rarity is 4 or higher

* `calculateValue(double multiplier)` — returns the value multiplied by the multiplier

* `getDescription()` — returns a String describing the treasure
