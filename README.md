pool shows pearl on ping
should Bandit specials execute?
Void Reaver secondary gets cancelled by sprint

# To-Do
## Backend
- [X] add wiki page for `DebugToolKit` macros and uses
- [CUSTOM] make printer behavior in singleplayer match `ShareSuite`
  - this will remove the option to print and then use Recycler on the item (or other behaviors), but will make the mechanic more consistent

## UI
- `BetterUI`
  - [?] could potentially reimplement item counters, would need to individually assign a value to each item
  - [?] should I attempt to remove the menu button?
  - [?] buff tooltips are hard coded, otherwise appear blank
    - `WolfoQoL` additional buffs do not have descriptions either
- `Pingprovements`
  - [ ] does pinging a "hidden" item (ie `BiggerBazaar`) show different information to clients and hosts
- `WolfoQualityOfLife`
  - [?] corrects a ton of the wrong descriptions and adds some missing ones; be sure to check against this when making language edits
- [CUSTOM] find a way to apply `Pingprovements` colors to scanners
  - uses "game-defined tier color"
- `HuntressBuffULTIMATE`
  - [HACK] hardcodes Energy Drink description incorrectly; doesn't match with BetterUI item stacking (which is also hardcoded)
    - potential solutions:
      - create a custom version that doesn't edit Energy Drink (and doesn't have a stupid name)
        - if AutoSprint has custom dependencies on this mod, that would break things
      - override the item description with a custom language mod and a soft dependency
        - might need to do this anyways with other mods that make language edits at runtime

## Gameplay
- `ChensMinionRetarget`
  - [CUSTOM] doesn't seem to have any effect on minion targeting at all; might be worth creating a more brute-force version like old `AllyPing`
- `EphemeralCoins`
  - [BUG] currently breaks when loading with `ProperSave`; coin count is shown as 0 at all times, and profile coins are used instead
    - https://github.com/VarnaScelestus/RoR2/issues/8
    - could go back to modifying profile?

## Balance
- `WolfoQualityOfLife`
  - [ ] should there be 3 lunar seers?
    - doesn't result in duplicates, gives full control of next stage vs 2/3 chance, conflict still unknown
  - [?] changes many abilities to no longer disable Red Whip; should I document this on the wiki?
- [ ] should I change eclipse levels like GeneralFixes?
- [ ] should red-to-white cauldron only give 3 whites?
- `GestureEnigma`
  - [ ] should Gesture autofire?
  - [ ] does this mod change the description accordingly?

- RevisedShieldOSP (https://thunderstore.io/package/VarnaScelestus/Enhanced_OSP/ possible alternative)
- other Wolfo mods

## Potential Additions
- BiggerBazaar
- BazaarPrinter
- InstantTeleporter
  - [ ] need a solution that keeps the timer honest, but also doesn't make Focused Convergence useless
- https://thunderstore.io/package/Moffein/Clay_Men/
- artificer, huntress tweaks
- CloakBuff
- alternate elites
- Direseeker
  - would like to see a third optional boss for mushroom map to make behavior consistent
- alternate survivors
  - lesser Heretic/HereticUnchained?
  - Paladin
    - https://thunderstore.io/package/Moffein/PaladinHealthTweak/
  - Enforcer
  - Dancer
  - Miner
  - Han-D
- ~~ScalingBloodShrines~~
- GrovetenderBuff (deprecated)

# Mechanics I Want To Change
- [CUSTOM] asynchronous Aquaduct buttons
- [CUSTOM] two question marks or duplicate item in shops
- [X] Gesture behavior
- [CUSTOM] impact nades
- [?] other behavior from HarbTweaks
- [?] viable Tonic build
  - reduce CD?

# New Content
- Shrine of Randomization
  - could potentially use the shrine of order model with a shader applied, might be easier

# Custom Event Logging
- data
  - stage switches, stage count
  - lunar coins gained/spent
  - item gained, rarity
  - game time @ each event
  - player/monster level at stage start
- would be ideal if data was parsable for getting averages

# Survivors of the Void Changes
https://riskofrain2.fandom.com/wiki/Survivors_of_the_Void_Update

- Eclipse is available in multiplayer
- Void Fields
  - timer doesn't pause
  - cell vents drop a Void Potential
  - DoT scales with level and is no longer affected by damage reduction or dodge chance
    - correction: appears that the damage is actually 2.5% of current health/s
- Acrid
  - animation cancel removed; sprint now starts next attack in the chain
    - [ ] this may have consequences with autosprint
  - jumps no longer collide with enemies, meaning you can't hit airborne stuff with them
- Artificer
  - secondaries are no longer hold-to-charge
  - flamethrower damage-per-tick buffed
    - [ ] tooltip apparently still incorrect
    - scales the number of damage ticks with attack speed; probably affects total damage done, meaning the tooltip might never be accurate?
- Captain
  - DIABLO can damage allies
- Commando
  - [ ] Suppresive Fire apparently has a recast?
- Burn Damage
  - max damage-per-tick based on max health (unchanged); however, no longer duration-based but based on a total damage pool; means higher health pools no longer take more total damage
  - ignite condition added and clarified; total damage pool is equal to 50% of the impact damage
- chest spawns
  - "large variants of damage, healing, and utility chests"
- cleansing pools are more common
- lobbies remember the last played character instead of defaulting to Commando
  - [ ] could have adverse effects with custom characters
- some item tooltips have been updated
  - [ ] interstellar desk plant 5m base radius is "still incorrect"
- Brittle Crown refunds lost money upon using a Shrine of Blood or a self-damaging skill
- Simulacrum
  - [ ] bugged; scavenger augment drops a lunar, not a red
