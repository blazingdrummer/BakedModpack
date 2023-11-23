## Risky Artifacts
Adds 8 artifacts to ruin your run with.

- **Artifact of Origination**
	- Bosses invade the map every 10 minutes.
	- Invaders gain +50% movement speed, +30% attack speed, and +20% damage, and -30% cooldown reduction,.
	- Invaders drop items when killed, with a chance to drop their respective boss item.
	- Boss spawn count scales based on playercount and loop count.
	- Config allows for Classic Origin, where only Imp Overlords spawn.

- **Artifact of Arrogance**
	- Mountain Shrines are permanent.
	
- **Artifact of Expansion**
	- Teleporter radius is mapwide, but takes longer to charge.
	- Doubles Moon/Void field holdout radius but increases their charge time.

- **Artifact of Conformity**
	- Prevents scrappers and printers from spawning.
	
- **Artifact of Warfare**
	- Boosts monster movement speed, attack speed, and projectile speed by 50%.
	
- **Artifact of Primacy**
	- The Primordial Teleporter spawns on every stage after looping. 
	
- **Artifact of the Phantom**
	- The Phantom King of Nothing hunts you down if you spend too long on a stage.
		- Spawns after spending 4.5min-6min on a stage.
		- 12000 HP, 200% damage
		- Immune to Void Fog and fall damage.
		- Can die to Void Reaver bubbles.
		- Drops an Irradiant Pearl and 5 Lunar Coins when killed.
		- Begins ravaging the map with explosions after death.
		
- **Artifact of Cruelty**
	- Enemies can spawn with multiple elite affixes.
		- Mainly intended as an artifact to enable post-loop with MidRunArtifacts.
	
## For Mod Devs
If you are making a custom boss and want to add it to the Artifact of Origination spawn pool, add a softdependency to com.Moffein.RiskyArtifacts then do:
`Risky_Artifacts.Artifacts.Origin.AddSpawnCard(Spawncard, BossTier);`

Boss Tier affects when the boss can spawn.

Stage 1-2: 100% chance T1

Stage 3-4: 30% chance T1, 70% chance T2

Stage 5: 25% chance T1, 65% chance T2, 10% chance T3

Stage 5+: 5% chance of Scavengers, 95% chance of Stage 5's boss pool


T1: Beetle Queen (disabled), Titan, Vagrant, Dunestrider

T2: Imp Overlord, Magma Worm, Solus Control Unit, Grovetender, Xi Construct, Void Devastator

T3: Grandparent (disabled)

## Credits

Main Dev - Moffein

Warfare Icon - MinHui12g

Icons for Conformity, Arrogance, Expansion, Origin - KoobyKarasu

Chinese Translation - JunJun_w

Ukrainian Translation - Damglador

Spanish Translation - Juhnter

Portuguese Translation - Kauzok

Cruelty - RyanPallesen's FloodWarning Artifacts

## Installation

Place the Moffein-RiskyArtifacts folder in /Risk of Rain 2/BepInEx/plugins/

## Changelog

`2.0.5`

- Cruelty
	- Enemy rewards now scale. (Default: Additive)

`2.0.4`

- Cruelty
	- Default Special Boss max affixes increased 3 -> 4 so that it matches the affix limit from the previous update (need to update config)

`2.0.3`

- Cruelty
	- Added config option for max T2 affixes (Default: 1)
	- Added config option for max non-T2 affixes (Default: 3)

`2.0.2`

- Cruelty
	- Fixed Special bosses receiving Cruelty bonuses when the artifact isn't active.

`2.0.1`

- Cruelty
	- Added option to make it guaranteed for Special Bosses (Mithrix, Voidling, Aurelionite, AWU, Direseeker), disabled by default.
		- Gets 3 affixes, affix count can be changed in config.
	- Non-elite enemies that get turned into elites now receive the proper HP/Damage multipliers for the first elite affix gained regardless of settings.
	- Artifiact now works if it's enabled mid-stage via MidRunArtifacts

`2.0.0`

- Expansion
	- Changed default price increase from 1.2x -> 1.0x (no increase)
	
- New Artifact: Cruelty (From RyanPallesen's FloodWarningArtifacts)
	- Enemies can have multiple elite types, with increased health to match.
	- Config Options:
		- Scale HP (None/Add/Multiply)
		- Scale Damage (None/Add/Multiply)
		- Scale Cost (None/Add/Multiply)
		
	*Starting ports of some of the old artifacts that used to get run in hosts. Thanks to RyanPallesen for giving me permission to include them here!*

`1.9.6`

- Friendly Origination bosses no longer turn the skybox purple.

`1.9.5`

- Updated BR TL.

`1.9.4`

- Added Brazilian Portuguese translation (Thanks Kauzok!)

`1.9.3`

- Primacy
	- Fixed lunar teleporter having the wrong starting orientation after Void Fields.
		- Now checks if the stage spawns a lunar teleporter naturally, instead of checking stage count.

`1.9.2`

- Arrogance
	- Guaranteed Mountain Shrine no longer spawns on the Moon, Void Locus, and Voidling

- Origination
	- Added config option for invasion timer.
	- Fixed Stage 5+ boss chances being set incorrectly
		- T1 Boss: 16.7% -> 25%
		- T2 Boss: 72.2% -> 65%
		- T3 Boss: 11.1% -> 10%
	- Added Scavengers
		- On stage 5+, adds a 5% chance to overwrite the boss with Scavengers.
		- Half as many Scavengers spawn compared to normal bosses.

`1.9.1`

- Arrogance
	- Fixed Mountain Shrines spawning in intermission levels (Bazaar, Gilded Coast, etc.)

`1.9.0`

- Arrogance
	- Now always spawns an extra mountain shrine like Prestige in Returns.
		- Can be disabled in config.

`1.8.10`

- Origination
	- Changed boss spawnpoint selection from NearestNode to Approximate. This will make it generally less buggy and less prone to instant boss deaths.

`1.8.9`

- Added Spanish translation (Thanks Juhnter!)

`1.8.8`

- Phantom
	- Added min stages config (0 by default).

`1.8.7`

- Phantom
	- Reduced spawn distance from Far to Standard
	- Increased damage multiplier from 2 -> 3

`1.8.6`

- Added Ukrainian translation (Thanks Damglador!)

`1.8.5`

- Origination now supports ArtifactOfPotential from zombieseatflesh7

`1.8.4`

- Added nullchecking to Conformity so the game doesn't error when mods spawn printers in the main menu.

`1.8.3`

- Phantom and Origination now get Evolution items.

`1.8.2`

- Artifact of the Phantom
	- Increased lunar coin drop count from 4 -> 5.
	- Added spawn timer config.

`1.8.1`

- Artifact of the Phantom
	- Reduced spawntime from 5.33min-7min -> 4.5min-6min
	
	*Felt like Mithrix never showed up unless you really took your sweet time farming.*

`1.8.0`

- New Artifact: Artifact of the Phantom
	- The Phantom King of Nothing hunts you down if you spend too long on a stage.
		- Spawns after spending 5.33min-7min on a stage.
		- 12000 HP, 200% damage
		- Immune to Void Fog and fall damage.
		- Can die to Void Reaver bubbles.
		- Drops an Irradiant Pearl and 4 Lunar Coins when killed.
		- Begins ravaging the map with explosions after death.
		
	*Inspired by the ghost from Spelunky. Barely playtested, give feedback! Will add config for spawn times once I have a better feel for how it plays.*

`1.7.3`

- Added Simplified Chinese translation (Thanks JunJun_w!)

`1.7.2`

- Languagefile support.
- Origin
	- Increased boss spawn distance from Close to Standard
	
	*Hopefully this will reduce instances where bosses get instagibbed when spawning.*

`1.7.1`

- Origin
	- Bosses no longer have adaptive armor when looping.
		- Can be re-enabled in the config.
		
	*Disabled since adaptive armor sucks to fight when going against horde bosses.*

`1.7.0`

- Origin
	- Reduced Yellow drop chance from 11% -> 8%
	- Now attempts to drop the corresponding boss's item if possible.
		- Falls back to Green items if there is no boss item available.
		
	*Getting regular Pearls from boss drops felt pretty underwhelming. This behavior should resemble RoR1 more.*

`1.6.1`

- Conformity
	- Added config options to let you only disable Scrappers/Printers, instead of being forced to disable both.

`1.6.0`

- Origination
	- Now tries to avoid repeating the same boss twice in a row.
	- Magma Worms now drop their items at the nearest available navigation node.
	- Fixed Pearls dropping way too often. (Was set to have around a 50% drop chance. Now is more like 10%)
	- Added Xi Construct.
	- Added Void Devastator.

`1.5.1`

- Primacy
	- Added force enable config option. (Disabled by default)

`1.5.0`

- Primacy
	- Added config option to enable it on the first loop. (Disabled by default)

`1.4.11`

- Fixed for real.

`1.4.10`

- Fixed for latest patch?

`1.4.9`

- Conformity
	- Fixed Red/Yellow printers not getting deleted.

- Arrogance
	- Made values public for cross-mod compatibility.

`1.4.8`

- Origination
	- Boss counter no longer increases when spawning new waves in the Artifact Reliquary.
	- Added extra null checks.


`1.4.7`

- Fixed Conformity Disable in Bazaar config option.

`1.4.6`

- Added CannotSteal tag to OriginBonus.

`1.4.5`

- Added OriginBonus to BrotherBlacklist

`1.4.4`

- Fixed incompatibility issues.

`1.4.3`

- Updated for latest R2API update.
- Origin bosses now only show 1 entry on the objective HUD.
- Rewrote Conformity code to work with the new update.
	- Now destroys Printers and Scrappers after they spawn.
	- Might be buggy.

`1.4.2`

- Fixed Expansion not working when ZetTweaks is installed.
- Note: Elites are currently broken due to R2API issues. Should be fixed once that updates.

`1.4.1`

- Removed Conformity debug text.

`1.4.0`

- Updated for DLC update.
- Origination
	- Bosses are now on the Void team (can be changed in config).
	- Bosses now have a chance of dropping Void items if the DLC is enabled.
	- Disabled Grandparents by default.
	- Fixed Grandparents being unable to be disabled.
- Expansion
	- Lowered price multiplier from +30% -> +20%
	- Now affects Void Locus (uses same settings as Void Fields)

`1.3.5`
- Fixed Aetherium's Witches Ring causing Origin Bosses to drop items.

`1.3.4`
- Added missing EliteAPI submodule dependency that was causing errors on certain mod setups.

`1.3.3`
- Origination
	- Disabled per-loop boss count scaling.
	
*This was spawning too many bosses when combined with the +1 Boss Per Invasion change.*

`1.3.2`
- Origination
	- Each invasion spawns +1 extra boss, multiplied by Player Factor and Loop Factor.
	
*Origination Bosses were feeling like too much of a pushover compared to Vengeance/Worms, so their numbers have been increased.*

`1.3.1`
- Added config options for disabling artifacts.

`1.3.0`
- Origination
	- Overhauled Elite selection code so that it can select modded Elite tiers.
		- This breaks the Allow Elite Worms config option because it checks the elite spawning conditions. Mods that remove the Elite Worm restriction will be able to get around this.
	- Item Drop rarity is now based on the Elite Cost Multiplier.
		- Cost >= 3 guaranteed Greens
		- Cost >= 15 gives guaranteed Reds
		- White/Green chances decrease from their base chances to 0% linearly as the cost approaches each threshold.

`1.2.2`
- Origination
	- Made tweaks to spawning and fixed a bug that was causing less bosses to spawn than intended. Hopefully this will fix instances where bosses fail to spawn.
	- Adjusted elite boss drop odds. Since they're tanky and take up a ton of potential boss spawns which would give more loot, they need better drops to account for that.
		- If a T1 Elite drops a Pearl, it will always be an Irradiant Pearl.
		- T2 Elites are now more likely to drop Reds instead of Pearls.
		- TODO: Convert this into a consistent function that takes in a Elite's cost multiplier and adjusts drops based on that.

`1.2.1`
- Readme update.

`1.2.0`
- New Artifact: Artifact of Primacy
	- Primordial Teleporter spawns on every stage after looping.

`1.1.0`
- Origination
	- Reduced spawn count from +0.5 per player to +0.3 per player (same as how the game's difficulty scales with playercount).
	- Now tries to combine spawns into elite bosses if too many are spawning.
		- Elite Bosses drop better loot.
			- T1 Elites drop Uncommons and above.
				- If Honor is active, they drop Commons like normal unless the Ignore Honor setting is enabled.
			- T2 Elites drop Legendaries and Irradiant Pearls.
	- Reduced per-loop spawncount increase from +100% -> +50%
	- Fixed Honor bosses having more HP than intended.
	- Added config to disable forced elites for Honor.
	- Added config for what bosses can spawn.
	- Added config to disable particle effect.

`1.0.11`
- Origination
	- Fixed a bug where bosses sometimes wouldn't spawn if players are dead.
	- ??? now adds 3 extra bosses per stack.

`1.0.10`
- Origination
	- ??? now adds 2 extra bosses per stack.
	- ??? extra boss count now increases with each loop.
	- Fixed a bug where ??? stacks sometimes wouldn't be counted when spawning bosses.

*In RoR1, a single Unstable Watch could net you 7+ imps per spawn. Hoping this should make it easier to get a party going in 2.*

`1.0.9`
- Origination
	- Fixed bosses never dropping Pearls.

`1.0.8`
- Origination
	- Formula now only rounds downwards at the end so that it scales properly for even playercounts.
		- New formula is Floor((0.5 + 0.5 x LivingPlayers) x Floor(StagesCompleted/5))

`1.0.7`
- Origination
	- Bosses now only get Adaptive Armor after looping.
	- Each loop now causes extra bosses to spawn.
	- Redid how the total amount of bosses is calculated. This should fix bosses sometimes failing to spawn if certain players are dead.
		- New formula is Floor(0.5 + 0.5 x LivingPlayers) x Floor(StagesCompleted/5)

*I found that Origin bosses were feeling a bit too tanky early-on when you don't have the DPS to burst them down, but become trivial once you start looping and reach the point where you can burst them in seconds. Hoping to address both of these issues with this update. Considering making it so that multiple bosses combine into 1 elite boss if too many are spawning, but at the same time a large part of the appeal of Origin in RoR1 is the sheer amount of bosses that could spawn from it, so I'm leaving it as-is for now.*

`1.0.6`
Fixed the mod breaking when ProperSave isn't installed.

`1.0.5`
- Arrogance
	- Now supports ProperSave (Thanks kumakuma215!)

`1.0.4`
- Origination
	- Fixed bosses failing to spawn if a player is too far from an AI node.

`1.0.3`
- Origination
	- Spawn count reduced to 1 boss for every 2 players.
	
*In multiplayer, Origination can end up feeling like a cheap run-ender due to the sheer amount of HP and area suppression the bosses have, compared to regular Vengance clones who only become dangerous later into the run. This spawncount change should more closely match with how RoR2's difficulty scales with playercount, and will make taking ??? more impactful.*

`1.0.2`
- Origination
	- Damage bonus reduced +50% -> +20%
	- Attack speed bonus reduced +50% -> +30%
	- Cooldown Reduction bonus reduced -40% -> -30%
	
*The damage bonus was set to 1.5x to be lower than a T1 Elite's damage bonus, but it ended up being too much when combined with all their other attributes. -40% cooldowns and +50% attack speed were proving to be too much with Ancient Wisps, so they've been reduced slightly.*

`1.0.1`

- Fixed Expansion applying to the escape ship's holdout zone.

`1.0.0`

- Release