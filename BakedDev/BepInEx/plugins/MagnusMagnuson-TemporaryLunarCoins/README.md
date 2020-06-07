# TemporaryLunarCoins

This mod makes Lunar Coins reset every run with options for drop chance and multiplier. 
Since [LoonerCoins](https://thunderstore.io/package/paddywan/LoonerCoins/) is deprecated and someone asked me about it, I decided to make a simple and more basic version.
It borrows part of an IL hook from LoonerCoins, so credit for that goes to them.

## Features
 - Makes Lunar Coins temporary by resetting at the beginning of every run.
	 - Participating players are frozen in place at the beginning of the game until everyone agrees to reset their lunar coins (to prevent griefing)
 - Drop chances and multiplier can be set via config.


## Installation

- Install [BepInEx Mod Pack](https://thunderstore.io/package/bbepis/BepInExPack/) (if you haven't already)
- Install [R2API](https://thunderstore.io/package/tristanmcpherson/R2API/) (if you haven't already)
- Place the mod in the Risk of Rain 2\BepInEx\plugins folder.

Only the host requires this mod.

If you want to change the config
- Run the game once after installing the mod and close it out to create a config file
- The config file will be created at Risk of Rain 2\BepInEx\config
- Open the config and adjust to your liking
 
## TODO / Issues
- There seem to be incompatibilities with certain mods
- Late joiners are not required to have their lunar coins removed
- Being lazy

## Contact
![contact](https://i.imgur.com/gPBrPrQ.png)

## Changelog
- 0.2.1 Feature Request: Automatic removal of coins in single player mode via config. Additionally, "tic_aye" will now also be accepted as command.
- 0.2.0 Update for Artifacts Update
- 0.1.0 Initial release
