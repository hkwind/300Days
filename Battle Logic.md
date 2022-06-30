# Battle Logic

### This is the battle logic of the app 300Days. 

#### Back Logic

Each hero / enemy have their own Race (Human, Elf, Orc, Dwarf, etc), Class (Warrior, Archer, Spellcaster, Bard, Rogue), Attack Value, Defense Value, Speed Value(0.5-2), and Current Health.

Each battle, the above stats will be turn into numbers. Health is their base value, Attack - Opponent defense is the damage (at least 1), while the damage will be affected by race, class and traits. Speed value affects damage dealt speed.

Formula:



#### Before Normal Battle

The battle menu should split in half:

  - Left Half: Players hero show Attack Value, Defense Value, Current Health, Traits (3 Most), player swipes to change hero
  - Right Half: Enemy(s) show Attack Value, Defense Value, Current Health, Traits (3 Most)
  - Somewhere have a battle button and an escape button


