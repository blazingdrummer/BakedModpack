## Heretic

Adds the Heretic as a selectable survivor with stats balanced around the base cast.

Grab all 4 Heresy items in a run to power up and acquire the Mark of Heresy!

We are looking for translators! Check the languages folder on the [GitHub](https://github.com/Moffein/HereticMod/tree/master/language) if you would like to submit a translation for your language.
Current Supported Languages: English, Spanish, Simplified Chinese, Russian

[![](https://i.imgur.com/zX96kAC.jpg)]()
[![](https://i.imgur.com/INtd4VY.png)]()

Squawk button can be assigned in the in-game options menu!

## Changes from Vanilla

*Note: The first stack of all Heresy items will have no effect on the Heretic, as they are replacing her existing skills. This behavior was chosen for the sake of internal consistency (otherwise, there'd need to be a bunch of different cases for how Heresy items work if you spawn as Heretic or if you pick them up and become the Heretic mid-run).*

- Base Stats
	- HP reduced from 440 -> 110
	- Damage reduced from 18 -> 12
	- HP Regen increased from -6 -> 1

- Visions of Heresy's reload scales with Attack Speed instead of Cooldown.
	- Can be toggled in the config.
	- If RiskyMod is installed, the Visions changes from this mod will take precedence.
	
- Mark of Heresy (New Item)
	- Automatically granted when all 4 Heresy items are collected up in a single run.
		- Cannot be cleansed, printed, stolen, or removed.
		- Happens at the same time as the Heretic transformation.
	- Increases HP 4x
	- Increases damage by 50%
	- Reduces your base regen all the way to -6HP/s (value used for Rainstorm) regardless of difficulty.
		- Unaffected by Tonic as well.

## Installation

Drop the Moffein-Heretic folder into \BepInEx\plugins\

## Credits

Code - Moffein

Spanish Translation - Anreol

Simplified Chinese Translation - WockyTheWolf, JunJun_w

Russian Translation - Drochuagon

French Translation - HolographicWings

German Translation - juppytaar

Portuguese Translation - Kauzok

## Changelog

`1.2.2`

- Added BR translation (Thanks Kauzok!)

`1.2.1`

- Added DE translation (Thanks juppytaar!)

`1.2.0`

- Mark of Heresy
	- Changed how the damage increase works internally.
		- Old Behavior: Add +50% to your damage multiplier.
		- New Behavior: Add +50% base damage and level damage.
		
	*This is a more correct way of increasing the damage, since a lot of damage-affecting items additively increase the damage multiplier, which resulted in a very different damage value from Vanilla Heretic.*

`1.1.11`

- Added FR translation (Thanks HolographicWings!)

`1.1.10`

- RiskOfOptions is now a SoftDependency.
- Set RiskOfOptions icon.
- Changed default sort position to after Captain, since she's a part of the RoR2 basegame.
	- This will not affect existing configs.

`1.1.9`

- Improved Squawk responsiveness.

`1.1.8`

- Mark of Heresy negative regen is now divided by Curse Penalty so that you don't instantly die when playing with the Artifact of Glass.

`1.1.7`

- Updated Russian translation.

`1.1.6`

- Updated Russian translation.

`1.1.5`

- Updated readme and DLL version number.

`1.1.4`

- Added Russian translation (Thanks Drochuagon!)

`1.1.3`

- Added Simplified Chinese translation (Thanks WockyTheWolf and JunJun_w!)

`1.1.2`

- Fixed unlock condition triggering when beating the game as any survivor.

`1.1.1`

- Added spawn protection for up to 0.5s after Heretic's spawn animation ends.

`1.1.0`

- Added unlock condition: Escape the moon as the secret survivor.
	- Added Force Unlock config option to skip this.

`1.0.7`

- Fixed Squawk button being broken online due to the previous update.

`1.0.6`

- Fixed a minor nullref related to Essence of Heresy.

`1.0.5`

- Fixed Mark of Heresy instantly killing you when Transcendence/Perfected Affix is equipped.

`1.0.4`

- Mark of Heresy
	- Improved negative regen code. Now is completely unaffected by regen multiplier items (MonsoonHelper, DrizzleHelper, Tonic, etc.).

`1.0.3`

- Tweaked Ruin Skill Description styling.
- Added Spanish translation (Thanks Anreol!)

`1.0.2`

- Fixed Vanilla typos/styling with the Secondary/Special skill descriptions.
	- Can be disabled in the config.

`1.0.1`

- Character Select Sort Position added to config file.

`1.0.0`

- Release.