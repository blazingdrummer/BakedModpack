If you have any issues, contact me on discord (@Rein#7551)

## New this update:
- Dealt with the secret breaking changes in most recent R2API...

## General information

### Install
- Delete old versions. (You never know)
- Unzip the plugin zip.
- Copy all files to the plugins folder in Bepinex(in your game install directory)
- Bonus points if you create a separate folder inside the plugins folder for every mod

### Uninstall
- Delete the files that come with the mod from the plugins folder

### Multiplayer compatibility
All players must have this mod installed in order for it to work in multiplayer. Mods like unmodded clients or setbuildid are not sufficient.

### New this update
- Compatibility with Artifacts update
- Temporairly disabled the new skin while I switch over to my new framework.
- Re-enabled item display, some items will hover weirdly where jetpack was but all will work at least.

## Mod Overview
This mod adds new passive to Artificer that can be selected from the loadout menu in character selection. The new passive is aimed to play in to a grounded, close-range playstyle and offers considerable utility and damage over ENV Suit.

In addition to the passive, this mod does the following:
- Adds a fancy new skin and fixes some clipping issues on the Artificer model.
- Reworks Ion Surge to be viable for use with both the old and new passive.
- Makes Nano Bomb into a more distinct ability relative to Nano Spear.

### The new passive
There are three parts to the passive, one for each element. The number of skills selected for each element increase the power of that portion of the passive.
- Fire grants a stacking temporary buff on skill cast that increases the damage dealt by burn ticks. The number of stacks per cast scales with power.
- Ice causes enemies that die while frozen, or are killed by Ice damage, to create a delayed area freeze. The size of the area scales with power.
- Lightning fires homing projectiles on every skill cast. The number fired per cast scales with power.

### Ion Surge rework
Without ENV Suit, Ion Surge became entirely non-viable. Rather than just delete it entirely, I decided to keep it as a way to enable a much higher mobility playstyle for Artificer. Of course, choosing Ion Surge comes at the cost of Flamethrower, which is a very high damage skill.
- Now consists of three recurring dashes. The direction of each dash is controlled by the direction you aim, along with movement keys (including jump)
- During the time between each dash you hover in the air.
- All other skills can be cast at all times during the dashes, or while hovering.
- The three dashes occur automatically after first activation.
- No longer deals damage or stuns.

### Nano Bomb tweaks
Nano Bomb and Nano Spear were far too similar in my opinion. In order to make Nano Bomb more unique, I made the following changes:
- Projectile is now affected by gravity, this means you need to arc it towards a target.
- Explosion has significantly larger radius, meaning that it excels at clearing large groups of enemies.
- In addition to the larger explosion, the arcing lightning also can bounce one time, occurs at a longer range, and also occurs more frequently.


## Future Plans
- A variant for each element in each slot. This is a fairly massive undertaking overall, so it may be a while before I do so.
- Some more skins (Let me know if you have any color requests in particular)


## Changelog
### 1.1.0
- Compatibility with Artifacts update
- Temporairly disabled the new skin while I switch over to my new framework.
- Re-enabled item display, some items will hover weirdly where jetpack was but all will work at least.

### 1.0.5
- Dealt with the secret breaking changes in most recent R2API...

### 1.0.4
- Updated to make use of new APIs in R2API.
- Swords now detonate sooner after impact and home in a bit more reliably.

### 1.0.3
- Skin updated to be interesting.
- Targeting for lightning spears is much smarter.
- Fixed various errors.
- Code cleanup.
- Ion surge now dashes a tiny bit less distance.

### 1.0.2
- Can switch between the old and the new passive in the loadout menu.
- Jetpack removal only applies when new passive is selected. (Still applies the clipping error fixes)
- Ice explosions have a 50% larger radius.
- Removed a few of the models used for the lightning missiles (They just didn't fit in my opinion)
- Added checks while loading to verify that the required SubModules are enabled.
- Added checks that ensure that the selections for skins and skills are not saved to your profile, preventing potential issues during game load in vanilla.

### 1.0.1
- Dramatically improved consistency of ice passive triggering.

### 1.0.0
- First release
