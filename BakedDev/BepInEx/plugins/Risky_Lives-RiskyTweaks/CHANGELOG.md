`1.7.0`

- Halcyonite
	- Shrine-spawned Halcyonite stat boost level is now capped at 20 (12x HP, 4x damage)

`1.6.8`

- Fixed Railgunner Polar Field buff reducing the damage of friendly projectiles.

`1.6.7`

- Fixed for MemOp update.
	- Removed Seeker/CHEF proc coefficient tweaks.

`1.6.6`

- Removed False Son's hidden Slam cooldown.

`1.6.5`

- Dynamic Barrier Decay is now disabled while in Seeker's Reprieve, since the skill is balanced around vanilla barrier decay.

`1.6.4`

- CHEF
	- Glaze is no longer cancelled by Sear.

`1.6.3`

- Moved Snappier Cleaver attack speed scaling to RiskyFixes.

`1.6.2`

- CHEF
	- Dice min duration delay changed from 0s -> 0.2s (Vanilla is 1s), and now scales with attack speed.

`1.6.1`
	
- CHEF
	- Dice proc coefficient increased to 1.0
	- Dice minimum return delay has been removed.

`1.6.0`

- SotS part 3
	- False Son
		- Slam Proc Coefficient now sets falling slam proc coefficient to 1 as well.
		
- Seeker
	- Meditate now stuns and cleanses projectiles. (Formerly RiskySeeker)

`1.5.4`

- Seeker
	- Spirit Punch 3rd hit proc coefficient increased from 0.75 -> 1

`1.5.2`

- Halcyonite
	- Removed ImmuneToVoid flag.
	- Now stunnable during Whirlwind.

`1.5.1`

- False Son (Playable)
	- Heavy Slam proc coefficient reduced from 3 -> 1
	- Laser proc coefficient increased from 0.45 -> 1

`1.5.0`

- Updated for Seekers Part 2
	- Void Fields
		- Reverted Void Fog damage ramping. (it increases it teamwide btw lmao)
		- Removed enemies gaining items while outside the bubble. (This doesn't even fix Sonorous/Sacrifice farming on the other hidden realms so why is this a thing AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA)

`1.4.2`

- Ally Regen
	- Added Inferno Drone (Sandswept) compat.

`1.4.1`

- Recompiled for latest update.

`1.4.0`

- Seeker
	- (Client-Side) Default M2 no longer modifies FOV.
	
- Allies
	- (Server-Side) Most allies regen to full HP in 40s. Affected by Difficulty regen multipliers. Disabled if RiskyMod is installed.
		- List:
			- Gunner Drone
			- Healing Drone
			- Missile Drone
			- Incinerator Drone (30s)
			- Healing Drone
			- Equipment Drone
			- Emergency Drone
			- TC-280 (30s)
			- Gunner Turret (30s)
			- Col. Droneman
			- Empathy Cores
			- Beetle Guard
			
			- Shock Drone (SS2)
			- Duplicator Drone (SS2)
			
		- This list is manually-built, but external mod devs can add to it.
		
	- Gunner Turret
		- (Server-Side) No longer needs to reload.
		
	- TC-280
		- (Server-Side) Reduced price from $350 -> $300

`1.3.12`

- Pillars/Signals Drop Items
	- Fixed issue where White/Green/Red items could still drop when their chance is set to 0 in the config.

`1.3.11`

- Warbanner
	- Fixed incompatibility with RiskyMod resulting in duplicated Warbanner buff.
- Added RU TL (Thanks inkyarev!)

`1.3.10`

- Acrid
	- Fixed Regenerative is Healing not scaling with buff stacks.

`1.3.9`

- Actually remembered to disable Visions code when Heretic is loaded.

`1.3.8`

- Fixed conflict with Heretic due to Visions fix.

`1.3.7`

- Raise Level Cap - Fixed levelup bell sound ignoring the "max level to play levelup effects" cap.

`1.3.6`

- Fixed Loader Sprint QOL not working.

`1.3.5`

- Fixed Visions attack speed scaling.

`1.3.4`

- Primordial Tele Loop
	- Fixed tele spawning in the wrong orientation.
	- Added some compatibility code to prevent potential conflicts with RiskyArtifacts' Artifact of Primacy.

`1.3.3`

- Void Fiend
	- Uncorrupted Trespass move speed scaling disabled. (Can be changed in-game via Risk of Options)

`1.3.2`

- Mobile Turret Buff
	- Added fall damage immunity.
	
`1.3.1`

- Added Specials to Loader Sprint QoL.
- Changed Blast spread reduction from -100% to -50%

`1.3.0`

- Disabled Roll of Pennies in the Bazaar.
- Fixed internal inconsistency with "Enabled" variable name.

- Survivors
	- MUL-T
		- Scrap Launcher
			- Removed falloff.
			
			*This has roughly the same AoE as Artificer's Plasma Bolts, but with pitiful splash damage due to the SweetSpot modifier.*
			
	- Acrid
		- Regenerative now counts as healing, and it is unaffected by difficulty regen modifiers.
			- Still affected by Eclipse modifier.
			
	- Bandit
		- Changed Blast from No Spread to Reduced Spread. (-50% spread)
			
- Enemies
	- False Son
		- Removed i-frames from Corrupted Paths.
		
	- Child
		- Removed i-frames from teleport.
		
	- Scorchling
		- Removed i-frames from burrow.

- Commencement
	- Faster Holdouts
		- Pillar of Mass charge duration reduced from 60s -> 40s
		- Pillar of Soul charge duration reduced from 30s -> 20s

- Void Locus
	- Void Signal charge duration reduced from 60s -> 40s

`1.2.0`

- Teleporter is now replaced with Primordial Teleporter after looping.
	
- Artificer
	- Snapfreeze now fires as soon as you release the button.
	- Ion Surge height no longer scales with movement speed. (Can be changed in-game)
	- Flamethrower burn is now guaranteed, reverting the SotV nerf.
	
- Void Fiend
	- Corrupt transition duration reduced to 0.5s
	- Primaries now have no random spread.
	- Corrupted Crush fires faster and has no use limit.

`1.1.1`

- Recompiled for latest RoR2 update.

`1.1.0`

- Bandit
	- Blast pierces.
	- Blast has less spread.

- Engi
	- Mobile Turrets now always sprint, have more range, and no longer have Early Access health regen.

`1.0.0`

- Release