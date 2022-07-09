# EliteReworks
This mod seeks to address the longstanding issues with Elite bulletsponge that have been around since the day RoR2 released into Early Access. Elite damage and HP multipliers are reduced, but their spawn cost is decreased and their abilities are more impactful. You might also start to see elite bosses earlier into runs now, due to their reduced cost.

Updates will probably slow since I don't have a lot of time to develop/test things, so feedback will be super helpful.
Open an issue on the GitHub or send me a DM if you have any thoughts.

All players need the mod.

# Current Balance Concerns
- How are the Celestine changes?
- Are Overloading enemies threatening?
	- Does the passive lightning do enough damage?
	- Does the passive lightning punish melee characters too much?
	- Is the on-hit effect doing anything relevant?

# Changes
- **General:**
	- T1 Elites:
		- Cost reduced 6x -> 4.5x
		- HP reduced 4x -> 3x
		- Damage reduced 2x -> 1.5x
	- T2 Elites:
		- HP reduced 18x -> 12x
		- Damage reduced 6x -> 3.5x
		
	*Vanilla elites are essentially 1shot HP sponges, with their abilities generally being an afterthought that doesn't really come into play when fighting them. This mod seeks to reduce elite tankiness and instead make their abilities more pronounced. Also to compensate for the lower HP, elites have had their spawn cost reduced, so they'll be able to spawn more frequently.*
	
	- Stun/Shock/Freeze now disables most passive elite effects.
	
		*This should allow melee survivors to fare better against elites with passive damage abilities without having to rely on i-frames.*

- **Glacial:**
	- Attacks have an AOE that slows for 3 seconds (think Behemoth, but slowing instead of damaging).
	
		*Vanilla Glacials pretty much don't do anything. This change should hopefully make them better at slowing players.*
		
- **Overloading:**
	- Shields removed.
	- On-hit lightning bomb radius increased from 3m -> 7m
	- Passively scatters 5 lightning bombs nearby every 6 seconds.
		- Each deals 36 damage, scaled to enemy level.
	- Stun/Shock/Freeze disables the passive lightning bombs.
	
	*The main feature of vanilla Overloading is bosses healing half of their HP pool if you focus on something else for a bit. These changes are intended to shift Overloading enemies into being less about tanking, and more about chaotically spamming projectiles everywhere, hopefully leading to a more engaging experience when fighting them.*
		
- **Blazing:**
	- Fire trails damage now scales based on level, instead of damage.
	- Stun/Shock/Freeze disables the passive fire trail.
	- Reverted burn mechanics to pre-SotV.
	
	*Fire trails are very unpredictable due to being scaled off of enemy damage. Some enemies won't do much damage, while others will melt you in a few ticks. This change makes Blazing trails consistent across all enemies, which should make them more predictable to fight as melee characters.*

- **Malachite:**
	- Malachites now have a passive anti-heal AOE.
	- Malachite spikes now deal 50% of your current HP.
	- Malachite spikes now apply Anti-Heal + Weaken for 8 seconds.
	- Stun/Shock/Freeze disables their passive spikes + anti-heal AOE.
	
	*Vanilla Malachites suck to fight. Their anti-heal is an interesting way of neutering the massive healing players can get from items, but it never really gets much use in practice since it requires you to get hit by one of their near instant-kill attacks to trigger it. These changes seek to make Malachites less about 1shotting, and more about denying heals. Malachites now have a passive anti-heal AOE around them to make sure that their anti-heal actually gets use, and their spikes act more like traps that slow players and keep them inside the AOE, rather than instant kill anti-melee landmines.*

- **Celestine:**
	- Removed vanilla behavior.
	- Attaches to up to 4 nearby enemies.
		- Attached enemies gain +50% attack speed, +70% movement speed, and -30% cooldown reduction.
		- On death, they revive as a ghost and will continue to live on for up to 60s.
		- Killing a Celestine kills all their attached ghosts.
	- On-hit effect changed to -20 armor instead of slowing.
	
	*Instead of covering the map in ugly gimmicky bubbles, Celestines now buff their teammates and make them more aggressive, and will keep them in the fight even if they are killed. Need to fine-tune the effectiveness of ghosts/buffed enemies.*

- **Mending:**
	- Stun/Shock/Freeze disables healing.
	
- **Voidtouched:**
	- Collapse replaced with Void Reaver Nullify
		- 1 stack per hit
		- Lasts 8s (scales with proc coefficient)
	- Removed built-in 30% damage penalty.
	- Now gets a +50% damage bonus to match other elites.
	
	*Vanilla Collapse suffers from the same issue as Early Access Blazing where it scales off of enemy base damage, leading to cheap instakills. Originally wanted to swap it to 50% of the hit's damage, but was having trouble with setting that up so I changed it to Nullify instead.*

## Installation

Place EliteReworks.dll in /Risk of Rain 2/BepInEx/plugins/

## ChangeLog

- 1.7.0
	- Celestine
		- Added VFX to show which enemies are connected to which Celestine.
		- Champion Celestine enemies now get +2 extra max attached ghosts. (6 total)
		- Ghost lifetime increased from 30s -> 60s
		- Champion Ghosts now get +30s lifetime.
		- Ghost damage increased 30%
			- Does not apply to alive enemies.
		
		*Ghosts were expiring too fast to do anything. Increased duration should make killing the host Celestine a higher priority, since Ghosts won't simply disappear if you leave them alone for a short while.*

- 1.6.1
	- Celestine on-hit change can now be toggled via config.

- 1.6.0
	- Glacial
		- Sound now only plays when the buff is first applied.
		- Slow duration modifier at the edge of the blast increased from 25% to 50%
		
		*Glacial slow was feeling too irrelevant due to the duration falloff changes from earlier updates.*
		
	- Overloading
		- Passive Lightning
			- Now always shoots 5 projectiles regardless of enemy size.
				- This generally means less projectiles from most enemies.
			- Tweaked blast radius
				- Blast radius increased from 3m -> 5m
				- Boss blast radius increased from 3m -> 7m (same as Overloading Worm)
			- Boss projectiles now use Overloading Worm VFX.
			- Non-boss projectiles now have quieter VFX.
		
			*It ended up being nearly impossible to actually get hit by Overloading projectiles since the radius was too small. New radius is roughly the same as an Overloading Worm's lightning bombs.*
		
		- On-Hit Lightning
			- Now is the same as Vanilla, but with a bigger blast radius (3m -> 7m) and different SFX.
			- Old scatterbomb behavior can be re-enabled in the config.
			
			*The on-hit scatterbombs looked cool, but didn't actually do much and ended up being too spammy for my liking. Moving these closer to Vanilla, but leaving the old behavior in for those who liked it.*
		
	- Malachite
		- Antiheal buildup time reduced from 4s -> 3s

- 1.5.1

	*Quick hotfix update to fix Voidtouched Templar stunlocks.*
	
	- Voidtouched
		- Now has a +50% damage bonus to match other T1 elites.
		- Nullify
			- Proc chance now scales off of proc coefficient
			- Duration changed from 8 x proc coefficient -> 8 x sqrt(proc coefficient)
		
			*Voidtouched Templars could stunlock you in a fraction of a second with no way to fight back due to guaranteed procs. This change will make it so that they have to shoot at you for a decent amount of time before you get stunned.*
			
	- Overloading
		- Added config to individually enable/disable the passive and on-hit lightning reworks.
		- Shield config is now locked behind Enable Overloading Changes since each part of the rework can be toggled individually now.
	
	*Plans for the next update:*
		*- Make Overloading/Glacial sounds less noisy.*
		*- Take a look at Overloading balance. They currently spam a lot of projectiles, but the projectiles don't actually do much and rarely hit.*

- 1.5.0
	- Fixed for the DLC update.
	- Reduced T2 Elite HP Multiplier from 14 -> 12
	- Added config options for modifying T1 Honor stats (left as Vanilla by default)
	- Mending
		- Stuns/Shock/Freeze interrupt healing.
	- Voidtouched
		- Replaced Collapse with Nullify.
		- Removed built-in 30% damage penalty.

- 1.4.3
	- Fixed new config options not working.

- 1.4.2
	- Added missing EliteAPI submodule dependency. This should fix errors with certain mod setups.
	- Added config options for Elite Cost/HP/Damage multipliers.

- 1.4.1
	- Added additional network checks to Malachite stuff.
	- Corrected incorrect Malachite buildup time in the previous version chagelog.

- 1.4.0
	- Elite Passive stun bonus duration reduced from 2s -> 1.2s
	- Malachite
		- AOE antiheal now builds up over 4s.
		- Every 0.8s, a stack of Antiheal Buildup is applied (similar to Shattering Justice).
			- Each stack reduces healing by 20%
			- At 5 stacks, it becomes the full antiheal debuff.
		- Leaving the radius or stunning the Malachite will cancel the antiheal buildup.
		
	*Malachites being able to instantly shut down all healing in an AOE immediately upon spawning ended up countering melee characters too hard. With this change, the Malachite AOE should be more manageable.*

- 1.3.0
	- Now uses R2API's EliteAPI for better compatibility with mods that add custom elites.
	- Increased T2 Elite Spawncost/HP
		- Spawn Cost multiplier increased from 15 -> 36	(same as Vanilla)
		- HP multiplier increased from 10 -> 14
		
*T2s were spawning way too often, constantly spamming Spikes/AOE effects. Seeing as their abilities are generally more impactful compared to Vanilla, the greatly increased spawnrate was making things too much of a clusterfuck to deal with. T2 spawnrate is now the same as Vanilla, while their HP is a halfway point between Vanilla and the value from previous versions.*

- 1.2.1
	- Fixed Celestine Reviving not being affected by stuns due to the previous update.

- 1.2.0
	- Stunning/Freezing/Shocking Elites now disables passive effects for an additional 2s after the stun ends.
	
	*This should help make Malachite and Blazing Elites more manageable for melee characters who don't have I-frames.*

- 1.1.0
	- Glacial
		- Slow duration modifier at the edge of the blast reduced from 50% to 25% to match vanilla blast scaling.
	- Overloading
		- Passive bombs from bosses deal 60% more damage.
	- Blazing
		- Passive fire trail from bosses deals 60% more damage.
		
	*Boss Elite Passive damage has been increased to bring back the Vanilla mechanic of Elite Bosses dealing more damage with their passives. The damage increase is based on the difference between an Imp/Imp Overlord, as that is a Vanilla example of an effect balanced around base damage (Imp Bleed). On-hits are unchanged.*

- 1.0.0
	- Overloading
		- Fixed multiple Overloading enemies on the map causing passive bombs to be spammed.

- 0.2.1
	- Glacial
		- ZetAspects: Fixed mod slow stacking on top of vanilla slow. Both buffs can still be applied, but their slow no longer stacks on top of each other.
	- Celestine
		- Once an enemy is attached (30m range), they must be greater than 45m away to detach.
		
	*Celestines would often pass by random enemies and buff them briefly, before unbuffing due to getting out of range. This should help them be more consistent.*

- 0.2.0
	- Celestine
		- No longer beta, is now enabled by default.
		- No longer receives a stat boost for possessing enemies.
		- Possessed Enemy Stats
			- Cooldown Reduction increased 25% -> 30%
			- Move speed increased 50% -> 70%
			- Attack speed increased 30% -> 50%
		- Added extra null checking when attempting to spawn ghosts.
		- Removed simple indicator option due to code clutter + the rework being enabled by default.
		
	*Feedback on Celestines would be grealty appreciated! Need to fix Overloading enemies shooting out way more passive bombs than intended sometimes before I can make the mod 1.0.0*

- 0.1.7
	- Celestine (Beta)
		- Max active ghosts increased 3 -> 4
		
	*Felt that being limited to 3 ghosts made them not very impactful. I'd like to add a target prioritization system to make them prioritize buffing stronger enemies sometime. Once that's in, I'll probably be moving the rework out of beta and enabling it by default.*

- 0.1.6
	- Celestine (Beta)
		- Ghosts now lose their elite affixes.
	
	*It was near impossible to tell what type of elite a ghost is since they all use the same ghost texture, and allowing stuff like Malachites to become ghosts and continue AOE suppressing heals while there was no way to stop/stun them felt bad.*

- 0.1.5
	- Added a network check when adding the Elite ability handler components. Hopefully this should fix Overloading enemies sometimes spitting out tons of passive lighting projectiles.

- 0.1.4
	- T2 Elites
		- Damage reduced 4x -> 3.5x
		
	*4x damage seemed to bring them back into constant 1shot territory, so I'm putting it at a halfway point between the old 3x damage and the damage in the previous update.*
	
	- Glacial
		- Fixed slow duration being able to exceed 2.5s on attacks with a proc coefficient greater than 1.0 (Jellyfish).
	
	- Celestine (Beta)
		- No longer slows on-hit. Now just reduces armor by -20.
		- Reduced max active ghosts from 7 -> 3
		- Ghost lifetime reduced 30s -> 20s.
		- Attached enemy move speed increased 30% -> 50%.
		- Attached enemies now gain -25% cooldown reduction.
		
	*There were too many movement slows from too many different sources (Glacials, Malachite Spikes), so Celestines no longer slow on hit. Max ghost count has been cut down since it got out of hand really quickly (3 random Celestines in a crowd would turn into 21 ghosts). In exchange for a lower ghost count, ghosts now have increased stats. I wasn't sure how I'd go about with increasing their stats to make them more threatening, since simply increasing damage ends up being unfun and 1shotty, so I've tried reducing their cooldowns and boosting their move speed to make them more aggressive.*

- 0.1.3
	- Fixed Glacials not actually using blast falloff.

- 0.1.2
	- Celestine (Beta)
		- Tweaked visuals. Hoping this should improve readability.
			- Now, only Celestines show a particle effect (the warbanner icon).
			- Enemies attached to Celestines now have a red tint.
			- Celestine Ghosts now have a red tint.

	- Overloading
		- On-hit explosives now scatter randomly
		
	*With the lower blast radius, the bombs from on-hit attacks weren't really hitting their mark consistently. Randomizing their scatter pattern should help make them more of a threat, while their lowered blast radius from the earlier update should keep them dodgeable.*
		
	- Glacial
		- Duration reduced from 1s + 2s(proc) to 0.5s + 2s (proc)
		- Getting hit on the edge of the blast (>50% of the blast radius) now reduces slow duration by 50%.

- 0.1.1
	- Celestine (Beta)
		- Celestines now gain +30% attack speed and movement speed while controlling ghosts.
		- Celestines now show a particle effect while controlling ghosts. (this didn't work)
	
	*This should help with visiblity.*
	
	- Overloading
		- Passive damage increased 32 -> 36.
		
	*Felt that their passive damage is a bit too low considering how it's harder to get hit by lightning now. Let me know if this ends up being too high, or if it's not high enough.*
		
- 0.1.0
	- T2 Elites
		- Cost increased 12x -> 15x
		- HP increased 8x -> 10x
		- Damage increased 3x -> 4x
		
	*Felt T2 Elites were spawning too often, so I've upped their cost and increased their HP a bit to compensate. Damage has been increased since I felt they weren't threatening enough damagewise, but it's still considerably lower than their vanilla damage multiplier.*
		
	- Celestine (Beta)
		- Disabled by default, must be enabled in the config.
		- Removed vanilla behavior.
		- Attaches to up to 7 nearby enemies.
			- Attached enemies gain +30% attack speed and movement speed.
			- On death, they revive as a ghost and will continue to live on for up to 30s.
			- Killing a Celestine kills all their attached ghosts.
		- On-hit effect changed to Cripple (like Perfected elites)
			
	*Unsure about this, lemme know if this is any fun to fight, or if I need to go back to the drawing board on this one. Ideally I'd like to have a line or some sort of indicator to show which Celestine each enemy is connected to, but I have no clue how to network it. Thoughts would be greatly appreciated.*
		
	- Overloading
		- Increased passive lightning damage from 28 -> 32
		- Increased on-hit lightning damage from 50% -> 70%
		- Reduced on-hit lightning AOE from 5m -> 3m
		- Lightning bomb explosion noise reduced (now just makes a generic shock explosion sound effect).
		- Reworked cooldown behavior:
			- Overloading enemies have a stock of 20 bombs that fully recharge over 1.6s
			- Attack bomb count scales off of proc coefficient, and uses up bombs from the stock.
		
	*Overloading Lightning in its current state essentially is just low but guaranteed free damage to things nearby. Experimenting with making it stronger but with a tighter AOE so that it's more based around dodging. Reworked cooldown behavior is mainly there to make Overloading Templars and other rapid-hit enemies look less jank, the amount of bombs they can put out should be about the same. Thoughts on these changes would be greatly appreciated.*
		
	- Blazing
		- Increased fire trail damage from 18/s -> 21/s
		
	- Glacial
		- Slow duration partially scales with proc coefficient now.
			- Slow is guaranteed to last for at least 1 second, while the remaining 2 seconds will scale off of proc coefficient.

	*Glacial wisps were being a bit too oppressive, being able to shotgun blast in your general direction and slow you for 3 seconds.*

- 0.0.6
	- Fixed nullref spam with latest version of CHEF.

- 0.0.5
	- Fixed Glacial Elites stunlocking you when ZetAspects is installed.
	- Fixed a bug where you become unable to proc Overloading's effect when using Wake of Vultures (?)

- 0.0.4
	- Overloading passive damage reduced 32 -> 28
	- Overloading on-hit damage reduced 80% -> 50%

- 0.0.3
	- Fixed a bug where Malachite and Overloading enemies could sometimes lose their passive effects.
	- Overloading disable shield config option can now be enabled when Overloading Changes are disabled.
	- Overloading passive damage increased 24 -> 32
	- Overloading on-hit damage increased 50% -> 80%
	- Overloading on-hit bomb count now does not scale downwards with proc coefficient.
	- Overloading on-hit now has a 0.33s cooldown per trigger. This may be raised in the future if it is still lagging a lot.
	- Malachite antiheal AOE radius reduced 25m -> 22m (for reference, Celestine is 30m)
	- Malachite antiheal AOE now has a subtle range indicator.
	- Added config option to hide Celestine bubbles (disabled by default).

- 0.0.2
	- Fixed an incorrect description in the readme.

- 0.0.1 ``Initial Release``