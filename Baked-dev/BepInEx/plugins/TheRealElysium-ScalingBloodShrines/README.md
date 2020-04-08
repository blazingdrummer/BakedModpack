# ScalingBloodShrines

This is a simple mod which makes blood shrines viable all the way in to the late game.

If the game director is using credits to spawn something, I figure it should at least be worthwhile.

## How it works

In vanilla, you are rewarded money equal half of the HP you sacrifice to the shrine.

`0.5 * SacrificedHP = money`

This is works fine at the start of the game, but as you progress further the cost of things quickly outpaces the rate at which your HP goes up.

ScalingBloodShrines resolves this by using the cost of interactables on the current map to determine how much a blood shrine should reward.

`(((InteractableCost * ConfigAmount) / MaxHP) / 2.18) * SacrificedHP = money`

ConfigAmount default is 4.  This value represents a chest.

This means you will be rewarded with enough money to open 4 chests after having used an entire blood shrine.

This formula has a floor of 0.5 so it will never give you less than what vanilla does.

2.18 represents the entirety of a blood shirne. (0.5 + 0.75 + 0.93)

In a 4 player game, this will likely result in a buff to blood shrines from the very start with the default value.

## Configuration
1. **Make sure you run the game with the mod installed to generate the config file**
2. Navigate to `\Risk of Rain 2\BepInEx\config\`
3. Open `com.Elysium.ScalingBloodShrines.cfg` in any text editor
4. Edit the values for the setting as you see fit!

You can also set the setting in-game with the command listed below.

sbs_chests value (value can be 0.1 or higher, do not recommend going below 1 however.)


## Installation Guide

- Copy the `ScalingBloodShrines.dll` file to your BepInEx plugins folder.


## FAQ

**I want to play this with my friends. Do they also need to install this mod?**

*No, only the host requires this mod to function. It will do nothing if you are not the host.*

---

**How do I configure the mod while the game is running?**

*Open up the console window (``ctrl + alt + ` ``). All commands starts with `sbs_` and will autocomplete.*


## Bug Reports, Suggestions & Feedback

Please feel free to contact me for suggestions/feedback/bug reports on discord *`Elysium#5804`*.

## Changelog

`1.0.1` - Updated readme. Credits to Harb for making the mod icon! <3

`1.0.0` - Initial release.
