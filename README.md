# Tower Defense

A board game inspired by tower defense video games. There are others out this, this one is focussed on co-operative play and possible narrative/legacy exploration.

- [Tower Defense](#tower-defense)
  - [What you need](#what-you-need)
  - [Setup](#setup)
  - [Rules](#rules)
  - [References](#references)
    - [Bad Guys](#bad-guys)
    - [Purchases](#purchases)
  - [Scenarios](#scenarios)
    - [Scenario 1](#scenario-1)

## What you need

- A map
  - Currently hand drawn on a piece of A3 paper
- A whole bunch of 6 sided dice, in an ideal world grouped by the following (maybe different colours)
  - 8 tower dice
    - These will be your towers, each tower starts on level 1 (1 pip showing). As towers level up you show the next pips until max level 6
  - 3 gate dice
    - Represent the health of your gate/base, you lose the game if you run out of these dice
  - 4-8 gold dice
    - Represents how much gold you have to buy towers and upgrades
  - 4-8 battle dice
    - The dice you roll to resolve damage
  - 1 phase dice
- 1-4 Hero miniatures
- A bunch of bad guy miniatures
  - 20-30 normal bad guys
  - 10-20 fast bad guys
  - 5-10 heavy bad guys
  - 1 boss bad guy

## Setup

- Layout your map on the table
- Group all your dice by color/group
- Put your hero on the gate space
- Pick a [scenario](#scenarios) to play
- Place your hero health dice on the hero space, with 6 showing
- Place the corresponding amount of gate dice on the gate space, according to the scenario (with the correct pip showing)
- Take the phase dice and place 1 pip up on the phase 1 space. This indicates round 1 of phase 1
- Take the corresponding amount of gold, according to the scenario. (Take enough gold dice with the pip count matching this value)

## Rules

Objective, whatever it says on your chosen scenario

The game happens in the following turns

- Phase starts
  - Bad guys turn
    - Activate bad guys
      - If any bad guy is in the space of a hero
        - Look up the bad guys Damage Value, minus that from the hero health dice.
          - If the hero's health is down to 0, they are severely wounded. Take them back to the gate. Each round a hero spends on the gate gives them +1 on their health dice, but only if they do no other action on that round
      - Else if a bad guy is in the gate space
        - Look up the bad guys Damage value. Minus that from the gate dice and discard the bad guy
          - If a gate dice is down to 0, discard it, you can no longer upgrade or restore that dice
      - Else
        - Look up the bad guys speed and move the bad guy that many spaces towards the gate.
        - If their is a crossroad, gather up all the bad guys of that type who are doing the same movement and split them evenly each way.
          - If there's an uneven amount, spawn a new bad guy of that type to even it out
            - If the bad guy is a boss or 1 of a kind character roll a d6, 1-3 one way, 4-6 the other.
    - Spawn
      - Look at what phase and round you're on, based off the phase dice. Match that up with the what bad guy the scenario says you should play. Something like "Normalx1". Normal is the kind of bad guy to put down. "x1" is how many d6 to roll to figure out how many of those bad guys to put down.
      - Roll the "x1" number of dice and place that many of those bad guys in the spawn space
  - Players turn
    - Spend gold
      - You can use all the gold you have to buy towers, upgrade them, upgrade your character and increase gate defences. Check out the [purchases](#purchases) for how to spend your gold. Each time you spend, decrement your gold dice. If a dice goes to 0, put it with the rest of the discarded gold dice.
      - Some scenarios may override/add what's in the purchases table
      - When you buy a tower it starts on level 1 (1 pip showing), you can put the tower dice on any spare tower space
      - When you buy a tower upgrade, rotate the dice to show the level it's at
    - Activate towers
    - Each tower can fire once in an area that it's arrows point to. (Unless the upgrade ability says otherwise)
    - When a tower fires, roll the number of dice equal to the towers level. Each dice can target 1 specific bad guy. To kill a bad guy you must roll the same or higher than the bad guys health value. If you succeed, discard that bad guy and add gold equal to the bad guys Reward Value. If you miss, bad luck.
      - Bosses are handled slightly differently. See the bosses section.
    - Activate hero's
      - Each hero can do 2 actions
        - Move up to 2 spaces
        - Attack
          - Pick 1 bad guy and roll 2 dice to attack them. Resolving in the same way as towers.
  - Increase phase dice
    - If the phase dice is on the last round of that phase (according to the scenario) then you must wait until all bad guys have been defeated or discarded then move the die to the next phase on pip 1.
      - If the scenario has no more rounds, you can leave the dice as it is. No more spawns will be happening.

## References

### Bad Guys

| Type   | Damage Value | Speed Value | Health Value | Reward Value | Special Rules                                                |
| ------ | ------------ | ----------- | ------------ | ------------ | ------------------------------------------------------------ |
| Normal | 1            | 1           | 3            | 1            |                                                              |
| Fast   | 1            | 2           | 2            | 2            |                                                              |
| Heavy  | 2            | 1           | 5            | 3            |                                                              |
| Boss   | 5            | 1           | 5            | 10           | Must be hit successfully 3 times (Use another dice to track) |

### Purchases

- Tower - 4
- Upgrade - 3
- Gate health +1 - 6

## Scenarios

### Scenario 1

- Gate Dice - (3, 3, 3)
- Phases
  - 4 - (Normalx1, Normalx1, Normalx1, Normalx1)
  - 4 - (Normalx2, Normalx2, Fastx1, Fastx1)
  - 4 - (Heavyx1, Normalx2, Fastx2, Heavyx1)
  - 4 - (Heavyx2, Boss, Heavyx2, Fastx2)
- Starting gold - (12)
