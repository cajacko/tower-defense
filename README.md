# Tower Defense Board Game

![Tower Defense prototype v2](assets/v2-narrow.jpg "Tower Defense prototype v2")

A co-operative tower defense board game for at least 2 players, with a bunch of different maps/scenarios and a legacy component to it. To make it feel more like a story.

## Table of Contents

- [Tower Defense Board Game](#tower-defense-board-game)
  - [Table of Contents](#table-of-contents)
  - [What you need](#what-you-need)
  - [Setup](#setup)
  - [Rules](#rules)
  - [References](#references)
    - [Minions](#minions)
    - [Bosses](#bosses)
    - [Towers](#towers)
    - [Heros](#heros)
  - [Scenarios](#scenarios)
    - [Scenario 1](#scenario-1)

## What you need

- The rules (You're reading them)
- A map board
  - Currently hand drawn on a piece of A3 paper. Shows a path leading to the gate which you need to defend. The enemies will spawn at the opposite end and make their way down the path. The path is split into around 6 sections. Where the pieces will move between each section. There are also tower spaces on the map, that indicate where you can build towers.
- 4 sets of 6 sided dice, ideally each set is a different colour.
  - 10 tower dice
    - These will be your towers, each tower starts on level 1 (1 pip showing). As towers level up you show the next pips until max level 6
  - 10 health dice
    - Will be used to represent the health of your gate, heroes and the boss
  - 10 gold dice
    - Represents how much gold you have to buy towers and upgrades
  - 10 battle dice
    - The dice you roll to resolve damage
- 4 Hero miniatures
- 4 Hero cards
  - Describe the heroes abilities and has space to put on a health dice
- Tower miniatures
  - 6 towers of each type. Which has a space in the top to place the tower dice, showing the level of that tower
- 30 tokens for each type of minion (Circular tokens depicting each minion type. Done as tokens so they can be stacked on top of each other)
- 3 boss miniatures
- Event Cards
  - A bunch of cards that describe what enemy gets spawned (minion type or boss) and how many or describing another event that happens

## Setup

- Pick a [scenario](#scenarios) to play
- Layout your map on the table
- Group all your dice by colour/group
- Each player chooses a hero to play. They take the corresponding hero card and place their miniature on the gate space of the map. Place a health dice on the hero card, with the max health of the hero showing.
- Place the corresponding amount of gate dice on the gate space, according to the scenario (with the correct pip showing)
- Take the corresponding amount of gold, according to the scenario. (Take enough gold dice with the total pip count matching this value)
- Create the event deck as described in the scenario

## Rules

Your objective is whatever it says on your chosen scenario.

The game happens in the following turns:

- Event phase
  - Draw the top event card and do the following depending on the event type. If there are no more event cards left, do nothing in this step. If there are no more enemies on the board when this happen and you still have not reached the scenario objectives, you have lost.
    - Spawn
      - Follow the card instructions to spawn the corresponding enemy tokens on the spawn space of the map
    - Custom event
      - Just follow the instruction son the card
    - Wait
      - Do not draw another event card until the map is clear of all enemies
- Enemy phase
  - Activate each enemy. Each enemy gets 1 activation. Choose the first possible action from the following list for each enemy. First activate enemies by the highest movement value, then by the highest damage, then by the highest health. Otherwise the order does not matter.
    - If an enemy has a custom ability that takes precedence, do that
    - If the enemy is in the same space as a hero, and that hero has not been attacked during this phase.
      - Look up the enemies Damage Value, minus that from the hero's health dice.
        - If the hero's health is down to 0, they are severely wounded. Take them back to the gate, reset their health to 1. And they must skip the next players phase.
    - If an enemy is in the gate space
      - Look up the enemies Damage value. Minus that from the gate dice and discard the enemy token
        - If a gate dice is down to 0, discard it, you can no longer upgrade or restore that dice
        - If there are no more gate dice less, you have lost the game.
    - Else
      - Look up the enemies movement and move the enemy token that many spaces towards the gate.
      - If there is a crossroad, gather up all the enemies of that type who are doing the same movement and split them evenly each way.
        - If there's an uneven amount, spawn a new enemy of that type to even it out
          - If the enemy is a boss or 1 of a kind character roll a d6, 1-3 one way, 4-6 the other.
- Players phase.
  - For each hero you can do 2 of the following actions, you can do the same action twice.
    - Build a tower
      - If you are in a space that is adjacent to an empty tower space, you can spend the required amount of gold to build a tower on that tower space. Reduce your gold by that amount, and place the corresponding tower miniature with a tower dice on 1, on that space.
    - Upgrade a tower
      - If you are in a tower or on a space that is adjacent to a tower, you can spend the required amount of gold to upgrade the tower. Reduce your gold by that amount, and turn the tower dice up by 1 pip.
    - Increase the gate health
      - If you are on the gate space you can spend 20 gold to increase one of the gate dice by 1 pip.
    - Mount a tower
      - If a hero is on a space adjacent to a tower space they can mount that tower. Move the hero off of the path and next to the tower space. Only 1 hero can mount a tower at a time.
    - Unmount a tower
      - Move the hero onto a space adjacent to the mounted tower space
    - Attack an enemy
      - You can attack an enemy in the same space as a hero. Roll 1 dice, if that dice value is equal or higher than the targeted enemies defense value, you kill it. Remove it from the board and gain the reward specified for that enemy.
    - Activate a special hero or tower ability that applies
      - If the ability text on a hero or tower lets you do an action at this stage, you can do that
    - Move
      - You can move the hero the same number of spaces as it's movement value
    - Do nothing
  - Each tower can fire once in an area that it's arrows point to. (Unless the upgrade ability says otherwise)
  - When a tower fires, roll the number of dice equal to the towers level. Each dice can target 1 specific bad guy. To kill a bad guy you must roll the same or higher than the bad guys health value. If you succeed, discard that bad guy and add gold equal to the bad guys Reward Value. If you miss, bad luck.
    - Bosses are handled slightly differently. See the bosses section.
- Tower phase
  - Each tower can make 1 attack on enemies it can target. See the Targeting column for each tower to see who it can attack. When attacking role the same number of dice as the towers level. Every dice value that is equal or higher than the targeted enemies Defense value is killed. Remove the killed enemy tokens from the space and pile them next to the tower that killed them. This represents unclaimed rewards. Any hero in that tower or an adjacent space to that tower can automatically claim all the rewards that tower currently has, even when passing through in a movement turn.

## References

### Minions

Minions are generic enemies. You will typically get many of these spawning at a time.

| Name          | Type   | Damage | Movement | Health | Reward | Abilities                                                                                                                             |
| ------------- | ------ | ------ | -------- | ------ | ------ | ------------------------------------------------------------------------------------------------------------------------------------- |
| Gremlin       | Ground | 1      | 1        | 3      | 1      |                                                                                                                                       |
| Devil Steed   | Ground | 1      | 2        | 3      | 2      |                                                                                                                                       |
| Bat Monkeys   | Flying | 1      | 1        | 3      | 2      |                                                                                                                                       |
| Golem         | Ground | 2      | 1        | 4      | 3      |                                                                                                                                       |
| Dark Wizard   | Magic  | 1      | 1        | 3      | 3      |                                                                                                                                       |
| Corrupt Dwarf | Ground | 3      | 1        | 4      | 4      | When finishes their activation in a space with a linked tower, pick a linked tower and decrease it's level by 1. Cannot attack a hero |

### Bosses

Bosses are unique in that only a roll of 6+ can harm them. Their health represents how many times you need to roll a 6+ to kill them. Keep track of their health with boss dice.

| Name    | Type   | Damage | Movement | Health | Reward | Abilities                                                                                                                                 |
| ------- | ------ | ------ | -------- | ------ | ------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| Morgu   | Ground | 5      | 1        | 10     | 30     | At the end of the enemy phase, all towers adjacent to the space this boss is in and that can target ground enemies get lowered y 1 level. |
| Damitat | Flying | 5      | 1        | 10     | 30     | At the end of the enemy phase, all towers adjacent to the space this boss is in and that can target flying enemies get lowered y 1 level. |
| Flambee | Magic  | 5      | 1        | 6      | 40     | At the end of the enemy phase, all towers adjacent to the space this boss is in and that can target magic enemies get lowered y 1 level.  |

### Towers

| Name          | Purchase Cost | Upgrade Cost | Targeting                                                                  | Special                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Can Target            |
| ------------- | ------------- | ------------ | -------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- |
| Archery Tower | 4             | 4            | Can only target enemies in a linked space                                  | N/A                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | Ground, Flying        |
| Swordsmen     | 4             | 4            | Can only target enemies in a linked space                                  | Any enemy in/passing through this space loses 1 movement (can't go below 1)                                                                                                                                                                                                                                                                                                                                                                                                   | Ground                |
| Bombers       | 6             | 5            | Can only target enemies in a linked space                                  | Roll double the amount of attack dice per tower level                                                                                                                                                                                                                                                                                                                                                                                                                         | Ground                |
| Mage Tower    | 8             | 6            | Can only target enemies in a linked space                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Ground, Flying, Magic |
| Stables       | 6             | 5            | Can target enemies in a linked space or a space adjacent to a linked space |                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Ground                |
| Trebuchet     | 10            | 6            | Can target enemies in a linked space or up to 3 adjacent spaces away       | Can only be used on 1 targeted space per round. Ignore the normal rules for attacking with a tower. Instead roll 1d6. On a 1, you missed the enemies and hit a tower linked to that space. Decrease the tower level by 1, if no tower then no effect. On any other roll you hit the enemy! Roll 1/2 the amount of attack dice as the tower level. Rounding down, no lower than 1 dice. Take the highest dice and apply that damage to every Ground enemy in the chosen space. | Ground                |

### Heros

| Name                    | Movement | Health | Special                                                                                                                                                | Can target            |
| ----------------------- | -------- | ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- |
| Glorbud the Huge        | 1        | 6      | Roll 2 dice when attacking, -2 to the purchase and upgrade cost of Bomber towers.                                                                      | Ground                |
| Keith the Crazed Archer | 2        | 5      | -1 to the purchase and upgrade cost of Archery towers                                                                                                  | Ground, Flying        |
| Henry the Horse Lord    | 3        | 4      | -2 to the purchase and upgrade cost of Stables                                                                                                         | Ground                |
| Mongo the Mage          | 2        | 3      | -2 to the purchase and upgrade cost of Mage Towers. When in a Mage Tower it can target enemies in a linked space or a space adjacent to a linked space | Ground, Flying, Magic |
| Edward the Engineer     | 2        | 4      | Can spend 10 gold to increase gate health by 1, -1 to all tower costs and upgrades                                                                     | Ground                |

## Scenarios

### Scenario 1

- Objective
  - Defeat all enemies
- Gate Dice - 3, 3, 3
- Starting gold - 12
- Event Deck
  - Put the following event cards in this order (So you would draw the first card listed here first)
    - Gremlin x 4, Gremlin x 4, Gremlin x 4, Gremlin x 4, Wait,
    - Gremlin x 8, Gremlin x 8, Devil Steed x 4, Devil Steed x 4, Wait
    - Golem x 4, Gremlin x 8, Devil Steed x 8, Golem x 4, Wait
    - Golem x 8, Boss (Morgu), Golem x 8, Devil Steed x 8, Wait
