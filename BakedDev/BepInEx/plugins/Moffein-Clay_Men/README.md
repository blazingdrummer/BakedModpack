Adds the unfinished Clay Man into the game as a fast melee trash mob that can deal high damage to unwary players.

They can chase and keep up with sprinting players, but can be outmaneuvered by jumping and strafing.

Spawns on Abandoned Aqueduct, Aphelian Sanctuary, Sulfur Pools, Scorched Acres

Replaces Imps on Scorched Acres

[![](https://i.imgur.com/Wa6TVRR.png)]()

All players need the mod.

Partially based on rob's unfinished Clay Man code.

## Installation
Place the Moffein-ClayMen folder in /Risk of Rain 2/BepInEx/plugins/

## Changelog

1.5.3

- Added Russian translation (Thanks Адский Шкед!)

1.5.2

- Added Simplified Chinese translation (Thanks JunJun_w!)

1.5.1

- Fixed logbook unlock not saving.

1.5.0

- Languagefile support.
- Added logbook entry.

1.4.5

- Removed debug text.

1.4.4

- Lunge force increased from 1600 -> 1800 (reverted 1.4.0 lunge force nerf)
- Fixed Ghost Clay Men being unable to deal damage.
	- Railgunner weakpoint has shifted as a result of this change due to internal jank.

1.4.3

- Fixed console spam when booting up the game.

1.4.2

- Added option to remove Imps from stages (default is Scorched Acres only)

1.4.1

- Fixed incomaptibility issue with NewtDrops

1.4.0

- Fixed for DLC update.
- Added DLC1 Elite displays.
- Added weak point.
- Changed death VFX.
- Increased spawn cost from 16 -> 28 (same as Imps now)
- Base Stats
	- Base damage increased from 11 -> 12
- Sword Slash
	- Damage Coefficient increased from 1.4 -> 1.5
	- Cooldown increased from 1s -> 1.4s
	- Lunge force reduced from 1800 -> 1600
	- Skill activation distance reduced from 16m -> 12m
	- Increased hitbox vertical range to be closer to Imps.
	
*New damage is slightly less than a Blind Vermin, but swings slower than both Imps and Vermin. Mobility/aggressiveness has been lowered a bit, but remains higher than Vermin and Imps.*

- Spawn Pool
	- Added to Dissonance.
	- Disabled spawns on Rallypoint Delta, Sundered Grove, and Bulwark's Ambry by default.
	- Now spawn on Aphelian Sanctuary and Sulfur Pools.
	- Now spawn on Snowy Forest after looping.
	
- For Devs: Reorganized code.
	- The Clay Man GameObject is now located in the Content class instead of the plugin class.
	- The Clay Man Director Card Holder can now be accessed via the Content class.

1.3.7

- Increased hitbox size 16%
- Added stage config.

1.3.6

- Reduced HP 160 -> 140 (same as Imps now)
- Reduced base damage 12 -> 11

	*I'm trying to tone down Clay Men a bit, while still making sure they're still strong enough to be a threat to the player. I don't want to touch their speed and mobility since that's their defining feature. Their HP won't go any lower than this since they should be at least as sturdy as Imps at the minimum. Let me know how they feel with this update!*

1.3.5

- Remembered to include the dll.

1.3.4

- Updated for the Anniversary Hotfix update.

1.3.3

- Fixed Elite displays.

1.3.2

- Added missing dependency.

1.3.1

- Updated for Anniversary update.

1.3.0

- Reduced slash damage 150% -> 140% (turns 1.2.0 didn't actually reduce the slash damage).
- Increased spawn cost 15 -> 16.
- Reduced HP 170 -> 160.
- Beetles on Abandoned Aqueduct now have their spawnweight reduced from 2 -> 1.
- Temporarily disabled config. I plan to be making a decent amount of number tweaks to Clay Men, so I'll be re-enabling the config in a week or two once I have them in a good spot.

1.2.1

- Added lore.

1.2.0

- Reduced base damage 14 -> 12
- Reduced sword hitbox size by 14%.
- Clay Men can now spawn on Sundered Grove since Dunestriders spawn there.
- Clay Men can now spawn in the Void Fields and Bulwark's Ambry.
- Added a spawn noise.
- Added Elite displays.

1.1.3

- Clay Men now use BodyClones for better compatibility with PlayableTemplar. Clay Men are now internally labeled as MoffeinClayManMaster when spawning them via DebugToolkit.

1.1.2

- Reverted spawn cost back from 18 to 15. The original intent of increasing the spawn cost was to make Clay Men spawn a bit less frequently earlygame, but it instead caused them to rarely spawn at all. Even increasing the spawn cost just to 16 seemed to reduce their spawnrate significantly, so I'll be leaving it at 15.
- Reduced HP from 180 to 170. This is a minor change that should make it a bit easier to deal with Clay Men on stage 2 when you still have few damage items.
- Added spawn cost config option. This is server-side.

1.1.1

- Increased spawn cost from 15 to 18 to be on par with the Cost:HP ratio of other enemies.

1.1.0

- Fixed issues with Huntress targeting and melee in multiplayer.

1.0.1

- Readme update.

1.0.0

- Release