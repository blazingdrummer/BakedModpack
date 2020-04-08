# ShrineOfDio

This mod replaces the Shrine of the Woods with the Shrine of Dio, which lets you resurrect fallen teammates.
Depending on the setting in the config, you can pay with gold or offer a Dio's Best Friend to the Shrine.


## Features
- Each Stage spawns with a Shrine of Dio
- Resurrect fallen teammates on use
	- Player is chosen randomly
- Choose via config whether you want to resurrect using gold or an offering of Dio's Best Friend
	- The gold cost can be adjusted in the config as well
	- The cost scales with difficulty (like everything else), but not with repeated usages


## Limitations
- If a client does not have this mod installed, Shrine of Dio will still work, but the text displayed will be incorrect. 
	- Additionally, if choosing to pay the Shrine with Dio's Best Friends, the interactability glow might be incorrect.

Therefore it's recommended that everyone has the mod installed to avoid confusion.

## Installation

- Install [BepInEx Mod Pack](https://thunderstore.io/package/bbepis/BepInExPack/)
- Copy 'ShrineOfDio.dll' into your Risk of Rain 2\BepInEx\plugins folder
- Run the game once and close it out to create a config file
- The config file will be created at Risk of Rain 2\BepInEx\config
- Open the config and adjust to your liking

## Contact
![contact](https://i.imgur.com/gPBrPrQ.png)


## Changelog
- 1.3.2 Disconnected players were not taken out of the pool of possible resurrection targets
- 1.3.1 Forgot to remove some testing stuff that broke things
- 1.3.0 Update for Artifacts update
- 1.2.0 Update for Hidden Realms update
- 1.1.0 Update for Scorched Acres patch
- 1.0.1 Fixed another small display issue and removed MonoMod.Utils.dll since BepInExOack 2.0.0 is out
- 1.0.0 Fixed client side displaying issues and no price tag shows up for Dio's Best Friend using mode
- 0.9.3 Some shrines had a wrong gold cost in specific situations.
- 0.9.2 I'm an idiot and made a confusing mistake in the config description about when the gold cost value is used/active
- 0.9.1 Added contact info
- 0.9.0 Mod deactivated for Single Player
- 0.8.0 Shrine of Dio upload
