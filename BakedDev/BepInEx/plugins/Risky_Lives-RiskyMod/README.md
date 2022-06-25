## RiskyMod
A full-game overhaul that aims to bring it closer to RoR1's balance. My main priority is multiplayer, but the mod is balanced in solo as well.

I highly recommed installing https://thunderstore.io/package/Moffein/EliteReworks/ to go with this.

Full change list can be found at https://docs.google.com/document/d/1Igxdur0M33fdkcDLYgDEbLE0M4-89gSTorxgdn-oyKs/

This mod merges in fixes and tweaks from a bunch of other mods. If you have those mods installed, these fixes/changes will disable and the original mod will take priority (Except for Bandit Grace Period).

Feel free to take features of this mod and release them as standalone as long as you link the original GitHub repo in the README.

## Main Features

- Removed proc chains.
- Oneshot Protection now actually works.
	- Oneshot = Going from >90% HP to 0% HP in under 0.5s
	- Once triggered, you have to be out of danger (no damage for 7s) before it can be retriggered.
- Shields gate against HP damage like the Guardian's Heart in RoR1.
	- Transcendence/Perfected Affix disable Oneshot Protection due to having shieldgating built-in.
- Big balance pass over nearly all the items.
	- Bad items like Squid Polyps and Warbanners have gotten substantial buffs.
	- Strong damage items like AtGs and Elemental Bands now have lowered damage stacking.
	- Most forms of range scaling have been removed, and most items aren't able to proc chain anymore.
- Big balance pass over all the Survivors
	- Less useless skill options, default Commando is good now!
- Drone performance now remains the same on all stages.

## Other Changes

- Combat Shrines give less money, but drop items for the team on completion.
- Teleporter radius expands once the boss is dead.
- Tweaked Commencement
	- Only 2 pillars are required to activate the jump pads.
	- Pillars drop items for the team on completion, and you can complete as many as you want.

## Installation
Place RiskyMod.dll **AND** the **language folder** in /Risk of Rain 2/BepInEx/plugins/RiskyMod

## Planned Changes (Not implemented yet)

*Mostly done with everything I've wanted to do with the mod. Plan going forward is to iron out the existing balance and do a bit of spawn pool tweaking. I don't like the state that Pennies/Watch/Elixir are in, and Corpsebloom/Desk Plant are still bad, but they probably won't get changed. I personally just blacklist them when playing.*

- Make Google Doc more readable/pretty.
	- Split up into multiple separate docs?
- Tweak enemy pools?
	
## Credits

Drone Targeting fix - ZetTweaks

Squid Polyp distraction - DestroyedClone

Language Support - Anreol

Skill Icons - KoobyKarasu

Acrid Hitbox Tweaks - TheTimesweeper

Buff Icons - SOM

## Changelog

`0.9.7`

- Happiest Mask
	- Fixed the item attempting to proc on pots/barrels/eggs.
	- Reduced damage from 1500%(+450%) -> 800%(+240%)
	
	*Noticed ghosts shredding Mithrix/Overloading Worms within seconds even after multiple loops.*
	
- Commando
	- Frag Grenade
		- Fixed skill selection not being saved when closing the game.

`0.9.6`

- Fixed Safer Spaces description showing 7%/stack instead of the Vanilla 10%/stack.

	*This was a change from an early version when the SotV Update first released, which quickly ended up getting scrapped.*

`0.9.5`

- Ocular HUD
	- Fixed Railgunner/Bandit gaining crit chance instead of crit damage.
	
- Planula
	- Added option to disable order-of-operation changes for compatibility with other mods that change Planula.
		- RiskyMod disables Vanilla Planula code and moves Planula procs so that they run after Stealthkit/Squids are procced.
	
- Improved error handling for better mod compatibility.
	- IL Hooks will now print an error to console instead of causing the whole mod to crash if an incompatibility arises while the plugin is being loaded.
		- A lot of code was moved around internally, so let me know if any issues suddenly arise with this version.

`0.9.4`

- Artificer
	- Added RTAutoSprint support for Blaze Storm and modded Snapfreeze.

`0.9.3`

- Moon Pillars Drop Items
	- Fixed Pearl Overwrite Chance setting not working.
	
- Void Signals Drop Items
	- Fixed Pearl Overwrite Chance setting not working.

`0.9.2`

- Shrine of Combat Items
	- Removed an extra space in the notification string.
	
- Leeching Seed
	- Fixed description showing the old heal percents.

`0.9.1`

- Items
	- Defense Nucleus
		- Increased HP from 0% (+30%/stack) -> 300% (+150%/stack) to match the new Vanilla scaling.
		- Increased damage from 0% (+100%/stack) -> 300% (+150%/stack) to match the new Vanilla scaling.

`0.9.0`

*Releasing this earlier than expected due to the Vanilla update breaking the previous version. Let me know if there's any bugs or if I accidentally left some unfinished changes in.*

- Artificer
	- Blaze Storm
		- Changed sounds and VFX.
	
- Void Fiend
	- Tresspass
		- Gives +30% movement speed and fall damage immunity until you hit the ground after exiting the skill.
		
- Player-Controlled Monsters
	- Now immune to Stun/Hitstun.

- Run Scaling
	- Modded Scaling
		- Now is handled via a less-intrusive hook instead of replacing the whole method, since only 1 value is changed.
		- Increased per-player exponential factor from 0.1 -> 0.15 (Vanilla is 0.2)
	- Loop Boss Armor
		- Increased from 40 -> 50
		- Now applies to all Champion enemies, instead of just Teleporter Bosses.
		
		*Applies to all Champion enemies now because they all die before they even get a chance to fire off their attacks. The armor bonus alone isn't enough to let bosses keep up while looping. Look at making Elite bosses appear as TP bosses earlier?*
		
- Gold Scaling
	- Now enabled by default.
	- Merged all config options into a single option.
	- Scale Gold to Initial Stage Difficulty
		- Reverted 0.8.0 change
			- Now only multiplies by Ratio instead of Ratio^2 since it had too much impact earlygame.
			
	*Generally, the new scaling should keep the first few stages feeling roughly the same, while Stage 5+ will require a bit more farming than Vanilla instead of being able to instabuy the whole stage. Feedback will be helpful for fine tuning this.*
	
- Shrine of Combat Items
	- Shortened text.
	
- Enemies
	- Fall Damage
		- Monsters can now die from fall damage.
		- Monsters take +50% extra damage from fall damage.
		- Mithrix is now immune to fall damage.
		
	- Xi Construct
		- Now takes +50% more damage while its chassis is open (firing its laser).
		
		*Need to figure out how to make it less cancer for melee characters to fight later.*
		
	- Magma Worm (TODO)
		- Revert Early Access HP nerf, make the head a +50% damage weak zone for all characters?
		- Fireballs leave pools of fire?
		
- Items
	- Safer Spaces
		- Now has a 0.1s invulnerability period after triggering.
		
		*This will make the item able to gate against multiple hits in the same frame. With the latest update, this technically allows for full invincibility at around 50 stacks, but I think it should be fine since that will only really happen in Bazaar lobbies.*
		
	- Old Guillotine
		- Increased HP threshold from 30% -> 50%
		
		*In terms of Effective HP reduction, Guillotines were pretty lackluster compared to other Green items. This should make them less situational.*
		
	- Chronobauble
		- Increased movement slow from -60% -> -80%
		
		*This increases the actual slowdown from -37.5% -> -44.4%, since slowdown is calculated as 1 / (1 + slow percent)*
		
	- Leeching Seed
		- Reduced healing from 5% (+2.5%) -> 3% (+1.5%)
		- Now heals a flat +1HP on top of the damage-scaled healing.
			- Flat HP is meant for earlygame when your damage will be low.
		
		*Past Lv20, Seeds were outperforming fullcrit Harvester Scythes on most attacks. This lower number should make it so that at full crit, Scythes outperform Seeds for weak attacks while Seeds will outperform Scythes for strong attacks. Need to see how this plays and adjust further, and need to see how this affects earlygame.*