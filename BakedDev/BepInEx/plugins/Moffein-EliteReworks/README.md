# EliteReworks
This mod seeks to address the longstanding issues with Elite bulletsponge that have been around since the day RoR2 released into Early Access. Elite damage and HP multipliers are reduced, but their spawn cost is decreased and their abilities are more impactful. You might also start to see elite bosses earlier into runs now, due to their reduced cost.

All players need the mod.

# Changes
- **General:**
	- T1 Elites:
		- Cost reduced 6x -> 4.5x
		- HP reduced 4x -> 3x
		- Damage reduced 2x -> 1.5x
	- T2 Elites:
		- HP reduced 18x -> 12x
		- Damage reduced 6x -> 4x
		
	*Vanilla elites are essentially 1shot HP sponges, with their abilities generally being an afterthought that doesn't really come into play when fighting them. This mod seeks to reduce elite tankiness and instead make their abilities more pronounced. Also to compensate for the lower HP, elites have had their spawn cost reduced, so they'll be able to spawn more frequently.*
	
	- Stun/Shock/Freeze now disables most passive elite effects.
	
		*This should allow melee survivors to fare better against elites with passive damage abilities without having to rely on i-frames.*

- **Glacial:**
	- Attacks have an AOE that slows for 3 seconds (think Behemoth, but slowing instead of damaging).
		- Inner AoE slows for 3s, outer AoE slows for 1.5s.
	
		*This lets Glacials actually use their slow effect more often.*
		
- **Overloading:**
	- Shields removed.
	- On-hit lightning bomb radius increased from 3m -> 7m
	- Passively scatters 5 lightning bombs nearby every 6 seconds.
		- Each deals 36 damage, scaled to enemy level.
	- Stun/Shock/Freeze disables the passive lightning bombs.
	
	*Vanilla Overloading Shields were frustrating to fight (especially on bosses), and their on-hit bombs had such a small AoE that they never ended up being much of a threat unless you got direct-hitted. The new passive lightning effect is a callback to their zap AoE from RoR1, with the potential to deal high damage while still being avoidable. The increased AoE on the lightning bombs makes them a threat that you need to pay attention to.*
		
- **Blazing:**
	- Fire trails damage now scales based on level, instead of damage.
	- Stun/Shock/Freeze disables the passive fire trail.
	
	*Fire trails are very unpredictable due to being scaled off of enemy damage. Some enemies won't do much damage, while others will melt you in a few ticks. This change makes Blazing trails consistent across all enemies, which should make them more predictable to fight as melee characters.*

- **Malachite:**
	- Malachites now have a passive anti-heal AOE.
	- Malachite spike damage is capped at 50% of your current HP.
	- Malachite spikes now apply Anti-Heal + Weaken for 8 seconds.
	- Stun/Shock/Freeze disables their passive spikes + anti-heal AOE.
	
	*Vanilla Malachites suck to fight. Their anti-heal is an interesting way of neutering the massive healing players can get from items, but it never really gets much use in practice since it requires you to get hit by one of their near instant-kill attacks to trigger it. These changes seek to make Malachites less about 1shotting, and more about denying heals. Malachites now have a passive anti-heal AOE around them to make sure that their anti-heal actually gets use, and their spikes act more like traps that slow players and keep them inside the AOE, rather than instant kill anti-melee landmines.*

- **Celestine:**
	- Removed vanilla behavior.
	- Attaches to up to 4 nearby enemies.
		- Attached enemies gain +20% damage, +50% attack speed, +70% movement speed, and -30% cooldown reduction.
		- On death, they revive as a ghost and will continue to live on for up to 60s.
			- Ghosts lose their Elite bonuses.
		- Killing a Celestine kills all their attached ghosts.
	- On-hit effect changed to -20 armor instead of slowing.
	
	*Instead of covering the map in ugly gimmicky bubbles, Celestines now buff their teammates and make them more aggressive, and will keep them in the fight even if they are killed.*

- **Mending:**
	- Stun/Shock/Freeze disables healing.
	
- **Voidtouched:**
	- Collapse replaced with Void Reaver Nullify
		- 1 stack per hit
		- Lasts 8s (scales with proc coefficient)
		- Now only takes 2 stacks to root.
	- Removed built-in -30% damage penalty.
	- Now gets a +50% damage bonus to match other elites.
	
	*Vanilla Collapse suffers from the same issue as Early Access Blazing where it scales off of enemy base damage, leading to cheap instakills.*
	
- **Gilded:**
	- Spike damage now scales based on level, instead of damage.
	- Stun/Shock/Freeze resets Spike cooldown.
	- On-hit Gold Siphon now siphons gold directly to reduce lag.
	
- **Twisted:**
	- Projectile damage now scales based on level, instead of damage.

## Installation

Place EliteReworks.dll in /Risk of Rain 2/BepInEx/plugins/