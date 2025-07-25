`1.5.14`

- Commando
	- Frag Grenade
		- Removed falloff.

- Bandit
	- Blast
		- Fixed EntityState not being registered. (Will fix sound/anim not playing online)
		 
	- Specials(existing config unaffected)
		- Host Grace Period: 0.5s -> 0.25s
		- Client Grace Period: 1s -> 0.5s

`1.5.13`

- Gasoline
	- Increased radius from 12m -> 16m to match Will 'o Wisp changes.

- Safer Spaces
	- Fixed item stacking behavior acting as if you had +1. This means starting cooldown will actually start at 20s instead of 18s.
	- Removed 0.1s of i-frames. (Can be re-enabled in config)

`1.5.12`

- Happiest Mask ghosts now spawn at full health in Eclipse, so that their lifetime isn't halved.

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

`1.4.10`

- Added separate config option for Aurelionite changes.
	- This will reset your settings for the Stone Titan since they were previously linked together.
	
- Stone Titan
	- Reduced fist count from 4 -> 3

`1.4.9`

- Added config option to make Captain's Diablo Strike only deal damage to himself instead of all teammates. (Disabled by default)
	- Located in RiskyMod_Survivors.cfg -> Captain

- Artificer M1 Reload now gives priority to the standalone mod to make it easier for custom skill makers.

`1.4.8`

- Added config option to keep Special Ion Surge as a selectable skill when using Ion Surge Utility. (Disabled by default)

`1.4.7`

- Remembered to actually remove Shatterspleen crit chance.

`1.4.6`

- Support for new SS2 drones.

`1.4.5`

- Removed random spread from Void Fiend's primaries.

	*Small QoL that doesn't really matter much since the primary already has heavy autoaim. Only really noticeable at high attack speeds.*

`1.4.4`

- Ally Scaling
	- Disabled Scaling Changes by default in config. (existing config unaffected)
		- This only affects HP/Damage scaling (HP 20% -> 30% Vanilla, Damage 30% -> 20% Vanilla)
	
	*Played for a few months without it off and I found I prefered Vanilla scaling here.*

- Loader
	- Pylon magnetism no longer works against player-controlled entities.
	
	*Mainly intended for King Kombat Arena, but also so that you dont get locked when Loader Vengeance Clones use their pylon.*

`1.4.3`

- Captain
	- Fixed Beacon changes conflicting with Vanilla deployable handling.
		- This fixes your other beacon randomly disappearing sometimes when placing a new one.
	- Fixed Beacon Lysate interaction not actually working.

`1.4.2`

- Bandit
	- Fixed Lights Out Scepter only firing 1 shot when primary is empty.

`1.4.1`

- Updated CN localization for Warbanner.

`1.4.0`

- Warbanner
	- Removed armor bonus.
	- Now heals for 1% of your max HP every second to match RoRR.
		- The healing can stack from multiple banners. Other stats do NOT stack.
	- Now handled by a modded buff and GameObject so that it doesn't interfere with other mods that do stuff with Vanilla's Warbanner.
		- Can be changed to modify Vanilla Warbanner like it did before in the config.

`1.3.3`

- General
	- Fixed a potential bug where the ItemOutOfBounds code could attempt to teleport a single item multiple times.

- Survivors
	- Artificer
		- Flamethrower sprint cancel can now be toggled in-game.
		
	- REX
		- Utilities
			- Enemy knockback force no longer falls off over distance.
			
		- DIRECTIVE: Inject
			- Removed random chance of dropping fruits on-hit. (Can be re-enabled in the config)
			- Allies now heal for 10% of the damage dealt to Fruiting enemies. (before crit and other modifiers)
			- Increased AoE radius from 4m -> 6m so that it's possible to hit multiple enemies if they're close together.
			
			*Fruit-on-hit was neat but impractical to actually use. This should make the skill work better for actually healing people.*
		
- Items
	- Crowbar
		- Fixed description listing incorrect damage. (Was listed as 50% instead of the actual in-game value of 45%)
		
- Allies
	- Allies can no longer be executed.
	
`1.3.2`

- The Back-Up
	- Increased max drones from 4 -> 8 (existing configs unaffected)
	- Now restores a percentage of the cooldown if a drone fails to spawn due to the drone cap.

`1.3.1`

- Fixed Shatterspleen not giving bleed chance.

`1.3.0`

- Items
	- Old War Stealthkit
		- Chance scales off of DamageInfo's damage value so that it doesn't antisynergize with defensive items. (How it worked in pre-anniversary RoR2)
		- Can now proc while already cloaked to match its pre-anniversary behavior.

	- Squid Polyp
		- Chance scales off of DamageInfo's damage value.
		
	- Removed Planula Stealthkit/Squid compatibility code since it's no longer needed.
		
	- AtG Missile
		- Fixed damage being set to 300% (+200%) instead of 300% (+210%)
		
	- Plasma Shrimp
		- Fixed damage being set to 42% (+28%) instead of 40% (+28%)
	
	- Polylute
		- Lowered proc coefficient from 0.1 -> 0
		
		*Was still a direct upgrade to Ukulele even with lowered proc coefficient. Even with this nerf, it still remains very strong.*

`1.2.9`

- Fixed Ion Surge Movement Scaling config option being reversed.

`1.2.8`

- Fixed a bug where certain mod features wouldn't work if damage taken had no Attacker specified.
	- Fixed VengeanceFallImmune not working.
	- Fixed Turret DoTZone resist not working against Lunar Exploders.

`1.2.7`

- Fixed Ocular HUD changes not working.

`1.2.6`

- Fixed Brainstalks running its changes when disabled in the config.
	- If you know of any other bugs like this, report it on the GitHub!

`1.2.5`

- Huntress
	- Flurry attack speed fix now actually works.
- Converted most On.RoR2.Run.Start and On.RoR2.Stage.Start hooks to use the proper delegates provided by the game.
	- This is an internal change that improves mod compatibility.

`1.2.4`

- Remembered to add config for toggling MoreDrones compat.

`1.2.3`

- Ally Changes
	- Added MoreDrones compat.
	- Gunner Drones and Missile Drones now attempt to prioritize the AI's current selected enemy if possible.
		- This is for compatibility with ChensMinionRetarget, since their reworked targeting was ignoring it.

`1.2.2`

- Vengeance clones are now immune to fall damage.


`1.2.1`

- Freeze Execute no longer works on player-controlled entities.

`1.2.0`

- Survivors
	- Commando
		- Frag Grenade
			- Reduced max damage falloff from -75% -> -50%
			- Increased blast radius from 11m -> 12m
			- Now has a separate Scepter state.
				- Throw multiple grenades for 5x700% damage.
			
			*This skill was feeling a bit redundant with Phase Round lightning and Suppressive Fire AoE.*
			
		- Engineer
			- Pressure Mines
				- Fixed skill description still getting changed when changes are disabled in the config.
			- Thermal Harpoons
				- Increased targeting range from 150m -> 2000m
				
		- MUL-T
			- Nailgun
				- Increased damage from 60% -> 70% (same as Vanilla)
				
				*Originally lowered it to try to encourage use of his other weapons, but in retrospect I don't think this was really necessary.*

- Items
	- Power Elixir
		- Reduced barrier gain from 100% -> 50%
		
		*Barrier gain originally got buffed because it was getting punched through super quickly in multiplayer runs. After playing around with it for a while, I've found that it's way too strong in solo while still being pretty bad in multiplayer, so the change has been reverted.*
		
	- Infusion
		- Fixed Infusion gaining orbs from Forgive Me Please.
		
	- Brilliant Behemoth
		- Removed per-stack damage scaling.
		- Extra range no longer decreases below 1.25m.
			- Old: 4, +2.5, +1.5625, +0.9766, +0.6104, etc.
			- New: 4, +2.5, +1.5625, +1.25, +1.25, etc.
		
		*Damage per stack was a holdover from earlier versions where range scaling was removed. Removing the damage scaling, and making the diminishing returns on the range scaling less severe.*
		
	- Newly-Hatched Zoea
		- Added to the Engi Turret blacklist to be consistent with Queen's Gland and Empathy Cores.
		- Stacking above 6 no longer increases ally HP since the main draw of Void allies is their death implosion.

`1.1.4`

- Fixed Thunderstore tags.

`1.1.3`

- Survivors
	- Captain
		- Diablo Strike
			- CDR from Bandoliers/Resupply Beacon increased from 50% -> Max(50%, 20s)
			
			*This is so that CDR items won't make Bandoliers less effective.*

- Items
	- Empathy Cores
		- No longer affected by Normalize Drone Damage/Ally HP+Damage Scaling changes.
			- Still benefits from RiskyModAllyRegenItem/RiskyModAllyMarkerItem.
			
		*These are fine in Vanilla, and deal way too much damage with RiskyMod ally scaling.*

`1.1.2`

- Fixed typo in Void Fiend Risk Of Options config menu.
- Added (Client-Side) to in-game option descriptions to make it clear that it's okay to change them mid-game.

`1.1.1`

- Fixed Risk Of Options compatibility not working due to the compatibility check being run after the config options are applied.

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

`1.0.2`

- Lunar Wisp
	- Reduced projectile shot damage mult from 1.5 -> 1.0
	- Reduced projectile homing angle from 20 -> 15
	- Increased director credit cost from 550 -> 700
	
	*Noticed these getting spammed en-masse when reaching the moon after looping (especially in MP), creating instadeath firing squads the moment you leave the spawn area. Current credit cost is 2x the price of a Lunar Golem (350). For comparison, Greater Wisps cost 5x the price of a Stone Golem. 1.5x damage multiplier was originally there to compensate for 2 hitscan shots being merged into 1 projectile, but after playing around with it a bit I noticed people were dying way too fast to them.*


`1.0.1`

- Fixed Artificer Electrocute Scepter skill being loaded when the skill is disabled.

`1.0.0`

- Pillars Drop Items
	- Fixed pillars failing to drop items if the jump pads activate mid-charging.
	
*Nothing major in this update, but I think this pretty much covers all I've intended to do with this mod. There's a few sore spots left, like Void Lens, but RulebookUnlocker blacklisting works well enough.*

`0.18.4`

- Gunner Turret Teleport
	- Changed placement mode from NearestNode to Approximate
	
	*This should fix all turrets being teleported to the same spot.*
	
- Bandit
	- Burst
		- Increased proc coefficient from 0.6 -> 0.7
		
	- Hemorrhage
		- Disabled on-impact effects.

`0.18.3`

- Fixed Risk of Options compat being initialized at the wrong place internally.
- 「V??oid Fiend』
	- Added config option to disable move speed scaling on 「?Tr?espass】 (Vanilla behavior is default)
		- Can be changed in-game with RiskOfOptions

`0.18.2`

- Bandit
	- Fixed Modify Stats config not working.
	
- Artificer
	- Added missing config option for M1 attack speed scaling.
	
- Items
	- Shatterspleen
		- On-death effect can now proc off of Collapsed enemies.

`0.18.1`

- Updated CN localization.

`0.18.0`

- Void Fields
	- Reduced Cell count from 9 -> 5
		- Each Cell counts as 2 waves, with the 5th wave being the same as wave 9.
	- Fixed holdout radius changes not being applied.
		- Radius was supposed to be increased from 15m -> 30m
	- Reverted holdout charge time from 40s -> 60s (same as Vanilla)

*Hoping to make Void Fields less tedious to do, since Starstorm's Nemesis Invasions are locked behind completing it. General idea is for it to be shorter but more intense. Worried about it being too easy to get a free Red, will adjust if needed.*

- Allies
	- Gunner turrets teleport to your position when beginning holdout zones.
		- Disabled if TeleporterTurrets is installed.

- Spawnpools
	- Sky Meadow
		- Fixed Lunar Golems not spawning.
			
- Items
	- Power Elixir
		- Increased barrier from 50% -> 100%
		
- Bandit
	- Hemmorrhage
		- Proc coefficient increased from 0.3 -> 0.5
		- Now triggers on-impact effects like Behemoth
		
		*Hemmorrhage tickrate doesn't scale with stacks, and I found it still ended up not being worth the effort compared to just shooting things with your gun.*

`0.17.8`

- Added CN translation (Thanks JunJun_W!)
- Volcanic Egg
	- Lowered damage from 800%/1600% -> 600%/1200%
	- Lowered blast radius from 16m -> 14m (same as Artificer Nanobomb)
	
`0.17.7`

- Lunar Wisp
	- Converted primary to a rapidfire projectile attack with light homing.
		- Each shot shoots 1 projectile that deals as much damage as 1.5 bullets (original skill fires 2 bullets per shot).
		- Reduced shots per second from 10 -> 8
			- DPS remains the same.

`0.17.6`

- Captain "Microbots Speed Scales with Drone Count" now works with DroneMeld.
- Bandit revolver animations no longer cancel the knife animation.


`0.17.5`

- Artificer Utility self-knockback is now disabled while the hover jetpack is active.

`0.17.4`

- Allies
	- Now take reduced damage from Mithrix's ground shockwave.
	- Added extra code to make sure Internal Ally Items only give benefits when on the player team.
		- ImmuneToVoidDeath/ImmuneToOverheat are exempt from this, but these are too niche to matter much.
	
- Gunner Turret
	- Now teleports to your location when starting the Mithrix fight.
	- Increased targeting range from 60 -> 120

`0.17.3`

- Ally Regen modifiers are now calculated after all HP changes.
	- Modifier has been moved to the end of RecalculateStats. This allows it to work with DroneMeld's HP scaling.
	
- Gunner Turrets are now repairable.

- Reduced default max Shrine of Combats per stage from 5 -> 3

	*Having too many of these on a single stage causes it to be a hassle for everyone to have to scramble across the entire stage to figure out which shrines they missed.*
	

`0.17.2`

- Added extra nullchecking to Lepton Daisy and TeleExpandOnBossKill.

`0.17.1`

- Changed default Mountain/Combat shrine limit back to 5.
`0.17.0`

- Interactables
	- Shrine of the Mountain
		- Changed default limit from 5 -> -1 (Unlimited)
		- Re-enabled director cost scaling with playercount (+0.5x per player).
		
	- Shrine of Combat
		- Changed default limit from 5 -> -1 (Unlimited)
		- Re-enabled director cost scaling with playercount (+0.5x per player).
		
	*Scaling director credit cost got broken by SotV, but I figured out a fix for it.*

- Character Mechanics
	- Nullify Debuff
		- Now only takes 2 stacks to root.
			- Disabled if EliteReworks is installed since the same change is added there.
			- This allows Void Reavers to root players in a single hit.
				- Leaving this on to see how it performs, since Reavers have always been pretty useless outside of their death explosion and Jailers already have access to a guaranteed root attack that's easier to land than this.

- Allies
	- TC280
		- Deathstate now supports DroneMeld.
	
- Items
	- Squid Polyp
		- Distraction no longer works on Champion (boss) enemies.
		
	- Defense Nucleus
		- Alpha Constructs now distract non-Champion (non-boss) enemies.
		
- Survivors
	- MUL-T
		- Scrap Launcher blast damage falloff reduced from -75% -> -50%

- Enemies
	- Parent
		- Reduced attack damage falloff from -75% -> -50%

	- Mithrix
		- Now tries to prioritize attacking human players if possible.
			- Does not apply to Phase 4.
		
		*With allies being a lot more durable, Mithrix often got stuck fighting them instead of acutal players.*
			
	- Voidling
		- Now tries to prioritize attacking human players if possible.
		- Reduced HP from 2000 -> 1400 (100% -> 40% tankier than Mithrix)
		- Void Fog now uses the same numbers as the Void Fields.
		
		*Just bare minimum changes to make it slightly more tolerable to fight.*

- Spawnpool Changs are now out of beta and are enabled by default. No longer relies on DirectorAPI.
	- Titanic Plains
		- Removed Alpha/Xi Constructs.
		- Removed Jellyfish.
		- Added Bisons when looping.
		
	- Distant Roost
		- Removed Lesser Wisps.
		- Jellyfish now spawn pre-loop.
		- Added Alpha Constructs when looping.
		
	- Siphoned Forest
		- Removed Beetles.
		- Removed Lesser Wisps.
		- Blind Vermin now spawn pre-loop.
		- Added Bisons when looping.
		
	- Abandoned Aqueduct
		- Clay Apothecaries now spawn pre-loop.
		
	- Siren's Call
		- Added Overloading Worms.
		
	- Sundered Grove
		- Removed Lemurians.
		- Removed Clay Dunestrider.
		- Reduced Mushrum spawnrate.
		- Added Alloy Vultures.
		- Added Grovetender.
		
	- Sky Meadow
		- Removed Alpha/Xi Constructs.
		- Removed Wisps.
		- Removed Mushrums.
		- Removed Bronzongs.
		- Added Jellyfish.
		- Added Imps.
		- Added Lunar Golems.
			- HP/Director Cost is scaled to be the same as Elder Lemurians.

`0.16.8`

- Fixed missing Acrid Scepter icon.

`0.16.7`

- Captain
	- Fixed M1 changes not being applied due to 0.16.0

`0.16.6`

- Barrier
	- Reduced decay rate from 1%-6% -> 1%-5%

- Allies
	- Increased DoT Zone Resistance from -80% -> 90%
	
		*Noticed turrets and similar allies still dying way too quickly to Mushrums and Exploders.*
	
	- Gunner Turret
		- Reduced full-regen time from 40s -> 30s
		- Increased HP from 240 -> 300
		
	- Emergency Drone
		- Increased HP from 340 -> 360
		
	- Incinerator Drone
		- Increased HP from 340 -> 480
		- Increased turn speed from 90 -> 180
		- Increased full-regen time from 20s -> 30s
		- Reduced base damage from 12 -> 10 (same as Vanilla)

- Items	
	- Aegis
		- Re-enabled Vanilla extra barrier conversion per stack.
	
- Artificer
	- Primaries
		- Reduced damage from 390% -> 360%
		
		*New damage number is the same as MUL-T's buffed scrap launcher, not factoring in Ignite.*
		
	- Fixed Utility Ion Surge cancelling Flamethrower.
	- Flamethrower ignite chance increased from 50% -> 100%
	
		*Puts this between pre-SotV numbers and current Vanilla numbers. Probably gets crazy with Ignition Tank, but it's such a niche item in most scenarios that this type of interaction is fine.*

`0.16.5`

- Bandit
	- Fixed Specials consuming all charges at once due to 0.16.0

`0.16.4`

- Pillars Drop Items and Combat Shrines are now compatible with ArtifactOfPotential from zombieseatflesh7.
- Delicate Watch
	- Added an option to disable the HUD buff icon.
- Infusion
	- Added an option to disable the HUD buff icon.
- H3AD-ST
	- Added an option to disable the HUD buff icon.
		- Disabling this prevents the cooldown mechanic modifications from working.

`0.16.3`

- Bandit
	- Fixed Enter Reload animation having the potential to cancel/delay the knife hitbox.

`0.16.2`

- Bandit
	- Fixed Primary animations having the potential to cancel/delay the knife hitbox.
	- Fixed Smokebomb consuming all charges due to 0.16.0

`0.16.1`

- Added config for AI Targetfinding in RiskyMod_Enemies.cfg

`0.16.0`

- Enemies
	- AI Targetfinding
		- Enabled FullVision flag and disabled LoS checks.
		
		*RoR2's AI targetfinding doesn't work well with its horde shooter gameplay. Enemies often go AFK in random parts of the map and take up spawnslots, and oftentimes they will forget what they're doing and go AFK mid-combat due to losing their target.*

- Items
	- Stickybomb
		- Disabled physics.

		*Bandaid fix for stickies falling off of flying enemies in MP.*

	- Shuriken
		- No longer procs Elemental Bands. 
		
		*For most characters, this item is an instant scrap due to how it steals Band procs.*

	- Razor Wire
		- Proc Coefficient no longer scales off of HP lost.
		- Proc Coefficient is now 0.5 for normal damage, 0.1 for DoT damage.

		*Simplifying this item's behavior since the proc coefficient thing is really only necessary for Helfire.*

	- Squid Polyp
		- Increased HP from 100% (+30%) -> 100% (+50%)

	- Unstable Tesla Coil
		- Increased radius from 20m -> 25m

		*New radius matches the radius used for most other lightning/AoE type effects.*

	- Shaped Glass
		- Logbook now lists the new stacking behavior.
		
	- Transcendence
		- No longer disables TrueOSP if ShieldGating AND Transcendence Always Shieldgate are disabled.

- Survivors

	- Made internal survivor modifaction code more robust.
		- SkillDefs are now modified by directly loading the Addressable, instead of searching the Character's SkillFamilies.
		- A lot of things got changed internally. Let me know if any skills are behaving weirdly!
	
	- Huntress
		- Flurry
			- Added extra code to be double sure that arrows aren't getting lost at high attack speeds.
		
	- Bandit
		- Stats
			- Reduced HP from 110 -> 100.
			
			*Bandit got a lot of buffs in this mod, with the extra dash from his knife, the invisibility position tracking buff, and more. Lower HP is more in line with his role of being a hit and run Assassin. This is the same HP value used for BanditReloaded.
			
		- Burst
			- Reduced proc coefficient from 0.75 -> 0.6
			
			*Closer to Vanilla, but still higher.*

		- Serrated Dagger
			- Fixed the attack getting delayed/cancelled by Smokebomb's animation.

		- Smokebomb
			- Increased cooldown from 6s -> 7s

			*This increases the effective cooldown from 3s -> 4s, which is the same as Commando's Roll.*
			
		- Special Grace Period
			- Now uses separate values for Host and Clients.
				- Host/Singleplayer: 0.5s
				- Multiplayer Client: 1.0s
				
			*0.5s was the original intended value for BanditReloaded, but it had to be increased due to problems with consistency for online clients.*

	- MUL-T
		- Fixed M2 changes applying to other mods that clone the projectile.

	- Engineer
		- Mobile Turrets
			- Now immune to fall damage.

			*These sometimes like to walk off cliffs because the AI isn't very smart.*
			
	- Artificer
		- Disabled Blaze Storm and Electrocute by default.
			- Only applies to new installs. Existing configs are unchanged.
			
			*These skills are made of reused assets and aren't polished at all. Since they won't be getting any work done on them, they'll be hidden by default.*

`0.15.0`

- Commando
	- Frag Grenades
		- Reverted to Vanilla, except that they explode on direct impact with enemies.
			- If the nade hits the world first, it will behave as it does in Vanilla.
		- Cookable nades can be re-added as a separate standalone skill with https://thunderstore.io/package/Gatorism/Commando_Grenade_Cooking/
			- Comes with a config as well!
		
		*Wanted to give the option to use vanilla-ish nades, since I feel cooking is a bit awkward with Commando's skill flow. I feel explode on impact trivializes Vanilla nades a bit, but that's preferable to being unable to use them against flying enemies.*

`0.14.13`

- Fixed Beetle Guard spam with QueensGlandBuff.
	- RiskyMod now disables all of its Queens Gland code except for the ally scaling changes when QueensGlandBuff is loaded.
	
	*Old compat code no longer works, so I'll just let QueensGlandBuff handle things.*

`0.14.12`

- Commando
	- Suppressive Barrage (Scepter)
		- Fixed missing name token.
		- Increased shot count from 10 -> 18
		
	- Changed HE Grenade (Scepter) into Carpet Bomb (Scepter)
		- Fixed the Scepter version not actually working.
			- It was supposed to give 2x damage and no falloff.
		- Now gives +5 additional projectiles (600% damage each) on top of the original 1200% damage grenade, as well as no falloff.
		
	*Commando's RiskyMod Scepters were a bit underwhelming because they were originally balanced around his RoR1 Scepter, rather than the balls to the wall insanity that 2's Scepter provides. These changes should bring them more in line with how they are supposed to be.*
	
`0.14.11`

- Enemies
	- Beetle
		- Fixed hitbox changes causing attacks to go through Enforcer's shield.
		
	- Blind Pest
		- Reduced AI primary skill max distance from 70m -> 50m
		
		*Same distance as Vultures. For comparison, Lemurians are 35m and Wisps are 20m*

`0.14.10`

- Enemies
	- Stone Titan
		- Disabled laser tracking rework.
		- Disabled laser min distance removal.
		- Reduced laser tickrate from 10 -> 8 (Vanilla)
		- Reduced laser DPS increase from +50% -> +25%
		
		*Laser Rework didn't work well at all, accuracy was too poor. Would require a rewrite of the skill state to make it workable, which I don't plan on doing.*

`0.14.9`

- Items
	- Power Elixir
		- No longer heals.
		- Now instantly gives 50% barrier on proc.
			- Scales off of Health + Shields.
		- Proc condition changed from 50% HP to 50% Combined HP (HP + Barrier + Shield)
			
		*50% healing on a single Common item was too strong, and there was no way to balance it without making it feel terrible. Barrier should allow this item to function as quick temporary protection, while still requiring you to actually find a way to heal yourself up.*
		
	- Leeching Seed
		- Reduced healing from 3% (+1.5%) -> 2% (+1%)
		
		*Trying to even out the performance of this item compared to Scythes.*
		
	- Defense Nucleus
		- Fixed allies spawning sideways.
		
- Enemies
	- Beetle
		- Extended hitbox forward range.

`0.14.8`

- Defensive Microbots Deletion Restrictions
	- Fixed code ignoring projectile cannotBeDeleted tag.
	
`0.14.7`

- Defensive Microbots Deletion Restrictions
	- Now checks if projectile speed > 0 before deleting, so that things like the moon escape explosions don't get deleted.

`0.14.6`

- Allies
	- Added Tinkers Satchel support.
	
`0.14.5`

- Allies
	- Damage Zone Resistance (previously Mushrum Resistance)
		- Now includes Lunar Exploder fire pools.
	- AllyRegenItem now scales with internal BoostHP items.
		- This will fix certain allies having really slow health regen.
		
- Items
	- Transcendence
		- Increased shield regen penalty from 0 (+0.5s) -> 0 (+1s)
		- Transcendence shieldgating is now a separate config option from the global shieldgating setting.
			- Located in RiskyMod_Items.cfg next to the Transcendence config option.
			- If enabled, Transcendence will shield gate even if Shield Gating is disabled.
			- If disabled, it will simply follow whatever setting Shield Gating is set to.
			
		*Putting this at a halfway point between the earlier 1s (+1s) value and the 0 (+0.5s) value.*
			
- Enemies
	- Stone Titan
		- Increased laser radius from 0 -> 0.2
		
		*Nerfs from previous updates made these a bit too ineffective at using their laser.*

`0.14.4`

- Railgunner
	- Fixed Bungus knockback fix not working online (and causing console spam).


`0.14.3`

- Commando
	- Reduced Phase Round damage from 480%/240% -> 450%/150%
	
- Allies
	- Added support for SS2's Security Drones, Spikestrip's Blue Lemurian, Chill Drone, QB Drone, and Gradius Mod.
		- Compat can be enabled/disabled in the config.

`0.14.2`

- Added Disable Projectile On-Kill Effects config option for Vagrants, Grovetenders, and Lunar Wisps in RiskyMod_Enemies.cfg
	- Prevents players from proccing on kill effects when shooting down projectiles from the above enemies.
		- This was already in the mod beforehand, but was tied to the other changes for each monster and couldn't be independently enabled/disabled.

`0.14.1`

- Fixed Vengeance Nkuhanas Opinion damage reduction not working.
- Fixed Void Locus Void Potentials being able to have duplicate item choices.
- Fixed Zoea Ignore Ally Cap config option causing Zoea allies to not benefit from ally changes when disabled.
- Internal ally bonus items are now disabled when KingKombatArena is active.
- Squid Polyps have -75% HP when spawned by enemies or when spawned in KingKombatArena

`0.14.0`

- Fixed missing DirectorAPI dependency causing the mod to not work on certain modpacks.
	- Bug probably showed up around 0.13.24 or 0.13.25
	
- Items that fall out of bounds are now teleported back into the stage.
	- Slightly jank, condition for triggering is item lifetime > 10s and item velocity > 5m/s.
	- Config option is located in the Misc section of RiskyMod_General.cfg
	
- Homing projectiles now select targets based on angle, instead of angle + distance.
	- This will make all homing projectiles more reliable at actually hitting their target, instead of suddenly curving off to the side and missing.
		- Notably affects Visions of Heresy.
	- Config option is located in the Misc section of RiskyMod_General.cfg
	
- Void Locus
	- Signals Drop Items
		- Removed Pearl/Lunar drop chance config option.
		- Reduced Common chance from 50% -> 45%
		- Reduced Legendary chance from 10% -> 5%
		- Now has a 10% chance to drop Void items.
		- Now drops Void Potentials.
		
		*You will need to manually change the chance config if you are updating.*

- Artificer
	- Fixed Utility self-knockback applying while grounded.
	
- Items
	- Aegis
		- Stacks no longer increase overheal->barrier percent beyond the initial 50%.
		- Now divides barrier decay rate by 2 (+1 per stack)
			
		*Should give this item a much more tangible benefit. Leaving the base overheal->barrier percent alone for now to gauge how effective this item is in its current state.*
		
	- Brittle Crown
		- Changed damage coefficient scaling range from 100%-1000% -> 200%-1200%
		
	- Needletick
		- Disabled changes.
		
		*The -1 armor did nothing to actually help the item in MP/loops, and just bloated the item's functionality. Will only re-enable changes if I actually have something that works.*
		
	- Newly-Hatched Zoea
		- Disabled in bazaar.
		- Reduced max ally count from 8 -> 6
		- Max ally count can now be specified in config.
		
- Enemies
	- Stone Titan
		- Disabled laser duration extension change.
		
		*Was annoying to fight at midrange, and made them worse at close range due to being committed to lasering for longer.*

`0.13.26`

- Power Elixir
	- Fixed heal being set to 25% over 4s instead of 50% over 8s.

`0.13.25`

- Artificer
	- Added config option to disable Snapfreeze Rework/Blaze Storm self-knockback.
		- Client-side and can be changed in-game.
		
	- Fixed Electrocute's config option name being horribly misspelled. This will reset the config option for this skill.


`0.13.24`

- Safer Spaces
	- Fixed config option not working.
	- Updated description to match changes.

`0.13.23`

- Tele Expansion
	- Changes are now disabled during Eclipse 2+ by default.
	
	*Can be changed in config.*
	
- MUL-T
	- Power Saw
		- Reduced barrier gain per second from 6% per enemy hit to 3% (+3% per enemy hit)
			- 6%/s for 1 enemy, 9%/s for 2, etc.
		- Separated hitbox changes from physics changes in the config.
		
- Items
	- Delicate Watch
		- Fixed buff icon persisting after losing the item.
		
	- Gasoline
		- Fixed description mistakenly listing the range as 16m instead of 12m.
		- Stacks now increase burn damage multiplier by 25%.
			- Total damage remains the same.
			
		*This used to be in an older version of the mod but got broken by SotV.*
		
	- Rose Buckler
		- Reduced sprinting armor bonus from +20 -> +10
			- Passive armor remains the same.
			
		*Reverting this to how it was in earlier versions of the mod.*
		
	- Hunter's Harpoon
		- Reduced duration from 3s (+1.5s) -> 2s (+1s)
		
	- Weeping Fungus
		- Reduced healing from 1.5%/0.75% -> 1.2%/0.6%
		
		*Bringing this closer to Starstorm 2's original values for Dungus (1.0%/0.5%)*
		
	- Safer Spaces
		- Increased cooldown from 15s -> 20s
		
		*Having done a lot of runs with this, I've found that Safer Spaces is generally a no-brainer on most characters, since you don't get hit very often.*
		
- Equipment
	- Goobo Jr.
		- Disabled ally stat scaling changes, since their damage was already fine before.

`0.13.22`

- Stone Titan
	- Reduced shot radius from 0.2 -> 0 (same as Vanilla)
	- Re-enabled falloff (same as Vanilla)
	
	*Laser radius buff was originally there to counteract the poor aim of the old laser rework. Now that the tracking works properly, it's not needed anymore. Falloff has been re-enabled to match the Xi Construct."

`0.13.21`

- Stone Titan
	- Improved laser rework accuracy while moving.

`0.13.20`

- Allies
	- Added an option to disable scaling changes.
	- Added an option to disable regen changes.
	
- Drones
	- Missile Drone
		- Reduced damage per burst from 4x15.6 -> 4x13.2 (Roughly the same as vanilla)
		
		*Pretty much the same as Vanilla now (but with better accuracy/targeting). This doesn't change breakpoints for killing Wisps/Lemurians.*
		
	- TC280
		- Fixed deathstate bugs.
		- Panic Shield
			- Improved VFX.
			- Increased cooldown from 90s -> 120s
		
- Items
	- Power Elixir
		- Slowed full-heal duration from 4s -> 8s.
		
		*Being saved from the dangerous <50%HP threshold every stage is an incredibly strong effect for a Common item, so healrate is getting lowered to make it less effective at facetanking out of situations where you should be dying.*
		
	- Spare Drone Parts
		- Moved config options to RiskyMod_Items.cfg
		- Reduced damage from 60% -> 50%
		- Chaingun ricochets now deal 50% less damage per bounce.
		
		*Toning down the ability of drone swarms to full-clear the map by reducing their crowd damage. Item is still incredibly strong despite these changes.*
		
- Enemies
	- Stone Titan
		- Increased laser cooldown from 15s -> 20s (Vanilla)
		- Reduced laser damage coefficient from 160% -> 150%
		- Turn speed is now only restricted while firing its laser.
		- Laser tracking speed reduced from 60 -> 30
		- Significantly improved laser accuracy.
			- Uses lockon, but has a restricted turn speed like the Xi Construct.
			
		*This is closer to my original intention, which was for the laser to be like Vanilla but without the perfect lockon. Cooldown was increased back to Vanilla levels because Titans were spending too much time lasering things and not enough time using their other skills.*

`0.13.19`

- Acrid
	- Fixed Separate Config being accidentally enabled by default.
		- This will reset the config option.
	- Attempted to fix bugs that may be related to Separate Config.
	
	*I've heard that Acrid changes got broken for some people after a recent update. I can't reproduce the bug on my end, so be sure to contact me with your LogOutput.log file if the issues persist after this update.*

`0.13.18`

- Bandit
	- Blast
		- Increased damage from 330% -> 360%
		- Reduced spread from 0.6 -> 0.4

		*This skill was still feeling like a direct downgrade to the shotgun. Reduced spread will allow it to be more effective at its intended range, and increased damage makes it come out on top in terms of proc DPS when compared to the shotgun (5x90% x 0.75)*

`0.13.17`

- Removed Bison debug text.

- Captain
	- Diablo Strike
		- Proc coefficient increased from 1.0 -> 3.0
		- Renamed "Diablo Strike Changes" config option to "Diablo Strike Ammopack Nerf" for clarity, and so that it can be toggled on/off separately from the proc coefficient changes.

`0.13.16`

- Hotfix.

`0.13.15`

- Added Tele Charge Time Increase option (disabled by default).
	- Located in the Game Mechanics section of RiskyMod_General.cfg
	- Increases tele charge time from 90s -> 120s to match RoR1 Monsoon.
	
	*Intended to counteract the faster clear times from Tele Expand on Boss Kill. Left disabled by default since I think it's not that fun, and a better option is to play modded difficulties with higher scaling values.*

- Items
	- Tweaked description style tags on Fresh Meat, Warbanner, Beetle Gland, and Squid Polyps.
	- AtG Missile, Plasma Shrimp, Molten Perforator, Charged Perforator
		- Increased damage of stacks from 60% -> 70%
		
		*Stacking damage increase was leaning a bit too close to Common item territory on AtGs. Similar items have been tweaked as well for consistency.*
		
	- Brilliant Behemoth
		- Reduced damage from 60% (+36%) -> 60% (+20%)
		- Re-added range scaling.
			- Has diminishing returns. Same range as Vanilla with 2 Behemoths, lower range beyond that.
				- Range is the summation of 4 x 0.625 ^ (itemCount - 1), so 4m, 6.5m, 8.0625m, etc.
			
		*Stacks felt lacking without range scaling, and the item is hard to stack in the first place.*
		
	- Defensive Microbots
		- Defensive Microbots Drone Scaling is now separate from Defensive Microbots Nerf in the config.
		- Fixed Defensive Microbots Nerf causing Beetle Guard projectiles to not getting deleted.
			
	- Artificer
		- Electrocute
			- Fixed the skill getting instantly cancelled by RtAutoSprint.
	
	- Acrid
		- Fixed Bite not getting the Slayer damagetype if Deeprot is equipped.
		- Frenzied Leap
			- Increased damage from 320% -> 550% (same as Vanilla)
			
			*Losing out on 1 extra jump is a huge penalty, even with the existing buffs from the mod.*

`0.13.14`

- Allies
	- Fixed Missile Drones not benefiting from ally changes.
	- TC280
		- Increased HP regen time from 30s -> 40s to match other drones
		- Increased Shield Overload cooldown from 60s -> 90s
		
		*Shield Overload stacked on top of faster HP regen and the drone's naturally high tankiness ended up being too much, especially since drones are now cheaper to repair if they go down.*
		
- Artificer
	- Ion Surge movement scaling
		- Height is now based on default sprinting speed.
		- Added Risk of Options support, since it's a client-side feature that can safely be toggled on/off midgame.

`0.13.13`

- Void Locus
	- Increased signal charge time from 30s -> 40s to match the modified Void Fields Cell charge time.

`0.13.12`

- Void Locus
	- Tweaked Fog Damage
		- Reduced HP% per second from 5% -> 2.5%
		- Removed damage rampup over time.
		
		*Void Fields got changed in an update post-SotV to make the fog damage more reasonable, but Void Locus never received that change. New numbers are the same as current Void Fields.*
	
	- Remove Fog
		- Changed default config setting from Enabled to Disabled. (Only affects newly-generated configs. Existing configs won't change.)
		
		*This was originally enabled by default due to the Void Fog being unplayable in large lobbies, along with the Fog killing too fast to catch up to teammates who decided to activate Signals early.*
		
- Items
	- Crowbar
		- Increased damage from +45% -> +50%
		
	- Queen's Gland, Empathy Cores, Defense Nucleus, Newly-Hatched Zoea, Halcyon Seed, Backup, Goobo Jr.
		- Separated Ally Changes from Item Changes. Item config no longer prevents Ally Changes from being applied.
		
		*This is how it used to work pre-0.13. Item config affects the actual stats/stacking, while the general game-wide ally scaling changes are tied to the Ally Changes config.*

`0.13.11`

- Spawnpools (Beta)
	- Siphoned Forest
		- Moved Bighorn Bisons back to being post-loop enemies.
		
		*Having Vermin, Pests, and Bisons on Stage 1 ended up making this stage feel skewed.*

`0.13.10`

- Enemies
	- Bighorn Bison
		- Disabled snow VFX overlay when spawning on non-snowy stages.
		- Increased Charge speed coefficient from 8 -> 12
		- Increased Charge turn speed from 300 -> 600
		- Reduced Charge self-stun duration from 3s -> 1s to match other stunning effects.
		
		*Partially inspired by Inferno's changes, should be compatible with it. Vanilla Bisons are too slow and unmaneuverable to be much of a threat. Faster charge speed should make them a bit harder to dodge. Turn speed has been increased as well, but I'm not sure if it's actually doing anything.*
	
- Spawnpools (Beta)
	- Titanic Plains
		- Bighorn Bisons can spawn post-loop and during Simulacrum.
	- Siphoned Forest
		- Bighorn Bisons can now spawn on the first loop.

`0.13.9`

- Artificer
	- Fixed Ice Wall not freezing when cast on midair enemies.
	
	*This bug was introduced a few versions ago when it got changed from Blast Jumping to a simple backwards push.*

`0.13.8`

- Defense Nucleus
	- Fixed another coding oversight related to the HealthDecay item when the "Inherit Elite Affix" config option is disabled.

`0.13.7`

- Defense Nucleus
	- Fixed some coding oversights.

`0.13.6`

- Queens Gland
	- [Compatibility] Fixed QueensGlandBuff's stats getting overwritten by RiskyMod's.

- Squid Polyp
	- Increased lifetime from 30s -> 40s
	
	*Intended to mirror how allies take 40s to regen to full.*
	
- Defense Nucleus
	- Now decays over 40s.
	- Added AoE resistance.
	
	*These would spawn on one side of the map, then sit there doing nothing while the fight has moved to another part of the map.

`0.13.5`

- Power Elixir (Rework)
	- Triggers when HP is 50% or lower after taking damage.
		- Counts actual HP only.
	- When triggered, rapidly regenerates 50% of your HP over 4 seconds.
		- Cannot retrigger while regen is active.
		- Unaffected by difficulty.
	- Breaks when triggered. Resets on the next stage.
	
	*Removing perma-break effect while trying to keep the spirit of the Vanilla item. 50% threshold will make this more consistent to trigger, but with a weaker healing effect to compensate for being more readily-accessible.*

`0.13.4`

- Fixed purchaseable drones not receiving ally-related items.
	- Fixes drones taking damage from Void Fog.
	- Fixes drones dying to Void Reaver explosions.
- Fixed Void Reaver changes not working.

`0.13.3`

- Fixed styling on Razorwire description.
- Increased Shatterspleen bleed chance from 5% -> 10%
	
	*No other +5% bleed chance items exist in the game, which made this feel out of place.*

`0.13.2`

- Little Disciple
	- Increased proc coefficient from 0 -> 0.5
	
	*Been on the fence about doing this for some time. After playing a lot with 0 proc Disciple, I've come to the conclusion that it needs some proc coefficient to be worthwhile.*

`0.13.1`

- Queens Gland, Defense Nucleus, Empathy Cores
	- Can now die to Void Implosions.
	
	*Enabling Void Implosion deaths on expendable allies that can easily respawn, as a stylistic touch. Things that don't respawn easily (Aureleonite, Col. Droneman, Drones in general) will remain immune to Void Implosions.*

`0.13.0`

- Compatibility and Configs
	- Added console messages to notify when a RiskyMod feature is disabled due to another plugin being loaded.
	- Fixed Sacrifice change conflicting with the standalone SacrificeTweaks plugin.
	- Repairable TC280 config option is no longer disabled when ZetTweaks is installed. It will instead give a console warning to let you know that you need to disable it in either plugin.
	- Added config options for Spawnpools beta.
		- Spawnpools will remain in beta until DirectorAPI gets updated to be more stable.

- AI Blacklist
	- Blacklisted Safer Spaces due to the possibility of unkillable enemies at high stacks.
	
- Survivors
	- MUL-T
		- Power Saw config now allows you to individually enable Physics Changes and Barrier-On-Hit.
	- REX
		- Removed leftover Swap Utility Effects code that was supposed to be removed in a previous update.
			- Alt Utility no longer applies Weaken.
			- Config option has been changed to "DIRECTIVE: Disperse Healing"

- Allies
	- Refactored code to be a LOT cleaner.
		- Added internal items to allow other modders to make their allies compatible with RiskyMod.
	
		*See the For Developers section of the README for more info!*
		
	- Increased Mushrum resistance from -67% damage -> -75% damage.
	- Drones
		- Repairing drones that were destroyed in combat is now 50% cheaper.
		
		- Missile Drone
			- Increased HP from 225 -> 250
		
		- Incinerator Drone
			- Increased HP from 300 -> 340
			- Increased range from 18m -> 25m (same as Artificer Flamethrower changes)
			
		- Emergency Drone
			- Increased HP from 300 -> 340
			- Reduced price from $100 -> $80
		
		- TC280
			- Mega Turret
				- Bullets are now explosive.
					- Damage remains the same.
				- Shot count increases with attack speed.
			- Rockets
				- Remove blast falloff.
			- New Passive: Shield Overload
				- When health goes below 25% HP, shock nearby enemies and temporarily gain a massive amount of shield.
				- 60s cooldown.
			- Gibs despawn after 15 seconds.
			
			*Is this too much?*
			
		- Col. Droneman
			- Increased HP from 180 -> 200
			- Added shields.
	
- Items
	- Happiest Mask
		- Reduced damage bonus from 900% (+240%) -> 600% (+180%)
			- Description incorrectly listed this as 800%
		- Now benefits from Ally changes.
		
		*Damage reduction is due to the +50% level damage scaling increase from Ally Scaling.*
		
	- Queen's Gland
		- Enemy Queen's Gland Guards no longer benefit from Ally changes.
		- Fixed initial stack damage being set to 400% instead of 300%
		- Description now correctly lists the first stack HP as 200% instead of 100%.
		
	- Empathy Cores
		- Enemy Empathy Cores no longer benefit from Ally changes.
		
	- Halcyon Seed
		- Now benefits from Ally changes.
		
	- Defense Nucleus
		- Now benefits from Ally changes.
		
	- Newly-Hatched Zoea
		- Removed hidden +50% damage bonus.
		- Now benefits from Ally changes.
			- Can still die to Void Implosions.
			
- Equipment
	- Goobo Jr.
		- Fixed damage being set to 400% instead of 300%
		- Fixed HP being set to 700% instead of 600%
		- Now benefits from Ally changes.
	
- Enemies
	- Aureleonite
		- Damage increased from 40 -> 60
		
- Spawnpools Beta
	- Siphoned Forest
		- Removed Beetles
		- Blind Vermin can now spawn on the first loop