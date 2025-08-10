This mod compiles a bunch of tweaks to vanilla content, most of these came from RiskyMod.

With this mod, the goal was to keep things mostly Vanilla-feeling, and only sticking to changes that wouldn't require in-game descriptions to be rewritten and changes that are unlikely to impact content-adding mods.

Vanilla-Compatible, some tweaks are client-side, some are server-side. Check the config, all tweaks can be toggled!

## General

- Barrier Decay is slower at low amounts.
- Shock no longer gets cancelled by damage.
- Cloak position updates are slower.
- On-Standing-Still effects trigger faster.

## Survivors

- Acrid
	- Regenerative now counts as healing, and isn't affected by Monsoon/Drizzle regen multipliers.
	- Poison is no longer damage capped.
	- Blight now resets duration on stack.
	- M1 hitbox buffed.
	
- Artificer
	- Snapfreeze now fires as soon as you release the button.
	- Ion Surge height no longer scales with movement speed. (Can be changed in-game)
	- Flamethrower burn is now guaranteed, reverting the SotV nerf.

- Bandit
	- Hemorrhage ignores armor.
	- Primary auto fires when holding the button.
	- Blast pierces enemies.
	- Blast spread is reduced.
	- Serrated Dagger has a larger hitbox.
	- Serrated Dagger lunges forwards.
	- Smokebomb can be triggered by holding the button.
	- Special no longer cancelled by sprint.
	- Special only fires when releasing the button.
	
- Captain
	- M1 has no falloff when fully charged.
	
- Engineer
	- Mobile Turrets always sprint, have more range, have fall damage immunity, and no longer have Early Access health regen.
	
- Huntress
	- Tracking angle is wider and tracks the enemy closest to your crosshair.
	
- Loader
	- M2 and Shift no longer cancel sprinting.
	
- Mercenary
	- Now has normal melee health regen.
	- M1 Expose combo hit no longer scales with attack speed. (Can be changed in-game)
	
- MUL-T
	- Scrap Launcher cooldown scales with attack speed.
	- Scrap Launcher no longer has random spread.
	- Scrap Launcher ICBM Synergy
	- Retool reloads primaries.
	
- REX
	- Seed Barrage is now affected by armor to be consistent with his other self-damage skills.
	- Utility knockback against enemies is stronger and more consistent.
	
- Railgunner
	- Polar Field reduces projectile damage.
	
- Void Fiend
	- Corrupt transition duration is faster.
	- Primary no longer has random spread.
	- Uncorrupted Trespass no longer scales with movement speed. (Can be changed in-game)
	- Corrupted Crush fires faster and has no use limit.
	
- Seeker
	- Default M2 no longer modifies FOV.
	- Meditate now stuns and cleanses projectiles.
	
- False Son
	- Removed Slam's hidden non-scaling 0.7s cooldown.
	- Air Slam proc coefficient reduced from 1.5 -> 1
	- Laser proc coefficient increased from 0.45 -> 1
	
- CHEF
	- Dice min return delay reduced from 1s -> 0.2s, and now scales with attack speed.
	- Glaze is no longer cancelled by Sear.
	
## Autofire Options

- Captain
- Engineer
- Bandit (if Primary Autofire is enabled)
	
## Items

- Warbanner spawns on Mithrix Phase 1 and in Simulacrum.
- Gasoline deals damage faster at higher stacks.
- Roll of Pennies is disabled in the Bazaar.

- Shuriken no longer procs Bands.
- Ghor's Tome
	- Disabled in Bazaar.
	- All money is given to the person who picked it up.
	
- Bottled Chaos no longer triggers Vase/Egg.
- Frost Relic
	- Disabled FOV modifier.
	- Disabled bubble.

- Visions of Heresy cooldown scales with Attack Speed.

## Equipment

- Preon Accumulator lightning tendrils no longer proc Bands.
- Remote Caffeinator can now trigger pressure plates.

## Minions

- Teleport distance threshold is much lower.
- Most allies regen to full HP in 40s. Affected by Difficulty regen multipliers. Disabled if RiskyMod is installed.
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
	
- Gunner Turrets no longer need to reload.

- TC-280
	- Reduced cost from $350 to $300

## Interactables

- Teleporter is now replaced with the Primordial Teleporter after looping, like in 1/Returns.
- Blood Shrine now is guaranteed to give at least 1 small chest per 50% HP.
- Mountain Shrine director cost now scales with playercount.
- Shrine of Combat gives less money, but drops white items for the team on completion.
	- Limited to 3 per map.
	- Director cost scales with playercount.

## Artifacts

- Vengeance Umbras are now a part of the Void team.
- Vengeance Umbras receive 90% less healing from heal effects that scale off of max health percentage.
- Vengeance Umbras deal 90% less damage with N'kuhana's Opinion.
- Vengeance Umbras no longer take fall damage.
	
## Stages

- Bulwark's Ambry is now guaranteed to drop a key every 25 kills.

- Void Fields
	- Reverted Seekers Phase 2 fog buff.
	- Reverted Seekers Phase 2 monsters gaining items while outside the bubble.

- Commencement
	- Pillars drop items.
	
- Void Locus
	- Nerfed fog damage to be consistent with Void Fields.
	- Signals drop items.
	
- Planetarium
	- Nerfed fog damage to be consistent with Void Fields.

## Enemy Mechanics

- Enemies can now die from fall damage.
- Enemies no longer have regen. (Only applies to a few enemies, the regen amount was insignificant and more like an oversight than an actual feature)
- Enemy AI now has full vision, and knows where the player is at all times. (So that they don't get stuck idling in random parts of the map)
- Teleporter Bosses are less likely to repeat between stages.
- Enemies no longer heal on levelup.
- Ambient Level cap is now 9999, like Simulacrum.
- Monsters spawned at the start of the map now give the same amount of money as Teleporter monsters.

## Enemies

- Beetles have a bigger hitbox and slightly buffed attack speed and movement speed.

- Child no longer has i-frames.

- Golem Claps now deal consistent damage, instead of scaling off of AoE distance.
- Brass Contraption attacks are interruptable by stun and freeze.
- Scorch Wurm no longer has i-frames.

- Halcyonite
	- No longer has stun/freeze immunity during certain attacks.
	- No longer has Void immunity.
	- Shrine-spawned stat boosts capped at +20 (12x HP, 4x damage)

- Parent director cost is lowered to account for the Anniversary Update nerf.

- Xi Construct sticks much closer to players.
- Grandparent Sun immediately stops dealing damage once a player is behind cover.

- Lunar Wisps
	- Now affected by Stun/Freeze.
	- Hitscan attack has falloff.
	- Director cost is increased.

- Mithrix
	- No longer takes fall damage.
	- Phase 4 guarantees an additional item return on hit, on a 15s cooldown.