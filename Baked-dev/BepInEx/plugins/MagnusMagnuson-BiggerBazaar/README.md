# BiggerBazaar

This mod expands the bazaar with items to purchase. Use money or alternatively lunar coins to purchase items. Consider trying it out with [TemporaryLunarCoins](https://thunderstore.io/package/MagnusMagnuson/TemporaryLunarCoins/) if you're using lunar coins as payment option.

![shop](https://i.imgur.com/2q9jTri.jpg)
![exchange](https://i.imgur.com/0HVfreX.jpg)

## Features
*Recent features in bold*

 - 6 random items are available for purchase
	 - Base cost and rarity for each tier can be adjusted in the config file
	 - Cost scales with difficulty (if using money)
	 - Limit how many times each item can be bought by tier
	 - Restrict the amount of total purchases and/or purchases per tier per player
 - Use money you have left at the end of the stage... 
	 - When you take the bazaar portal, your money is not converted into experience points. Instead you keep it to buy items at the bazaar. Money left when you then leave the bazaar is converted into experience points
 - **or use Lunar Coins.** Consider trying it out with [TemporaryLunarCoins](https://thunderstore.io/package/MagnusMagnuson/TemporaryLunarCoins/)
 	- **Cost can be configured and does not increase**
 - You can exchange Lunar Coins for money at the friendly Shopkeeper
	 - You can adjust the amount of money in the config. Setting this value as the same as e.g. a tier 1 item means one Lunar Coin always gives you enough money to buy a tier 1 item
	 - You can limit the amount of exchanges, completely remove them or have infinite
 - Only the host is required to have the mod installed
 - If you're using ShareSuite, you can choose in the config whether bought items are shared or not by setting "ShareSuiteItemSharingEnabled" to true or false. **Automatically turned on when sharing money.**
 - Experimental price scaling mode
 	- Apparently after playing for a bit, players always have enough money to buy all available items. To prevent this, this price scaling mode was introduced. The prices for chests are scaled in such a way, that the players' combined money is only enough to buy a random percentage (lower and upper bounds configurable) of the shops inventory. The configured base costs for tiers are used to keep the correct price ratio.
 	- Alternatively, you can use the new restriction configurations to limit the amount of purchases per player.


## Installation

- Install [BepInEx Mod Pack](https://thunderstore.io/package/bbepis/BepInExPack/) (if you haven't already)
- Install [R2API](https://thunderstore.io/package/tristanmcpherson/R2API/) (if you haven't already)
- Place the mod in the Risk of Rain 2\BepInEx\plugins folder.

If you want to change the config
- Run the game once after installing the mod and close it out to create a config file
- The config file will be created at Risk of Rain 2\BepInEx\config
- Open the config and adjust to your liking
 


## Contact
![contact](https://i.imgur.com/gPBrPrQ.png)

## Changelog
- 1.9.3 A feature that no one uses was preventing chests from spawning under certain conditions :D
- 1.9.2 Now works with Sacrifice Artifact. Option to enable/disable in config.
- 1.9.1 Fixed a networking issue that prevented clients from interacting with the bazaar.
- 1.9.0 Update for Artifacts Update
- 1.8.0 Lunar Coins can now optionally be used instead of money to purchase items. This feature was mainly added for [TemporaryLunarCoins](https://thunderstore.io/package/MagnusMagnuson/TemporaryLunarCoins/)
- 1.7.3 Temporary incompatibility fix for ShareSuite when using money sharing (until they have a solution), since I'm getting multiple pms about this daily now.
- 1.7.2 Bandaid compatibility fix for SavedGames (Loading into the bazaar with BiggerBazaar causes some issues)
- 1.7.1 Small fix
- 1.7.0 Added configs for bazaar restrictions and an alternative price scaling mode.
- 1.6.3 Fix for ShareSuite when using money sharing (Will still only grant the person using the lunar coin the money)
- 1.6.2 Update for Hidden Realms Update
- 1.5.2	Update for Skills 2.0 Update
- 1.4.2 Added support for [StartInBazaar](https://thunderstore.io/package/MagnusMagnuson/StartInBazaar/)
- 1.4.1 The Lunar Money Exchange Pod next to the Shopkeep no longer triggers fireworks due to an incident. No Newt was (seriously) hurt.
- 1.4.0 ShareSuite is now automatically detected. ShareSuite specific config for item sharing added. 1.3.0 config "ShareSuiteFix" removed/renamed.
- 1.3.0 Added feature for [ShareSuite](https://thunderstore.io/package/FunkFrog-and-Sipondo/ShareSuite/) users (per request).
- 1.2.0 Update for Scorched Acres patch
- 1.1.0 Added Feature: Limit how many times each item can be bought depending on tier (per request)
- 1.0.1 Compatibility fix for [ShareSuite](https://thunderstore.io/package/FunkFrog-and-Sipondo/ShareSuite/). Bigger Bazaar now works when using ShareSuite also.
- 1.0.0 Added more configuration options
- 0.9.0 Compatibility fix for [AutoItemPickup](https://thunderstore.io/package/KubeRoot/AutoItemPickup/). Display items are no longer distributed.
- 0.8.2 Mod was not actually using the config setting for lunar coin conversion 
- 0.8.1 Forgot to remove a console output
- 0.8.0 Initial release (please no typos)