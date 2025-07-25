## MinerUnearthed
- Adds the Miner from Risk of Rain 1, a ground up rewrite of the original Miner Mod by Gnome
- Fully multiplayer compatible and with more content planned
- Has completed item displays, including some modded items
- Has a bunch of unlockable skins and skills, as well as a challenge to unlock him
- Now includes Direseeker, a custom boss based on the original from RoR1

[![](https://i.imgur.com/PWNFE6C.png)]()

[![](https://cdn.discordapp.com/attachments/469291841859092488/780787095731437588/unknown.png)]()

[![](https://cdn.discordapp.com/attachments/747757793339244576/787552348523724830/minericon.png)]()

join the discord to share feedback/bugs- https://discord.gg/HpQB9fC
or ping/dm me- @TheTimesweeper#5727

## Overview
Miner is a high speed melee character, who uses high mobility and invincibility in fast-paced combat. 
Sounds somewhat like Mercenary, but where Mercenary slips in and out, Miner rushes in and swings wildly like a crackhead.

- His primaries, coupled with his passive `Gold Rush` encourage you to be offensive to build long kill combos.
- `Drill Charge` and `Backblast` are high mobility options with invincibility during and slightly after their dashes. 
- `Drill Charge` will always go the full distance, and increases damage by being held to charge longer.
- `Backblast` can be held to go backwards farther. Use as a long mobility option, or to stay in combos.
- `To the Stars`, when used correctly, can land huge damage on larger enemies.

Read Gnome's original mod page for more detailed descriptions. Gameplay is still the same for the most part

## Direseeker
Adds a custom boss, Direseeker, along with Miner. Disables itself if the standalone Direseeker mod is installed. The one included in this mod is basically Direseeker lite.

Direseeker is a massive Elder Lemurian with currently a new extremely powerful fireball attack. It's roughly Imp Overlord tier and only spawns on Abyssal Depths.

[![](https://cdn.discordapp.com/attachments/469291841859092488/784510230054436904/unknown.png)]()

[![](https://cdn.discordapp.com/attachments/469291841859092488/784511696118218812/unknown.png)]()

[![](https://cdn.discordapp.com/attachments/747757793339244576/783952180834992128/direIconRed.png)]()

## Credits
Gnome - Made the original Miner mod, a fantastic base to work off of  
fuu - Made the Miner model  
rob - coding, rewrite, polish  
TheTimeSweeper - coding, adrenaline flame particles, maintaining  
Moffein - help fix for CUM2, maintaining  
PapaZach - Skill icons  
Jot - CSS animation  
redacted - Grand Mastery skin  
bruh - Swag model  
Neik - Blacksmith concept  
Ruxbieno - Direseeker logbook entry  
Christian Gentry - Anvil model  
JunJun_W - Chinese Translation  
Адский Шкед and Hexxedude - Russian Translation  
Damglador - Ukrainian Translation  
Donitodorito - Portuguese Translation
Juhnter - Spanish Translation

## Future Plans 
- Gnome's Alt Special
- Skills++ and other fun stuff
- update skins
- fix rig
- help

## Changelog

`1.9.10`

- Tweaked broken anim fix to prevent accidental detonations.

`1.9.9`

- Fixed broken anims on dedicated servers.
- Direseeker
	- Now disabled by default due to confusion about this mod's Direseeker and the standalone one. (Existing configs unchanged)

`1.9.8`

- Updated RU tl (Thanks hexxedude!)

`1.9.7`
- forgot spanish translation in last update, sorry Juhnter!

`1.9.6`
- added UA translation from Damglador
- added pt-BR translation from Donitodorito
- been a while since I touched this so let me (Timesweeper) know if I fucked something up

`1.9.5`

- AssetBundle/Soundbank are no longer embedded in the DLL to reduce RAM usage.
- Updated skill icons (Thanks PapaZach!)
- Added RU translation from Адский Шкед

`1.9.4`

- Cave In
	- Fixed error spam when hitting the Sky Meadow rocks.

`1.9.3`

- Updated Meteor Shower skill icon.

`1.9.2`

- Crack Hammer
	- Reduced shorthop velocity from 24 -> 18 so that it doesn't launch you out of reach of enemies.

`1.9.1`

- Added placeholder icon for Meteor Shower Special.

`1.9.0`

- Visuals
	- Miner's visor now glows by default, like in RoR1.
	- Textures are no longer grainy.
	- Changed Blacksmith colors to be closer to the Starstorm sprite.

- Language files now contain all tokens.
	- Removed LanaguageAPI dependency.
	
- Crack Hammer
	- Increased hitbox size
	- Increased blast radius from 10m -> 12m
	- Increased damage from 2x200% -> 2x240%.
	- Removed chargeup since it didn't actually do anything.
	- Increased shorthop velocity on hit from 12 -> 24
	
- Cave In
	- Now uses the same input behavior as Backblast. (Hold the button to go further.)
	- Rewrote enemy pull code. Should be way more consistent now.
	- Changed VFX to make it more clear that the skill doesn't actually deal damage.
	
- To The Stars
	- Improved ability to hit flying enemies.
		- Increased internal BulletAttack radius to cover most of the explosion radius
			- The ability works by firing bullets directly downwards in a star pattern around Miner. Bigger radius = higher chance to hit flying enemies in the attack's path. One quirk of this method is that the explosion hitbox will be placed at the center of the hitbox that the bulletattack collides with.
	- Now applies downwards force to enemies hit by the explosions.

`1.8.8`

- Remembered to set CachedName field in SurvivorDef. Hopefully this will fix Eclipse progress not saving.

`1.8.7`

- Fixed CSS animation

`1.8.6`

- Fixed Miner getting re-locked if you have Direseeker installed.

`1.8.5`

- Removed LanaguageAPI completely.
- Added Chinese translation (Thanks Edge-R!)
	- Unlock strings are missing since they were added after the translation was done.

`1.8.4`
- fixed missing diamond picks
- fixed missing anvil
  - couldn't find the original so I just downloaded a new one
- fixed miner disappearing at certain camera angles

`1.8.3`

- Fixed missing Scepter skill icons.

`1.8.2`

- Fixed missing ending text.

`1.8.1`

- Fixed Adrenaline adding to Move Speed Multiplier instead of Base Move Speed.
- Now uses a language file for strings. Looking for translators!
	- This will break skill description numbers dynamically updating based on your config, but you can manually edit the language file to reflect your changes.

`1.8.0`

- Tweaked wording on skills.
- Skill selections now save when closing the game.
- Now uses DamageAPI and RecalculateStatsAPI, which should improve compatibility with other mods.
- Fixed the skin with the "Rallypoint Delta in 8 minutes" unlock condition using real time instead of the run stopwatch.

- Stats
	- Reduced HP Regen from 2.5 (+0.5) -> 1.0 (+0.2)
	
	*Previous change didn't consider the passive's regen bonus.*
	
- Gouge
	- Reduced damage from 275% -> 270%
	- Now interacts with Shuriken
	
	*Skill is coded in a weird way, so a hacky fix was done for Shurikens.*
	
- To The Stars (Rework)
	- Now creates 6 explosions below you that deal 300% damage each.
	- Spacing and shot pattern is always consistent regardless of the height you use it from.
		- Can't shotgun with it, but always has good coverage against crowds.
	- Old version of the skill has been moved to an alt skill.
	
	*Making this work more like RoR1. More consistent, lower damage potential than the alt. Feedback would be good.*
	
- Meteor Shower (Alt Special)
	- TODO: Icon
	- Jump into the air, shooting a spray of shrapnel downwards for 15x160% damage.
		- Damage increased from 90% -> 160% (overall damage has decreased slightly)
		- Shotcount reduced from 30 -> 15 to reduce lag with on-hits
		- Increased shot radius from 0.35 -> 0.5 to compensate for lower shotcount
		- Increased proc coefficient from 0.5 -> 0.7

	*Moved this to the alt slot due to being more finnicky to use compared to the reworked To The Stars.*

`1.7.0`

- Stats
	- Changed HP from 120 (+48) -> 140 (+42)
	- Increased HP Regen from 0.5 (+0.25) -> 2.5 (+0.5)

*Giving Miner consistent scaling with the rest of the survivor roster.*

`1.6.10`

- Direseeker compat fix.
- Grandmastery can now unlock on Inferno.
- ClassicItems Scepter support.

`1.6.9`
- nice
- fixed bug with r2api update (thanks to Moffein for the help)
- fixed direseeker boss and survivors' skills
- added a few void item displays

`1.6.8`
- fixed me uploading the wrong file for the last 2 versions

`1.6.7`
- made grandmastery skin achievable on eclipse
- fixed missing gouge icon
- fixed me lying about the gold rush icon last time
- made hithop scale with attack speed so you don't uncontrollably float anymore
- slight buff to Crush, it was under in dps when gouge's gouge was taken into account

`1.6.6`
- added new icon for Gold Rush passive
- fixed error spam about items when miner is installed

`1.6.5`
- fixed special using up all stacks
- fixed emission on materials whitewashing him
- added weakpoint for snopers to hit
- item displays weren't removed after all guau

`1.6.4`
- fixed for The Second CUMming
- sounds had to be redone. let me know if they're too loud/quiet/missing anywhere
- tweaked m1 anims again
- added impact sound to Crush m1
- tweaked menu sound to actually kinda be in timing now

`1.6.3`
- fixed unlockableapi

`1.6.2`
- Fixed cave-in not networked
  - niggas put `networkserver.active` inside a `isauthority` lol
- Didn't implement new skins cause I don't have time
  - cough cough

`1.6.1`
- CRUSHHUNLOCKABLE

`1.6.0`
- fixed all achievements
  - networked crush achievement
- fixed direseeker survivor config breaking everything
  - made direseeker survivor use the other mod version if it's installed
- fixed giant item displays in a try{}. it'll work when r2api updates

`1.5.4`
- Fixed all item displays. Thanks minka for reaching out about them
- Fixed modded item displays for aetherium and sivsitems
- as well as fuckhuge ancient scepter and golden coast items
- supply drop fuck you for having a plague mask forcing me to do your displays too - timesweeper xoxo

`1.5.3`
- Updated to work on the latest RoR2 version

`1.5.2`
- Updated to work on the latest RoR2 version
- Item displays and achievements broken for now

`1.5.1`
- Removed ClassicItems support and instead migrated to the Standalone Ancient Scepter

`1.5.0`
- Made Crush an actual skill (thanks Timesweeper!)
- Added Grand Mastery skin (model by redacted)
- Emotes can no longer be used while chat is active (thanks DestroyedClone for the fix)
- Updated primary skill icons
- Tweaked walk animation
- Networked Gouge hit sounds
- Fixed Crack Hammer animation being broken in multiplayer
- Replaced most instances of Miner in the code with Digger in another fruitless attempt to get Windows Defender to fuck off :]]]]

`1.4.4`
- Changed the internal name to DiggerUnearthed, hopefully stops this antivirus nonsense
- Fixed clients taking fall damage when using Falling Comet
- Fixed Gouge second swing taking longer than the first swing, moderately improving dps

`1.4.3`
- Changed the dll filename to stop antivirus falseflagging (it is seriously not a bitcoin miner..)

`1.4.2`
- Added drip
- Updated character portrait
- Changed unlock condition to killing Direseeker when Direseeker standalone is installed
- Tweaked some animations and VFX
- Tweaked skill icons
- Fixed Aetherium item displays
- Fixed clients suffering from fall damage when using Falling Comet
- Fixed Gouge creating duplicate effects in multiplayer and properly networked swings

`1.4.1`
- Direseeker now exists as a separate mod, so this one will disable itself if you have both mods installed- otherwise unchanged

`1.4.0`
- Updated Direseeker visuals, added some extra flair
- Increased Direseeker's fireball damage, increased fireball count to 15 and increased spread
- No longer counted as a boss when spawned normally
- Some more Survivorseeker fixes
- Fixed Miner's model being positioned slightly above the ground
- Made Miner: Tempered achievement a little more reasonable

`1.3.9`
- Fixed Direseeker survivor for real this time
- Tweaked Direseeker textures
- Reverted Blacksmith textures

`1.3.8`
- Accidentally left Direseeker survivor enabled by default, oops
- Fixed the survivor to actually work and interact with things

`1.3.7`
- Reverted Life Savings nerf- didn't work as intended, will figure something else out
- Added a custom boss, Direseeker

`1.3.6`
- Added a new skin
- Adrenaline glow now properly smooths from white to red, now applies on Tundra and the new skin added
- Updated some skill VFX
- Fixed Falling Comet applying fall damage to clients and stopped weird physics nonsense
- Added a new emote(bound to 3 by default)
- Fixed Miner's logbook display using the wrong shader

`1.3.5`
- Fixed infinite adrenaline bug because I can't code apparently
- Pickaxe/visor glow now transitions smoothly just like the adrenaline animations
- Fixed inaccurate Drill Charge description

`1.3.4`
- Nerfed Life Savings interaction- now requires a minimum of 3 gold earned to count towards adrenaline stacks
-- Goal isn't to kill the interaction but to stop it from breaking runs so easily with just one stack
- Reverted Crack Hammer sound
- Added config for primary damage and secondary damage/cooldown
- Tweaked adrenaline animations
- Fixed adrenaline visuals no longer working for clients

`1.3.3`
- Fix an issue with Backblast

`1.3.2`
- Adrenaline visuals now transition smoothly
- Locked alt skills behind challenges
- Changed Tundra skin unlock to reaching Rallypoint Delta in under 8 minutes
- Added Puple skin back
- Fixed emotes giving adrenaline stacks

`1.3.1`
- Miner is now locked- can be force unlocked via config
- Updated portrait
- Added some more adrenaline eye candy

`1.3.0`
- More animation work
- Finished item displays and added display rules for Siv's Items and Aetherium
- Added an upgraded special for ClassicItems' Ancient Scepter- Falling Comet: Jump into the air, shooting a wide spray of explosive projectiles downwards for 30x90% damage total, then fall downwards creating a huge blast on impact that deals 1500% damage and ignites enemies hit.
- Added a new skin(must be enabled via config)
- Added a ton of visual feedback for adrenaline passive
- Gouge moved to default primary slot, added a stacking armor debuff that's soft capped by attack speed
- Updated Drill Charge and Crack Hammer VFX
- Crack Hammer cooldown lowered to 4s, damage lowered to 2x200%, hitbox size decreased to stop accidentally getting caught on enemies
- Lowered To he Stars projectile count to 30
- Buffed Backblast damage to 600%
- Improved Cave In's reliability
- Added two emotes, bound to 1 and 2 by default
- Updated character portrait

`1.2.0`
- Cleaned up animations
- Updated Molten skin
- Lowered Crush damage to 225%
- Added alternate primary, secondary and utility skills
- Added some extra skins, must be toggled on via config
- Added configuration for Gold Rush passive
- Fixed Backblast effect sometimes not appearing
- Fixed Resonance Disc's item display	

`1.1.0`
- Nerfed passive attack speed
- Reduced Crush duration, buffed air stall slightly
- Increased projectile size on To The Stars to help with hitting smaller enemies
- Fixed compatibility with Aatrox
- Added agile keyword to Crush
- Added a couple more display rules and some visual tweaks
- Properly anchored picks to the hands

`1.0.0`
- Initial release