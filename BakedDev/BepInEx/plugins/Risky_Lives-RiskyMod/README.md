## RiskyMod
A full-game overhaul that aims to bring it closer to RoR1's balance. My main priority is multiplayer, but the mod is balanced in solo as well. Nearly every change from this mod can be toggled on/off, so you can configure it to your liking!

I highly recommed installing https://thunderstore.io/package/Moffein/EliteReworks/ to go with this.

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

Skill Icons - KoobyKarasu

Acrid Hitbox Tweaks - TheTimesweeper

Buff Icons - SOM, VALE-X

CN Translation - JunJun_W

/vm/ (formerly /v/)

## Changelog

*Full changelog included in the .zip*

`1.1.0`
		
- Artificer
	- Snapfreeze
		- Now blocks enemy projectiles and hitscan attacks.
			- Does NOT block movement or allied attacks.
		
		*Based on SS2U Cyborg code, hopefully this isn't too buggy.*

- Allies
	- DoT Zone Resistance
		- Removed 0.1 proc coefficient multiplier.
		- Damage is now multiplied by the proc coefficient on top of the existing 0.1 damage multiplier.
			- This is an overall buff to survivability against Mushrums/Exploders.
		- (Mod Compatibility) No longer modifies Vanilla projectiles.
			- DoT Zone Damage Type is now tied to the Mushrum/Lunar Exploder changes in RiskyMod_Enemies.cfg.
				- If the changes to these enemies are disabled, they won't be counted towards DoT Zone Resistance.
		
- Enemies
	- Mushrum
		- (Mod Compatibility) Changes no longer modify the Vanilla projectile.
		
	- Lunar Exploder
		- Reduced fire pool proc coefficient from 0.5 -> 0.2