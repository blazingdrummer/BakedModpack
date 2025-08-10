`1.7.3`

- Fixed Lunar Ruin hook.

`1.7.2`

- Fixed Lunar Ruin exponential damage.
	- Disabled if you have LunarRuinDamageNerf installed.

`1.7.1`

- Moved Halcyonite change to RiskyTweaks.

`1.7.0`

- Halcyonite
	- Fixed Shrine-Spawned Halcyonites having too much stats due to the shrine's gold drain not accounting for time scaling.

`1.6.2`

- Fixed an incompat with Bubbet's Items?

`1.6.1`

- Fixed for MemOp update.
	- Removed Seeker fixes.

`1.6.0`

- Fixed Mending Heal Cores not scaling with level.
- Fixed Seeker's Reprieve not rolling for crits.
- Fixed REX missing an animation for DIRECTIVE: Harvest.
- Fixed Backup Drones not scaling with Ambient Level.

`1.5.3`

- Fixed Palm Blast not scaling with level. (Merged this into the Palm Blast crit fix and renamed option)

`1.5.2`

- Re-added longstanding Solitude nullref since it isn't actually fixed.
- CHEF
	- Dice min duration now scales with attack speed as well.

`1.5.1`

- CHEF
	- Dice hold-for-double-damage now scales with attack speed.

`1.5.0`

- Update for SotS Patch 3.
	- Removed False Son Laser Burst/Step of the Brothers Crit fix.
	- Removed Wandering Vagrant tracking bomb fix.
	- Removed CHEF Sear aiming fix.
	- Removed CHEF bodyflag fix.
	- Removed Longstanding Solitude nullref fix.
	
- Added Seeker Palm Blast crit fix.
	- Aiming this skill is gigafucked online but I'm not gonna rewrite the whole thing.

`1.4.4`

- Removed Tether nullref fix since it doesn't work.

`1.4.3`

- Fixed Antler nullref
- Fixed TetherVFX nullref

`1.4.2`

- False Son
	- Fixed Laser Burst and Step of the Brothers being unable to crit.

`1.4.1`

- Fixed this mod's Breachin Fin damage still being set to +20%, exposed damage bonus so other mods can change it.

`1.4.0`

- Updated for Seekers Part 2
	- Removed DoT Expiry fix since it's fixed for real.
	- Removed Halcyonite fixes.

`1.3.8`
- Re-enabled DoT Expiry Fix from pre-1.3.3 since it wasn't actually fixed in Vanilla.

`1.3.7`

- Breaching Fin Fix
	- Fixed ModifyFinalDamage hook not actually being initialized, causing the item's damage bonus to not be applied.

`1.3.6`

- Made FocusCrystalSelfDamage IL Hook more robust.

`1.3.5`

- Fixed War Bonds buff stacks persisting between stages.
- Fixed multiple Gold Shrines being able to spawn on the same stage.

`1.3.4`

- Fixed Breaching Fin being able to re-apply its damage bonus multiple times in the same proc chain.

`1.3.3`

- Fix for latest update.
- Removed the following fixes since they're fixed in vanilla now:
	- Magma Worm crit hitbox
	- Scorch Wurm nullref
	- Seeker M2 nullref
	- DoT expiry bug
		- Might be wrong on this.
	
`1.3.2`

- Fixed entire game breaking due to 1.3.1

`1.3.1`

- Fixed Longstanding Solitude nullref.

`1.3.0`

- CHEF
	- Fixed missing Mechanical bodyflag.
	
- Halcyonite
	- Fixed spin hitbox persisting when it shouldn't, along with certain skill ignoring stun.
	
	*This has the potential to be a bit desynced, but I don't think it'll have too much of an effect.*

`1.2.1`

- CHEF - Sear
	- Removed Sear Force Align option because it affects Utility trajectory and Sear Vertical Direction option already fixes this.

`1.2.0`

- Fixed Burn/Blight/Poison expiration causing all DoT stacks to be wiped due to SotS.

`1.1.0`

- Removed REX Fruiting nullref fix since it's fixed in Vanilla now.

- Scorch Wurm
	- Fixed nullref on spawn.

- Safer Spaces
	- Seeker: No longer triggers off of rejected Sojourn damage.
	
- Added fixes from external mods. These self-disable if the standalone plugins are loaded.
	- Goorahk
		- Charged Perforator now inherits crit instead of rerolling it. (Server-Side)
		- Fixed Vagrant Orbs being invincible. (Not sure whether it's Client-side or Server-side)
		
	*Originally planned to leave these standalone but I realized I was installing a bunch of extra mods per new profile I set up, so I merged them in for convenience.*

`1.0.11`

- Recompiled with latest dlls.
- Fixed "Eviscerate Targeting Fix" not working.

`1.0.10`

- Recompiled with latest RoR2 dlls.
- Removed FixInvincibleMithrix dependency.

`1.0.9`

- Safer Spaces invuln fix
	- Fixed item failing to proc against Blood Shrines if the user has the hidden invulnerability buff (Merc i-frames, stage spawn).

`1.0.8`

- Fix_Playercount now has MultitudesDifficulty support.
- Removed CurseCatcher and Run History Fix from manifest.
	- Run History Fix is now fixed in the basegame.

`1.0.7`

- CHEF
	- Now always aligned to your aim when using Sear.
	- Sear can now be aimed vertically.

`1.0.6`

- FixPlayercount now remembers the highest playercount on the current stage.

`1.0.5`

- Fixed Bandit's Knife hitbox getting cancelled by other animations.
- Fixed Void Team enemies not being killed at the start of Mithrix's fight.
- Small holdouts now always charge at 100% speed
	- Only changes Moon Escape and Void Fields, Moon Pillars and Void Signals already do this.

`1.0.4`

- Drones and allies no longer attempt to retaliate against their owner.
	- This is intended to fix the bug in normal runs, but it will affect Chaos as well where this behavior is actually intended.
- Vengeance Umbras now have the same level as players.
- Fixed Unseen Hand nullref. (Taken from SeekerVFXFix)

`1.0.3`

- Removed main menu advertisement.
- Added NoVoidsentProcOnNewt.
- Added FixInvincibleMithrix as a dependency.

`1.0.2`

- Fixed Scorpion config option missing Server-Side tag.

`1.0.1`

- Added R2API network tag.

`1.0.0`

- Release