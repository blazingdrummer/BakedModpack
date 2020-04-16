## Character Skills

### Blood Bank (Passive)
- Special can hold up to 10,000 charges (though you start each stage with only 1 charge).
- In addition to recharging naturally with time and items, all of the Surgeon's other skills can work to reduce Special's cooldown.
- If the number of stored charges exceeds ten times your current stage number, abilities will no longer charge Special.
- Special has by far the highest DPS of any of the Surgeon's skills, so proper resource-management of its cooldown is the key to winning any engagement.



### Hemorrhage (Primary)
- A shotgun blast that pierces enemies. Each hit charges special.
- Holds up to five charges. The more charges you have stored, the more shots will be fired. Will never drop below 1 charge.
- Attack speed will affect the number of shots fired, rather than the rate of fire.

### Incision (Alt Primary)
- A rapid-fire attack that continues firing until it misses (does not require the button to be held down).
- Like Hemorrhage, charges special each time it hits. The amount each shot charges special increases the longer it fires without missing.



### Laughing Gas (Secondary)
- Drops a canister that covers the surrounding area in gas for a brief period of time.
- The gas lingers in place at the Surgeon's position when the move was used. 
- All enemies within range are continually stunned and weakened, and dramatically increase the amount Primary charges Special.



### Transfusion (Utility)
- Over the next couple of seconds, heals a fraction of your max HP.
- Healing above full will charge Special.
- Any damage taken while this ability is active is stored. Each healing tick, a static fraction of the stored damage is healed back.
- Stores more damage than is actually taken - meaning that taking damage may cause you to be healed more than if you hadn't been damaged at all.
- Can be canceled by other abilities (except Primary); doing so will 1) instantly heal back any stored damage that would have been healed had the ability completed naturally, and 2) partially refund Transfusion's cooldown.



### The Sanguinator (Special)
- A huge laser beam that deals tremendous damage to a single target.
- Continues firing as long as the button is held - as long as it has enough charges.
- The longer it fires continuously, the more damage it deals per charge consumed.

### Blood Bath (Alt Special)
- Hold the button to build up power. Once the button is released - or you run out of charges - unleashes a massive explosion that deals light damage to everything in its range.
- The damage and radius of the explosion increases the longer it is charged.




## Tips, Tricks, and Trivia
- For performance reasons, the actual number of shots Hemorrhage can fire is capped. The damage and special charge of each shot will increase to match the intended total values.
- Hemorrhage pierces through enemies, making it extremely effective against groups. Use the time spent waiting for its cooldown to line up the perfect shot.
- Incision's damage also increases the longer it continues firing - though it grows slowly enough that it isn't really noticable.
- Watch out for Malachite enemies; they render Transfusion completely useless.
- Though Special is most powerful when you allow it to build up a lot of charge, don't feel the need to save it exclusively for the teleporter boss.




## Changelog

### 1.4.2
- Fixed a bug where certain abilities wouldn't work properly if used by a non-host in multiplayer.

### 1.4.1
- Fixed a bug where Transfusion did not heal stored damage properly.

### 1.4.0
- Hemorrhage's horizontal spread has been increased, and its vertical spread has been reduced to almost zero. This should make it more consistent, particularly against groups.
- Hemorrhage's knockback no longer scales infinitely with attack speed, meaning it no longer sends small enemies flying late-game.
- Fixed a bug where Hemorrhage wouldn't properly alternate which hand is firing.
- Incision will no longer stop firing if it hits a teammate (such as Beetle Guards or Drones). Note that teammates give no special charge or growth; they only stop the chain from breaking.
- Laughing Gas' custom status condition is no longer considered a debuff (aka the number of debuffs Laughing Gas applies has been reduced from 2 to 1). Note that Death Mark doesn't count custom debuffs as debuffs without mods, so in most cases this changes nothing.
- Transfusion can now be canceled by other abilities; see its description above for more details.
- Fall damage during Transfusion no longer charges special (though the damage is still healed).
- Transfusion no longer stores damage dealt by Blood Shrines.
- Transfusion's special charge from all other sources of damage has been dramatically increased.
- Improved performance of various abilities at extremely high attack speeds.
- Removed April Fools ability descriptions (lol)


### 1.3.1
- Fixed typos in ability descriptions.


### 1.3.0
- Artifact update!
- Updated ability descriptions.
- The maximum number of charges Special can hold is now equal to ten times your stage number, rather than anything to do with character level.
- Primary's special charge now has falloff. At point-blank range, they'll charge special roughly twice as fast; further than ~20m, they will charge less than before.
- Changed Primary 1's name from Lacerate to Hemorrhage, for flavor reasons.
- Hemorrhage has been made slower, but significantly more powerful.
- Fixed an issue where Laughing Gas didn't proc items properly.
- Transfusion's base healing has been decreased, but its stored damage multiplier has been increased.
- Transfusion now calculates overheal charge for its base healing and healing from damage separately. Base healing always charges the same amount, while damage-healing charges based on the amount of damage taken relative to the Surgeon's max health with no items.
- The Sanguinator's base damage has been increased.
- Blood Bath is now a ranged attack.



### 1.2.0
- Hemorrhage's base damage has been increased, but it's proc rate has been reduced.
- Laughing Gas now increases Incision's growth rate (instead of applying a flat boost to its special charge).
- Laughing Gas' special charge boosting effect now stacks.
- Rex's Weaken will no longer increase the special charge of Surgeon's Primary.
- Transfusion now stores damage dealt to temporary barrier.
- All items that increase max health will now increase the amount of special charge gained from Transfusion's overheal (previously, only shields affected this).
- Added brief startup delay for Blood Bath, to make it easier to use only a single charge.
- Increased time between each hit of Blood Bath, to make the fact that it hits multiple times more noticeable.
- Increased Blood Bath's base damage, but gave it damage falloff.




## To-Do List
- Add UI elements near the crosshair for things such as current special charge, Hemorrhage's cooldown, or Transfusion's stored damage, to lessen the amount of time spent looking at health and skill icons instead of the actual game.
- The Surgeon uses Artificer as a base for a lot of non-gameplay things. The model and animations used aren't going to change, but the ability icons, skins, and ENV Suit eventually might.
- As a result, mods that change Artificer *may* have knock-on effects on the Surgeon. The mod may be restructured in the future to reduce such incompatibilities.
- Squishing bugs wherever they happen to emerge.


## Other Stuff
- This mod is installed the exact same way as every other mod.
- Works in multiplayer - though, of course, all players must have the mod installed.
- If you have feedback and/or complaints you can hit me up on Discord.
- Have Fun :)