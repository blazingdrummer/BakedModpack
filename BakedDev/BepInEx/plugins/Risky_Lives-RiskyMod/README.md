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

`0.10.7`

- Razor Wire
	- Damage and Range no longer scale off of HP lost
		- Now is always a fixed 160% (+40% per stack) damage and 25m range.
	- Proc coefficient (0.1-0.5 based on HP lost) now maxes out at 10% HP lost
		- Old Value: 50% HP lost
	
	*Reworked version was feeling underwhelming in most situations, so I'm simplifying it and moving it closer to Vanilla. Proc coefficient thing is there to tone down the effectiveness of Helfire + Razorwire.*

`0.10.6`

- Artificer
	- Electrocute
		- Reverted gauntlet VFX change due to syncing issues.

`0.10.5`

- Artificer
	- Electrocute
		- Increased damage from 900% -> 1000%
		- Increased lightning bounce distance from 15m -> 20m
		- Fixed the skill being unable to crit in multiplayer.
		- Fixed the gauntlet firing effect positioning in multiplayer.
			- Was showing at Artificer's server-side position instead of Artificer's client-side position. Not sure if this is better or worse for readability, since the lightning still is calculated from the server-side position.

- Items
	- Ghor's Tome
		- Now gives the full reward to the person who picked it up, instead of splitting it among the team.
		- No longer can be picked up by NPCs.
			- Only applies to Player team.
		
	- Needletick
		- Collapse now gives -1 armor per stack.
		
		*This item is strong earlygame, but falls off lategame and in multiplayer due to Bleed's better stacking behavior. Armor reduction should be small enough to not make a difference earlygame at low stacks, while providing some sort of benefit to high stacks while looping. Number is the same as Scorpion, but is tied to a temporary chance-based debuff rather than being permanent.*
		
	- Plasma Shrimp
		- Proc chance is now affected by proc coefficient.

- Enemies

	*Changes marked with 🔥 are disabled when playing on the Inferno difficulty.*

	- Lemurian
		- 🔥 Reduced melee lunge distance.
		
	- Stone Titan
		- Now always uses the laser for the full duration (8 seconds).
		- Reduced laser damage bonus from +80% -> +60%
		- Tweaked laser targeting, trying to see if this makes it smoother.

`0.10.4`

- Mercenary
	- Fixed Eviscerate being broken due to 0.10.2

- Allies
	- Incinerator Drone
		- Added shields.
		
- Enemies
	- Added "Inferno Compatibility" config option to disable certain enemy changes while Inferno is active to prevent conflicts. These changes will be marked by 🔥. (Enabled by default)
	- Beetle
		- Reduced move speed from 10m/s -> 8m/s (Vanilla 6m/s)
		- Increased headbutt duration from 1s -> 1.2s (Vanilla 1.5s)
		- Doubled headbutt hitbox size.
		- Increased AI headbutt activation range from 2m -> 5m
		- Reduced spawn duration from 5s -> 3.2s
		
		*Trying to make these look less jank, since the heavy stat boosts made their animations really jerky. AI Headbutt range increase will make Beetles more aggressive with using their headbutt, instead of only using it when they're practically inside of you.*

	- Lemurian
		- 🔥 Added melee lunge.

	- Imp
		- Added melee lunge when slashing.

`0.10.3`

- Spawnpools Beta
	- Rallypoint Delta
		- Disabled all changes since the last Vanilla update fixed Pests replacing Imps instead of Wisps.
	- Sky Meadow
		- Lunar Golem director credit cost reduced from 125 -> 115 (same as Elder Lemurian)

`0.10.2`

- Run Scaling
	- Teleporter Bosses are less likely to repeat for multiple stages in a row.
		- Remembers the last 2 teleporter bosses and tries to exclude them from the boss selection if possible.
		
		*Limited to 2 because most stages only have 3 basic bosses.*
		
	- Loops increase teleporter boss credits by 1 Mountain Shrine.
		- Does NOT affect item drops.
		
		*It takes way too long before Elite Bosses start to show up regularly. This should help with that.*

- Items
	- Queen's Gland
		- Added partial compatibility with QueensGlandBuff
			- Now uses QueensGlandBuff settings for damage scaling if it is installed.
			- Now uses QueensGlandBuff settings for HP scaling if it is installed.
			
			*Note: This ignores QueensGlandBuff's changes to how many beetles you can have, which is why this is listed as only being partially compatible. The mod and its ally changes work fine (and worked even before this update).*
		
- Mercenary
	- Eviscerate no longer stops on teammates if Chaos is disabled.

`0.10.1`

- Removed debug text when loading the mod.

`0.10.0`

- Firemode Selection (Credits to Nunchuk for the keybind code from CustomEmotesAPI)
	- Most Firemode settings can now be configured in-game via Risk of Options.
		- Will probably not add RoO support for most other config options due to issues with network syncing if they're changed mid-game.
		
- Allies
	- Turret allies now receive -66% damage from Mini Mushrum attacks.
	
- Items
	- Ukulele
		- Increased proc coefficient from 0.1 -> 0.2 (Same as Vanilla)
		
		*Polylute remains at 0.1 proc, hoping this makes it more of a choice when deciding between the two.*
		
	- Sentient Meat Hook
		- Increased proc coefficient from 0.1 -> 0.33 (Same as Vanilla)
		
		*This makes it the same as Vanilla. I don't think it's a major balance concern since most other proc chaining items have been disabled.*
		
	- Symbiotic Scorpion
		- Reduced armor reduction from 2 -> 1
		
		*Trying to make this a bit more even compared to Shattering Justice.*
		
- Enemies
	- Stone Golem
		- Reduced melee damage from 40 -> 30
		- Removed melee damage falloff.
		
	- Magma Worm and Overloading Worm
		- Reduced follow delay from 0.6s to 0.1s (inspired by Inferno)
		- Tried to make players a higher priority for the AI.
			- Not sure if this actually works.
		- Now fires fireballs in both stances, instead of only when leaping.
			
			*Is this too spammy?*
			
	- Stone Titan
		- Animations are faster.
			- FireFist exit delay reduced from 3s -> 1.5s
			- RechargeRocks duration reduced from 9s -> 5s
			- ChargeMegaLaser duration reduced from 3s -> 2s
			
			*Titans can't attack much because their anims take a ridiculously long time.*
			
		- Mega Laser
			- Increased damageCoefficient from 1 -> 1.8
			- Increased tick frequency from 8/s -> 10/s
				- Damage has been adjusted proportionally.
			- Increased shot radius from 0 -> 0.2
			- Reduced cooldown from 20s -> 15s
			- Removed lock-on.
			- Removed minimum distance check.
			- Increased max distance from 80m -> 200m
			- Now scales with attack speed.
			
			*Trying to shift laser from being a "hide behind cover" check to something that you actively dodge and interact with. Can be easily avoided, but deals high damage if it catches you off-guard. Needs playtesting.*
			
		- Lowered max aim velocity from 180 -> 60
		
			*This is to prevent the Mega Laser from jerking around erratically. Other skills are auto-targeting so I'm not too concerned about this.*
			
		- Stone Fist
			- Increased fist count from 1 -> 4 (Aurelionite is 6)
			
		- Stone Construct
			- Now directly targets enemies, instead of being tied to where the Titan is looking.
		
	- Aurelionite
		- Copied Titan changes.
		- Increased base damage from 40 -> 50
		
		*Early Access Aurelionite was notoriously bullshit, but nowadays people rarely die to it. Starting with a small increase due to the major Titan changes.*
		
- Commando
	- Suppressive Fire
		- Lowered direct hit damage from 100% -> 20%
		- Lowered direct hit proc coefficient from 1.0 -> 0.5
		- Increased AoE damage from 20% -> 100%
		- Increased AoE proc coefficient from 0.5 -> 1.0
		
		*Swapping the numbers on the Direct Hit/AoE to make this better at dealing with bunched up enemies.*
		
	- Suppressive Barrage (Scepter)
		- Lowered direct hit damage from 100% -> 20%
		- Lowered direct hit proc coefficient from 1.0 -> 0.5
		- Increased AoE damage from 20% -> 130%
		- Increased AoE proc coefficient from 0.5 -> 1.0
	
- Artificer
	- Blaze Storm (Needs Playtesting)
		- TODO: ICON
		- Now lists damage as Damage/Second (Like Arrow Rain/Directive: DRILL).
		- Increased total damage from 1500% -> 1920%
		- Increased lifetime from 3s -> 6s
		- Reduced tickrate from 3.33/s -> 2.5/s
			- Tick damage has been increased proportionally to compensate.
		- Fixed the skill using yellow damage numbers instead of the default color.
		
		*Trying to shift this more towards being an area control skill as was originally intended. With these changes, total damage is higher while immediate burst DPS is lower (500% DPS over 3 seconds -> 320% DPS over 6 seconds). Meant to be comparable to Arrow Rain and Directive: DRILL.*
		
	- Electrocute (Special) (Needs Playtesting)
		- TODO: ICON
		- Electrocute all enemies in front of you for 900% damage.
			- Range: 40m
			- Locks on to 1 enemy near your crosshair
				- If a target is found, lightning will chain to nearby enemies within 15m.
				- If no target is found, just fires a bolt of lightning forwards.
			- Hits 15 times, scales with attack speed.
		
		*Does this even work online? Intended to be more reliable than Flamethrower and good at dealing with flying trash, but worse at dealing with bosses and tanky enemies. DPSwise this is lower than your primaries, but it's guaranteed to hit. Needs balancing and polish.*
		
	
	- Unlimited Power (Electrocute Scepter)
		- Increases damage from 900% -> 1800%
		- Increases chain lightning range from 15m -> 20m
		- Increases chain lightning max bounces from 1 -> 2
	
- Captain
	- Power Tazer and Beacon: Shocking
		- Now applies a 50% move speed slow for 5s.
		
		*This should make these skills more useful when fighting unshockable enemies.*
		
	- Beacons
		- Added config option to enable infinite Lysate Cell stacking (disabled by default).
		
	- Beacon: Hacking
		- Moved Skill Recharge effect to Beacon: Resupply
		- New Effect: Reduces the cost of interactables in its radius by -40%
			- Does not stack.
			- Removing your Beacon reverts the prices to normal.
		- Added option to disable this beacon in the config for those who don't want to play with Hack Beacons at all.
		
		*The Skill Recharge effect from the rework would become unavailable depending on whether or not the host wanted to use Vanilla Hacks or Reworked Hacks, and often caused confusion among Captain players. To address this, the Skill Restock effect has been merged with Resupply beacons, and Hack beacons have been moved closer to their Vanilla effect so that there isn't such a big shift in functionality.*
		
	- Beacon: Resupply
		- Reduced Equipment recharge amount from +1 Stock -> -20s Cooldown
		- Increased uses from 2 -> 3
		- Reduced use recharge time from 30s -> 20s
		- Now restores skills as well (1 Bandolier worth)
			- Only restores 50% of Diablo Strike's cooldown.
			
		*The dedicated Skill Recharge beacon ended up being too niche. Thematically, Skill Restock/Equipment Restock have a pretty similar effect, and both beacons weren't very popular on their own, so merging them seemed like the right choice.*
	
- Acrid
	- Regenerative (Needs Playtesting)
		- Slowed down full heal duration from 1.5s -> 3s
		- No longer loses duration when taking damage.
		
		*Original intent behind duration loss on hit was to force Acrid to hit and run instead of facetanking, but it ended up feeling bad in practice due to how he could suddenly get every stack of Regenerative cancelled at the same time. Plan is to try to balance around Regenerative healrate instead. Will be challenging since Bite makes a huge difference to Acrid's regen speed.*
		
	- Frenzied Leap
		- Increased cooldown reduction from 0.7s -> 1s
		
		*This skill ended up lagging behind in MP due to enemies not bunching up as much as in solo, along with the loss of 1 jump being a huge mobility penalty in general.*

- Loader
	- Reduced armor from 12 -> 0
		
- Void Fiend
	- Fixed Safer Spaces being triggered when fall damage is blocked by the Utility's buff effect.
		
- Spawnpools Beta (Disabled by default)
	
	*Disabled by default. Can be enabled in the Core Modules section of RiskyMod_General.cfg*
	
	- Current Issues:
		- Enemy compositions feel off on certain maps (ex. Sky Meadow)
		- Probably has weird interactions with Family events.
		- DLC checks currently don't work.
	
	- General Notes:
		- Jellyfish/Wisps/Pests are intended to not overlap on the same map.

	- Stage 1
		- Titanic Plains
			- Removed Jellyfish
			- Removed Alpha Constructs
			- Removed Xi Constructs
			
		- Distant Roost
			- Removed Lesser Wisps
			- Jellyfish can now spawn on the first loop.
			- Added Alpha constructs when looping (Requires SotV)
			
			*Alpha Constructs mirror Hermit Crabs, and work nicely with how there's a lot of tightly-packed surfaces for the projectiles to bounce off of.*
			
		- Snowy Forest
			- Removed Lesser Wisps
			- Added Bighorn Bisons when looping
		
	- Stage 2
		- Wetland Aspect
			- Removed Lesser Wisps
			
		- Abandoned Aqueduct
			- Clay Apothecaries can now spawn on the first loop. (Requires SotV)
				- Does this actually work?
			- Added Magma Worms when looping
			- Added Overloading Worms when looping
			
			*Figured this stage could use stronger enemies since Aphelian Sanctuary has both Templars and Apothecaries on loop 1.*
			
	- Stage 3
		- Rallypoint Delta
			- Imps now spawn even when SotV is enabled.
			- Removed Lesser Wisps (Requires SotV)
			
	- Stage 4
		- Stadia Jungle
			- Removed Lemurians
			- Removed Clay Dunestrider
			- Mushrums spawn less
			- Added Grovetender
			- Added Vultures
			
			*Trying to make the spawnpool on this map less generic.*
			
		- Sirens Call
			- Added Overloading Worms
			
	- Stage 5
		- Sky Meadow
			- Removed Alpha Constructs
			- Removed Xi Constructs
			- Removed Bronzongs
			- Added Imps
			- Added Lunar Golems
			- Magma/Overloading Worms now spawn even when SotV is enabled.
			
			*I don't like Alpha Constructs since they take up enemy slots and AFK on the other side of the map. Split on whether or not removing Xi Constructs is the right call. Removed Bronzongs and replaced them with Lunar Golems since the map has too many flying enemies, along with Lunar Golems being a parallel to RoR1's Temple Guards.*