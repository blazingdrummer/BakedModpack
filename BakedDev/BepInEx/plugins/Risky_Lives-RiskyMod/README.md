## RiskyMod
A full-game overhaul that aims to bring it closer to RoR1's balance. My main priority is multiplayer, but the mod is balanced in solo as well. Nearly every change from this mod can be toggled on/off, so you can configure it to your liking!

I highly recommed installing https://thunderstore.io/package/Moffein/EliteReworks/ to go with this.

Also check https://thunderstore.io/package/Risky_Lives/RiskyStarterPack/ out if you want a stable multiplayer-ready modpack to go with this!

Check the Wiki tab for a quick overview of the main changes of the mod!
Full change list can be found at https://docs.google.com/document/d/1Igxdur0M33fdkcDLYgDEbLE0M4-89gSTorxgdn-oyKs/

Feel free to take features of this mod and release them as standalone as long as you link the original GitHub repo in the README.

**Contact me if you're interested in translating the mod!**

## Compatibility

This mod is compatible with nearly all content mods. The only things that will conflict are other mods that modify the Vanilla balance such as FlatItemBuff, but you can make it work by editing your RiskyMod config to disable conflicting features (ex. make sure you dont have both mods trying to modify Leeching Seed).

## Main Features

- Oneshot Protection now actually works.
	- Oneshot = Going from >90% HP to 0% HP in under 0.5s
	- Once triggered, you have to be out of danger (no damage for 7s) before it can be retriggered.
- Shields gate against HP damage like the Guardian's Heart in RoR1.
- Big balance pass over nearly all the items.
	- Bad items like Squid Polyps and Warbanners have gotten substantial buffs.
	- Strong damage items like AtGs and Elemental Bands now have lowered damage stacking.
	- Most forms of range scaling have been removed, and most items aren't able to proc chain anymore.
- Big balance pass over all the Survivors
	- Less useless skill options, default Commando is good now!
	- General power level is meant to be closer to later RoR2 survivors.
- Drone performance now remains the same on all stages.

## Other Changes

- Combat Shrines give less money, but drop items for the team on completion.
- Teleporter radius expands once the boss is dead.
- Tweaked Commencement
	- Only 2 pillars are required to activate the jump pads.
	- Pillars drop items for the team on completion, and you can complete as many as you want.
- Void Fields is shorter and progresses 2 waves at a time.

## Installation
Place RiskyMod.dll **AND** the **language folder** in /Risk of Rain 2/BepInEx/plugins/RiskyMod
	
## For Developers

To make custom allies compatible with RiskyMod's ally changes, use these items located in AllyItems.cs:

- AllyMarkerItem makes the holder benefit from Ally damage resistances. No effect when stacked.
- AllyScalingItem changes level scaling from +30% HP +20% damage -> +20% HP +30% damage so that allies perform the same on all stages. No effect when stacked.
- AllyRegenItem makes the holder's HP regenerate to full in X seconds, X being the amount of stacks.
- AllyAllowVoidDeathItem makes the holder to bypass the "No Void Death" config option.
- AllyAllowOverheatDeathItem makes the holder to bypass the "No Overheat" config option.
- AllyResistAoEItem enables the ResistantToAoE bodyflag on the holder, granting them +300 armor against attacks with DamageType.AoE

These are always initialized even if Ally changes are disabled and their effects have config-checking built-in, so you can simply add them to your allies without having to worry about anything.

Make sure these are only given to Player-team allies, since they'll be painful to fight against (in a bad/unintuitive way) when they're given to enemies.
	
## Credits

Drone Targeting fix - ZetTweaks

Squid Polyp Distraction - DestroyedClone

Language Support - Anreol

Skill Icons - KoobyKarasu, Thingw

Acrid Hitbox Tweaks - TheTimesweeper

Buff Icons - SOM, VALE-X

Simplified Chinese Translation - JunJun_W

Brazilian Portuguese Tra slation - Kauzok

/vm/ (formerly /v/)

## Changelog

*Full changelog included in the .zip*

`1.5.11`

- Fixed JSON issues with Portuguese TL.

`1.5.10`

- Added Brazilian Portuguese TL (Thanks Kauzok!)

`1.5.9`

- Readme update, fixed incorrect number in previous changelog.

`1.5.8`

- Bandit
	- Serrated Shiv
		- Now hits twice for 2x240% damage. (Can apply 2 stacks of Hemmorhage)
		
	*Just a small tweak to make this a bit more appealing to take when compared to Serrated Dagger's lunge and Dynamite's overall damage output, though I believe this skill will still end up by the wayside compared to the other 2.*

`1.5.7`

- Added RiskyStarterPack to readme.

`1.5.6`

- Drones are now immune to splat damage.

	*Not sure how well this actually works.*

- Items
	- Berzerker's Pauldron
		- New stacks refresh older stacks to match how Returns handles buff stacking.
		
	- Predatory Instincts
		- New stacks refresh the duration of all stacks.
		
		*This was a thing in earlier versions of the mod but was mistakenly removed due to the incorrect assumption that it got added to Vanilla.*

- Internal: Updated Ancient Scepter compat to replace skills by SkillDef instead of Index for better mod compatibility.

`1.5.5`

- Fixed Bandit2 DesperadoTracker nullref when using spawn_body via DebugToolkit.

`1.5.4`

- Updated CN Lang.

`1.5.3`

- Queens Gland
	- Fixed nullref related to Swarms where infinite allies would spawn.
		- Pre-emptively did a similar fix for Defense Nucleus.

`1.5.2`
	
- Tweaked Magma Worm fall death prevention code since it was prone to breaking if other mods did the same hook.

`1.5.1`

- Added icons for Standoff (Thanks Thingw!)

`1.5.0`

- Bandit
	- Desperado
		- Now persists between respawns on the same stage.
		
	- Added Standoff from Risk of Rain Returns as a selectable Revolver Passive.
		- Gain +20% damage on kill for 15s. Stacks up to 5 times.
		- Currently looking for an icon artist!
		
		*Damage bonus is lower than in Returns due to 2Bandit having backstab along with cooldowns being shorter compared to 1/Returns.*
	
- Items
	- Hunter's Harpoon
		- Now uses the Risk of Rain Returns version.
			- Gain 125% movement speed for 1s (+1s) on kill. Stacks up to 25s.
			
	- Razor Wire
		- Increased stack damage from 160% (+40%) -> 160% (+80%).