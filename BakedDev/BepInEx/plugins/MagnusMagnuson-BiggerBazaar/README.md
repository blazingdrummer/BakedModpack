# BiggerBazaar

[Host only/Server-side]

This mod expands the bazaar with items to purchase. Use money or alternatively lunar coins to purchase items. 

![shop](https://i.imgur.com/2q9jTri.jpg)
![exchange](https://i.imgur.com/0HVfreX.jpg)

## Recent feature

-


## Features

 - up to 6 random items are available for purchase
	 - Base cost and rarity for each tier can be adjusted in the config file
	 - Cost scales with difficulty (if using money)
	 - Limit how many times each item can be bought by tier
	 - Restrict the amount of total purchases and/or purchases per tier per player
 - Use money you have left at the end of the stage... 
	 - When you take the bazaar portal, your money is not converted into experience points. Instead you keep it to buy items at the bazaar. Money left when you then leave the bazaar is converted into experience points
 - or use Lunar Coins. Consider trying it out with [~~TemporaryLunarCoins~~](https://thunderstore.io/package/MagnusMagnuson/TemporaryLunarCoins/) [Ephemeral Coins](https://thunderstore.io/package/VarnaScelestus/Ephemeral_Coins/)
 	- Cost can be configured and does not increase
 	- Cost of vanilla shops can be adjusted
 - You can exchange Lunar Coins for money at the friendly Shopkeeper
	 - You can adjust the amount of money in the config. Setting this value as the same as e.g. a tier 1 item means one Lunar Coin always gives you enough money to buy a tier 1 item
	 - You can limit the amount of exchanges, completely remove them or have infinite
 - Only the host is required to have the mod installed
 - If you're using ShareSuite, you can choose in the config whether bought items are shared or not by setting "ShareSuiteItemSharingEnabled" to true or false. Automatically turned on when sharing money.
 - Compatibility with [ForesightArtifact](https://thunderstore.io/package/SpacePotato/ForesightArtifact/). 
 - Now all tiers and equipment can spawn if configured. Config file is reorganized which probably reset your configs (sorry). Old config should be at the bottom of the file.
 - Interoperability with [ItemDropList](https://thunderstore.io/package/Phedg1Studios/ItemDropList/). Only allows the selected items in the shop.


## Installation

(if not using a mod manager)

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
- 1.13.7 Lunar Pod wasn't working properly with Ephemeral Coins.
- 1.13.6 Fix for update.
- 1.13.5 Compatibility withg BetterUI. 
- 1.13.4 Added option to limit the amount of bazaar chests to spawn
- 1.13.3 ShareSuite money sharing fix (I hope)
- 1.13.2 Edge case ShareSuite compatibility fix. You probably never even had this issue. 
- 1.13.1 ShareSuite compatibility fix 
- 1.13.0 Update for recent patch.
- 1.12.13 Back to using R2API with Hookgen, since standalone MMHOOK has no more active functionality
- 1.12.12 Now only depends on the standalone MMHOOK and no longer R2API/ET.
- 1.12.11 Added version for Enigmatic Thunder (found in the corresponding zip). Only use one one
- 1.12.10 Fixed issue with new ShareSuite version. Should work again.
- 1.12.9 Fixed a recently introduced bug that broke the golden chest from [BazaarExpand](https://thunderstore.io/package/NetherCrowCSOLYOO/BazaarExpand/).
- 1.12.8 Fixed a bug that would prevent (lunar) equipment from being awarded when turning off ShareSuiteItemSharingEnabled. Thanks emtkmkk for reporting!
- 1.12.7 Fixed a recently introduced bug that would prevent certain chests from giving items. A scene check wasn't working properly.
- 1.12.6 Compatibility fix for [ForesightArtifact](https://thunderstore.io/package/SpacePotato/ForesightArtifact/). Changed chest tier costs to a multiplier as part of it. Current values have been automatically converted, so no need to change.
- 1.12.5 Turned off ShareSuiteItemSharingEnabled being set to true automatically when using ShareSuite money sharing, since lunar mode exists.
- 1.12.4 Fixed incorrect amount of money issue with ShareSuite money sharing when host dies and party goes to the bazaar.
- 1.12.3 Lunar mode was not displayed as requiring lunar coins on client. Changed chests to lunar chests for lunar mode.
- 1.12.2 "original bazaar" config wasn't displayed properly for clients.
- 1.12.1 A "original bazaar" config wasn't working. Wow, great testing Magnus. Good job.
- 1.12.0 Added some configs. Lunar price for vanilla bazaar shop can now be changed and some other small config options found under "Other".
- 1.11.1 Another weird edge case compatibility issue with ShareSuite where chests would spawn wrong items was fixed.
- 1.11.0 Reworked some stuff. Now all tiers and equipment can spawn if configured. Organized config.
- 1.10.2 Changed Bigger Bazaar to not spawn any chests if tier 1, 2 and 3 are disabled by ItemDropList, rather than spawning random items.
- 1.10.1 Forgot an exclamation mark, breaking money transfer when using ShareSuite with money sharing :^)
- 1.10.0 Added some basic interoperability with [ItemDropList](https://thunderstore.io/package/Phedg1Studios/ItemDropList/).
- 1.9.8 Added a config for ShareSuite. maxPlayerPurchases now affects the whole party by default.
- 1.9.7 Decided to instead just leave a message in the log :^) Sorry for spam. Everything works
- 1.9.6 Nevermind last change. Hook is too early affecting proper functionality. Will fix false positive issue later.
- 1.9.5 Changed a hook entry point to avoid false reports
- 1.9.4 Added Network Compatibility Level
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