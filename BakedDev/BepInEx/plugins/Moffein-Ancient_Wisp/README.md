Adds the unfinished Ancient Wisp boss into the game.
It's an 1000 credit boss (slightly more expensive than Imp Overlords and Magma Worms)
Spawns on Abyssal Depths, Sundered Grove, Sky Meadow, Sulfur Pools (postloop), as well Gilded Coast and Bulwark's Ambry.

Internal bodyname is MoffeinAncientWispBody.

Currently shares the same boss item drop as the Grovetender.
Send me feedback on the balance!

## Attacks

Default Attack - Barrage: Shoots a spread of 6 rolling fireballs

Signature Attack - Lightning Pillars: Summons many Lightning Pillars around the players

Utility - Enrage: At 50% HP, enrages and gains increased move speed and attack speed, which boosts the amount of projectiles it shoots.


[![](https://i.imgur.com/TXUxE9Y.png)]()
[![](https://i.imgur.com/POwj2jp.png)]()

All players need the mod.
Config options for what stages it spawns on can be found in /Risk of Rain 2/BepInEx/config/com.Moffein.AncientWisp.cfg

## Installation
Place the Moffein-AncientWisp folder in /Risk of Rain 2/BepInEx/plugins/

## Credits

Pikmin88 - Preview picture on Sky Meadow

rob - Logbook icon

## Changelog

`1.6.4`

- Updated AccurateEnemies compatibility. Now is affected by AccurateEnemies config options.

`1.6.3`

- Added Russian translation (Thanks Адский Шкед!)

`1.6.2`

- Pillar damage is now counted as AoE damage.
	- Only relevant for mods that use the ResistantToAoE bodyflag.

`1.6.1`

- Added Simplified Chinese translation (Thanks JunJun_w!)

`1.6.0`

- Languagefile support.
- Added to Wisp family.
- Logbook entry.

`1.5.2`

- AccurateEnemies compatibility.

`1.5.1`

- Changed Barrage projectile falloff moddel from Linear to Sweetspot.

`1.5.0`

- Re-enabled fire trails on Barrage.

`1.4.4`

- Can now be targeted by the Trophy Hunter's Tricorn.

`1.4.3`

- Fixed console spam on startup.

`1.4.2`

- Attempted to fix an incompatibility issue with NewtDrops.

`1.4.1`

- Fixed for R2API update.
- Added to Dissonance spawnpool.
- Changed config format. Stages are now stored in a single list.
- Added Buff Icon to Enrage.
- Elite Displays
	- Blazing horns are now symmetric.
	- Added Mending display.
	- Added Voidtouched display.

`1.4.0`

- Fixed for DLC Update.
- Added weak point.
- Increased director credit cost from 800 -> 1000
- Disabled spawning in the Void Fields by default.
- Can now spawn on Sulfur Pools postloop.
- Now spawns in Simulacrum if it is enabled on the respective stage.

*Ancient Wisps are incredibly deadly in groups, so its cost has been increased to reduce how many will spawn from teleporter events.*

`1.3.5`

- Added support for the Artifact of Origination from Risky Artifacts.

`1.3.4`

- Director spawn card is now accessible to other mods.
- Lighting Pillar chargeup time reduced 2.5s -> 2s
- Lightning Pillar base count increased 40 -> 45.
- Lightning Pillar max count increased 72 -> 120.
- Enrage duration reduced 3s -> 2.5s
- Enrage now spawns 2 Greater Wisps

Been feeling for a while that Ancient Wisps are too much of a pushover currently, so I've undone a few of the nerfs they've received in previous updates, and also reduced the amount of time it spends standing still waiting to charge up attacks.

`1.3.3`

- Fixed for the Anniversary Hotfix update. Had to change some stuff internally, so lemme know if Lightning Pillars are working properly online.

`1.3.2`

- Fixed mismatched version number.

`1.3.1`

- Swapped Lightning Pillars to Primary and Barrage to Secondary. This should only affect modded setups where Ancient Wisps can get Backup Mags.

`1.3.0`

- Fixed for Anniversary Update.
- Disabled fire trails on Barrage due to null reference errors from the new update. Will have to figure out a fix later.
- Barrage projectiles now travel further on the ground.
- Tweaked Barrage spread pattern.
- Lowered base Lightning Pillar count from 45 to 39.

`1.2.1`

- Fixed minimum stages completed config settings not working.

`1.2.0`

- Changed how the config works. Now specifies # of stages completed before the AW will start spawning on each stage. Negative values disable them from spawning on the specified stage.
- Ancient Wisps no longer spawn on Rallypoint Delta, since it's likely you won't have enough mobility to fight it at that point. This also should prevent occassions where you end up getting Ancient Wisps for 3 stages in a row.
- Lightning Pillar explosion delay increased 1.2s -> 1.3s.
- Lightning Pillar cooldown increased 18s -> 22s.
- Enrage no longer gives Armor.

`1.1.5`

- Added missing LoadoutAPI dependency. Most users will see no change from this, but this should fix the mod for people who don't have any survivor mods installed.
- Increased Barrage range from 100 -> 150.
- Removed Barrage gravity. The gravity was originally added because Ancient Wisps were really bad at aiming, but it turns out that was due to an AI bug which was fixed. The removal of gravity on the projectiles should make Ancient Wisps better at hitting airborne and long distnace targets, and will make them able to hit players camping in the wind tunnels in Sky Meadow. Lemme know how this change feels!
- Ancient Wisps are now slowed 50% while using Lightning Pillars and Enrage.

`1.1.4`

- Fixed Barrage being aimed at the Ancient Wisp's movement direction instead of at its current enemy.
- Increased Barrage max projectile count from 14 -> 16. (This will not be reached unless the Ancient Wisp has attack speed items)
- Ancient Wisps now always prioritize using their Lightning Pillars whenever available.
- Lightning Pillars now cannot be cancelled by Enrage.
- Enrage cast duration reduced from 5s to 3s.

`1.1.3 (Hotfix)`

- Decreased Lightning Pillar base pillar count from 90 -> 45.
- Increased Lightning Pillar max pillar count from 72 -> 90.

`1.1.2`

- Fixed Lightning Pillar max pillar cap not actually applying. This should fix endless lightning spam in modded setups where Ancient Wisps can get a lot of attack speed.
- (BUG) Accidentally increased Lightning Pillar base pillar count from 45 -> 90.
- (BUG) Accidentally decreased Lightning Pillar max pillar count from 90 -> 72.

`1.1.1`

- Ancient Wisps no longer stand still while casting attacks.
- Barrage charge time reduced from 3s to 2.5s.
- Lightning Pillar damage coefficient increased from 200% -> 210%.
- Lightning Pillar vertical hitbox damage increased from 40% TOTAL to 50% TOTAL.
- Lightning Pillar vertical hitbox range increased from 12m to 16m.
- Lightning Pillar explosion delay reduced from 1.5s to 1.2s.
- Lightning Pillar cooldown reduced from 25s to 18s. It should be noted that Ancient Wisps only use Lightning Pillars after expending all M1 charges (2 charges, 7s cooldown to recharge all stocks at once)

`1.1.0`

- Removed negative vertical aim offset on Barrage.
- Barrage projectiles are now affected by gravity. Hopefully this will make them a bit better at hitting targets instead of just flying off into the distance.
- Lightning Pillar damage coefficient reduced from 210% -> 200%.
- Lightning Pillar pillar count increased from 40 -> 45.
- Lightning Pillar max pillar cap increased from 80 -> 90.
- Lightning Pillars are now always oriented upwards. This is purely a visual change, as their hitbox is a sphere on the ground.
- Lightning Pillars now hit enemies above their center for 40% TOTAL damage. Would like feedback on this change!

`1.0.3`

- Fixed Lightning Pillar visual effects not disappearing when zapped by Captain's microbots (it still would successfully prevent the damage though).
- Reduced Enrage cast duration from 6s to 5s.

`1.0.2`

- Added attack speed scaling caps aimed towards modded enemies with items setups.
    - Barrage now caps at 16 projectiles when scaling with attack speed.
    - Lightning Pillars now caps at 80 pillars when scaling with attack speed.
- Fixed Enrage spamming its activation noise for clients online.
- Reduced death explosion frequency from 3/s to 2.5/s.

`1.0.1`

- Corrected incorrect readme description for default attack. It actually shoots 6 fireballs.
- Increased interactor distance from 3 to 6, for people who want to play as the boss. Bodyname is MoffeinAncientWispBody.

`1.0.0`

- Release
