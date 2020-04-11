# Rampage
#### By iDeathHD

`NEW` **ADD A CUSTOM RED-TIER ITEM !**

A mod that introduces the Rampage mechanic from Path of Exile.

Rampage is a kill streak mechanic, upon reaching specific number of kills when you have the Red-Tier Item called Bisco's Leash, special effects are activated. From fire orbs coming from your character to temporary beetles helping you.

### Informations

- You need to get the red-tier item to have the Rampage mechanic activated, called Bisco's Leash ;)

- The default timer before the rampage streak reset is 12 seconds, if you launch the game atleast one time with the mod installed, a config file should be created so you can change this timer if you want !

- UI is configurable in the config file.

- If you find any bug / have feedback about the mod, tell me about it in the RoR2 Modding Discord @iDeathHD

### Installation Guide

- Copy `Rampage` folder to your BepInEx plugins folder.

MiniRpcLib (made by Wildbook) is a networking library that will allow this mod to work in multiplayer.

### Current Rampage Tiers

In addition of getting specifics rewards for reaching tiers, your character will get :

- 1% (+1% per item stack) increased Movement Speed per 20 Rampage Stacks
- 2% (+2% per item stack) increased Damage per 20 Rampage Stacks

The rampage stack is not capped.

| Tiers                      | Required Kills |                                                       What do they do      |
| :------------------------: | :------------: | ---------------------------------------------------------------------------: |
| 1                          |       15       |2 nova of 15 fire orbs comes from the player in a rapid succesion        |
| 2                          |       30       |Detonate all enemies in a 100 unit radius                                     |
| 3                          |       45       |Summon 1 beetle for 30 seconds                                                |
| 4                          |       70       |Detonate all enemies in a 100 unit radius and summon 5 drones for 25 seconds  |
| 5                          |       100      |2 nova of 15 lightning orbs comes from the player in a rapid succession       |
| 6                          |       135      |Summon 10 backup drones for 25 seconds                                        |
| 7                          |       175      |5 novas of 15 fire orbs comes from the player with 1 second delay        |
| 8                          |       220      |Summon 2 beetles for 30 seconds                                               |
| 9                          |       270      |Detonate all enemies in a 100 unit radius                                     |
| 10                         |       325      |Detonate all enemies in a 100 unit radius and summon 2 beetles for 30 seconds |
| 11                         |       385      |5 nova of 15 lightning orbs comes from the player in a rapid succession       |
| 12                         |       450      |2 quick detonations in a 100 unit radius                                      |
| 13                         |       520      |5 nova of 15 fire orbs comes from the player, 10 drones, and detonation  |

### Changelog

`1.1.4` - Updated for the Artifact Update.

`1.1.3` - Fixed compatibility issue with Dedicated Server.

`1.1.2` - Fixed compatibility issue with the ItemTierSelection mod.

`1.1.1` - Updated for the latest R2API Release and December Game Update.

`1.1.0` - Updated for the latest R2API Release.

`1.0.9` - Updated for the 2.0 Skills Game Update.

`1.0.8` - Fixed an issue with the host being dead while other Enginner survivors getting kills not having their rampage stacks register correctly.

`1.0.7` - Added the 3d model to show up on survivors model.

`1.0.6` - Compatibility fix for upcoming mad engineer mod.

`1.0.5` - Updated to the latest version of the game. Cleaner code for finding the user body, fix for multiplayer client not having their damage or movespeed boosted on a rampage streak, now fully depend on the host for projectiles firing. Fix for the Enginner turrets giving rampage stacks without the item.

`1.0.4` - Minor bug fixes about the sticky bombs being all invisible and worm bosses having their projectile behavior modified.

`1.0.3` - A bit cleaner code and better description for the item.

`1.0.2` - Stacking the item now has stacking effects.

`1.0.1` - UI is now configurable in the config file.

`1.0.0` - Add a red-tier item in the game.

`0.0.10` - Updated to the latest version of MiniRpcLib.

`0.0.9` - Oops, pressing W was giving rampage stacks.

`0.0.8` - Added a configuration parameter for changing the timer of the rampage streak.

`0.0.7` - Should have tested the AllyPing fix before... Now should work !

`0.0.6` - The mod wasn't compatible with AllyPing mod with the last update fix to Engi turrets, it now should work ! Also changed some tiers : some use fire balls instead of lightning ones. Tier 1 : Now 2 delayed waves so you can aim some of the balls into monsters. Tier 2 radius : 50 -> 100 units. Tier 4 now spawn 5 drones. Tier 5 fixed so the balls doesnt spawn all at once, from 1 wave of balls to 2 waves.

`0.0.5` - Different technique for calculating distances, removing attached scripts to GameObject when not needed, and the most important of all, Engi turrets give rampage stacks !

`0.0.4` - Hopefully fixed the first tier not launching...

`0.0.3` - Fixed crashes related to the Lightning Balls. Made in a more Unity-esque way. ;)

`0.0.2` - Fixed the timer going down when the game was paused.

`0.0.1` - Initial release of the mod.