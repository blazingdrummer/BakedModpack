## BanditReloaded
- The most comprehensive Bandit rework yet. Highly configurable! Now with support for Vengeance!
	- Bandit's Blast skill allows him to shoot faster if you click faster, but the mod is balanced around the autofire fire rate. Mashing to click faster was enabled due to popular demand.

## IMPORTANT: READ THIS
- The host must have the mod installed for it to work.
- The config doesn't auto-update when installing new versions of the mod, so delete your config or manually change the values if you want to receive the newest balance changes.
- The first option in the config is "Enable Body Clones" which is disabled by default. Enabling this will improve compatibility with other Bandit mods, BUT will break compatibility with unmodded players and any BanditReloaded user who doesn't have it enabled. Leave this setting disabled unless you plan to ensure that every player will have it enabled.

## The Skills
- Click the images to see a short gameplay clip.
[![Default Skills](https://i.imgur.com/imisg0v.jpg)](https://streamable.com/0braj)
[![Alt Skills](https://i.imgur.com/kfuZiqg.jpg)](https://streamable.com/t0fav)

## Installation
Drop BanditReloaded.dll into \BepInEx\plugins\
Settings can be changed in BepInEx\config\com.Moffein.BanditReloaded.cfg

## Credits
mistername - Ice explosion fix
Rein - Networked damage code used in Smokebomb
Kooby521 - Skill icons
Tera - Skill icon concepts
N0TORIOUS_BLT - Bandit figurine used in the mod icon

Ping me in the RoR2 Modding Discord (@Moffein#8244) or DM me if you have any feedback!

##Changelog
`1.0.0`
- Release.
`1.0.1`
- Fixed Smokebomb not working in multiplayer.
`1.0.2`
- Hotfix for the Artifacts Update. Delete your config in BepInEx\config\ to get the new default values.
- Fixed a character select UI issue related to the Artifacts update.
- Increased Thermite Bomb cooldown from 4s to 5s to be consistent with Acid Bomb.
- Increased Asssassinate cooldown from 5s to 8s.
- Increased Assassinate min damage from 300% to 400%.
- Increased Assassinate max damage from 1800% to 2000%.
- Increased Assassinate max barrier gain from 12% to 20%.
- Reduced Lights Out debuff bonus damage from 350% to 250%.
- Fixed skills being broken in multiplayer.
`1.1.0`
- Added support for Vengeance.
- Fixed Smokebomb being able to proc items on the user when Chaos is enabled.
- Increased Lights Out debuff bonus damage from 250% to 300%.
`1.1.1`
- Fixed elite enemies instakilling Bandit due to the Chaos fix.
`1.2.0`
- Added skill icon borders.
- Fixed the Crowdfunder.
- Improved the code for fixing Chaos with Smokebomb so that it now uses the standard way of disabling self damage. It's a lot less hacky, but it has the side effect of re-enabling Chaos self damage for the "Use Vanilla Cloak" config option. If anyone happens to use that option and would like to see future support for it, ping me so that I can know there's interest.
- Added config option to swap Bandit's M1s to the vanilla Brainstalks behavior. If you enable this, Blast/Scatter won't be able to shoot infinitely while under the effects of Brainstalks.
- Added config option for Blast/Scatter bullet penetration.
- Added config option for Scatter range.
- Increased Scatter damage per pellet from 70% to 75%.
- Reduced Scatter pellet count from 8 to 7.
- Increased Scatter proc coefficient from 0.5 to 0.7.
- Reduced Scatter range from 200 to 150.
- Changed how reloading for Scatter works. The first shot will take 1s to reload, while subsequent shots will take 0.5s to reload.
- Improved how Lights Out's instant primary cooldown restoration interacts with Scatter. Instead of instantly completing the cooldown, it will now instantly reload 1 shot. This should make Scatter reload a bit faster than before when using Lights Out.
- Reduced Assassinate max barrier gain on hit from 20% to 15%.