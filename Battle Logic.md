# Battle Logic

### This is the battle logic of the app 300Days. 

#### Back Logic

Each hero / enemy are a mecha. According to their equipment / settings, they will have different Attack Value, Defense Value, Dodge Value, Speed Value(0.5-2), and Health value.

Each battle, the above stats will be turn into numbers. Health is their base value, Attack - Opponent defense is the damage (at least 1), while the damage will be affected by equipments and traits. Speed value affects damage dealt speed. 


Equipments example:
(e.g. Extra Tough armour: Defense value + 200)

Traits example:
(e.g. Acid resistance: V.S. acid damage defense value + 15%)


```js
def DamageCalculation():
    
  MechaA_damage = MechaA_Attack-MechaB_Defense
  MechaB_damage = MechaB_Attack-MechaA_Defense
  
  while (MechaA_health > 0 and MechaB_health > 0):
    time += 1
    if (time mod MechaA_speed == 0):
      dodge = Math.random()
      critical = Math.random()
 
```
  



#### Before Normal Battle

The before battle menu should split in 3 part: (top left, top right, bottom)

  - Left Half: Players hero show Attack Value, Defense Value, Current Health, Traits (3 Most), player swipes to change hero
  - Right Half: Enemy(s) show Attack Value, Defense Value, Current Health, Traits (3 Most)
  - Somewhere have a battle button and an escape button


#### Battle

The battle menu should split in 3 part: (top left, top right, bottom)
  - Left Half: Players hero show Attack Value, Defense Value, Current Health (show bigger), Traits (3 Most), player swipes to change hero
  - Right Half: Enemy(s) show Attack Value, Defense Value, Current Health (show bigger), Traits (3 Most)
  - In bottom show 3 button: Hard defence, balance, hard attack
  - need a speed up function
  - A window should show lines about how the fighting goes:
    `e.g. Mecha A uses "Machine arm super punch". It hits mecha B on its head. Critical damage! Mecha B -15 health.`



#### Battle Sequence 
Each mecha basic 3 action:
Attack: Use basic attack
Defense: Defend opponent attack
Boost: Gain a strong attack (glowing)

Glowing action: Will disappear after this round
Grey action: The action's prerequisites is/are not fulfill.


