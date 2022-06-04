# Ephemeral Coins

Provides settings to control various aspects relating to Lunar Coins, including an Artifact that replaces them with temporary, per-run fascimiles that do not affect your save file's coin count. Almost all settings are independant and can be used with or without the Artifact.

**All changes are configurable in game with [Risk of Options](https://thunderstore.io/package/Rune580/Risk_Of_Options/)!**

- Artifact of the New Moon: Lunar Coins become Ephemeral Coins, a temporary per-run currency.
	- Config to disable entirely, or 'always on' mode that applies the effect at all times without an Artifact.
	- Config to begin each run with a set number of Ephemeral Coins (default 0).
- Lunar Coins drop rate changed to 5% / 0.9 falloff / 0.5% min chance.
- Lunar Pods made free of cost.
- The Frog made free of cost, and you only have to pet it once.
- Bazaar Between Time Lunar Buds cost lowered to 1 coin, and refresh when the Slab (Lunar Reroller) is used, even if already purchased.
- Bazaar Between Time Lunar Seer cost lowered to 1 coin.
- Bazaar Between Time Slab (Lunar Reroller) made free of cost. Can only be used once.
- The chance for a Blue Orb to appear on stage start flattened to 37.5%, instead of decreasing for each visit to BBT.

## Known Issues

- Lunar Reroller won't let you reroll if you've already bought the entire store, even if the config is set to refresh the lineup.
- Very little multiplayer testing has been done. Please report any bugs on [Github](https://github.com/VarnaScelestus/RoR2).

## Todo

- Re-implement [ProperSave](https://thunderstore.io/package/KingEnderBrine/ProperSave/) compatibility.

## Credits

[Magnus](https://github.com/MagnusMagnuson/RoR2Mods) - For the original code this was forked from. Not only was it an excellent starting point, it helped me learn a lot too!

[RoR2 modding discord](https://discord.gg/5MbXZvd) - For help in figuring out the Slab (Lunar Reroller)'s horrible, horrible internal structure, and just being awesome in general!

## Changelog

2.3.3 - Small fix for [RiskUI](https://thunderstore.io/package/Bubbet/RiskUI/) compatibility.

2.3.2 - Debug additions.

2.3.1 - Bug fix for 'always on' mode not setting up properly, a small tweak to artifact logic that might address [#16](https://github.com/VarnaScelestus/RoR2/issues/16), fix for some NREs from the HUD hook when exiting a run, and a fix for the starting coins message occuring once for each player instead of just once.

2.3.0 - Rewrote networking code for syncing coin counts, and cleaned up code surrounding the artifact (it now enables/disables its functions more like vanilla artifacts do).

2.2.2 - Hopefully the last fix for [Risk of Options](https://thunderstore.io/package/Rune580/Risk_Of_Options/) integration. Minor tweak to try and address multiplayer sync issues.

2.2.1 - Small fix for [Risk of Options](https://thunderstore.io/package/Rune580/Risk_Of_Options/) integration. Yes, again.

2.2.0 - Added config option for 'always on' mode. Minor hook changes to attempt to fix some incompatibility issues. Disabled [ProperSave](https://thunderstore.io/package/KingEnderBrine/ProperSave/) related code due to conceptual issues (see [Issue #8](https://github.com/VarnaScelestus/RoR2/issues/8)).

2.1.0 - Reworked how coins are tracked internally so that each player has their own count (oversight from 2.0.0 that was causing major bugs). Fixed compatibility with [ProperSave](https://thunderstore.io/package/KingEnderBrine/ProperSave/) (I hope) and some errors in how [Risk of Options](https://thunderstore.io/package/Rune580/Risk_Of_Options/) integration was handled.

2.0.1 - Fixed thunderstore issue preventing the assetbundle from being loaded.

2.0.0 - Major codebase refactor. Added Artifact of the New Moon, allowing you to toggle whether to use temporary coins on a per run basis without affecting your save file. Added [Risk of Options](https://thunderstore.io/package/Rune580/Risk_Of_Options/) integration.

1.4.0 - Added THE FROG.

1.3.0 - Added config setting for minimum drop chance.

1.2.2 - Internal cleanup; manifest updates

1.2.1 - Updated to work with SotV expansion

1.2.0 - Improved compatibility with [ProperSave](https://thunderstore.io/package/KingEnderBrine/ProperSave/).

1.1.0 - Added config setting for a starting amount of Lunar Coins per player (defaults to 0).

1.0.4 - Added logic to prevent Lunar Pods from having their cost changed in the BBT to avoid conflicts with [BiggerBazaar](https://thunderstore.io/package/MagnusMagnuson/BiggerBazaar/). (They do not spawn there in vanilla anyway.)

1.0.3 - Fixed the multiplayer name issue for real this time

1.0.2 - Fixed version number and wrong default setting for Slab cost

1.0.1 - Fixed multiplayer names displaying incorrectly

1.0.0 - Initial release