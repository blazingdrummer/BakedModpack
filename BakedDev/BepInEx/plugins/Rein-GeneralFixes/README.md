This mod contains a few (more to come) balance changes, QOL, and bugfixes for the base game, aimed at removing exploits and normalizing item strength while also smoothing out some of the rougher edges in gameplay.

## Feedback (Please? I'll beg if needed)
- I am extremely open to any kind of feedback, question, suggestion, bug report, or really anything.
- I have a simple discord set up to help keep bug reports and feedback organized for all my mods, feel free to join and all that.
- https://discord.gg/TgaDGNh
- You can also DM me on discord if that is easier. (@Rein#7551)

### Install
- Delete old versions. (You never know)
- Unzip the plugin zip.
- Copy all files to the plugins folder in Bepinex(in your game install directory)
- Bonus points if you create a separate folder inside the plugins folder for every mod

### Uninstall
- Delete the files that come with the mod from the plugins folder

### New this update (2.4.4)
```
    Adjustments:
- Eclipse 1 health boost: 30% -> 20%
- In eclipse 3, if the survivor does not have a doppelganger set up a commando doppelganger spawns instead (temporary fix until I do a larger thing here)
- Will o wisp starting damage: 400% -> 300%
- Will o wisp damage per stack: 100% -> 300%
    This is actually from a weird typo and misunderstanding.
- Captain utility cooldown: 14s -> 18s
    The buff given to utility was massive, a 50% damage increase. In order to keep captain from falling back into utility and M1 spamming this is 100% required.

    Bugfixes:
- Improved compatibility with other mods that use the eclipse modifiers
- Razor wire now properly scales bleed damage instead of duration
- Shatterspleen no longer applies two stacks of bleed on crit (still stacks properly with tri tip)

    Removed:
- Removed fix for captain repeat scrapping passive item as it was added to base game.
```


# What's Inside

## QOL
### Eclipse
- Eclipse 1: Starting health reduction removed. Monsters now have +30% max health.
    Starting health reduction is very low impact, especially for some characters (rex) switching to boosting enemy health has meaningful impact at all times and also doesn't lead to annoying deaths when your survivor pod lands on a flock of golems.
- Eclipse 3: Instead of enabling frailty, it enables vengance.
    Unity's physics engine was not all designed for games with lethal fall damage. You can launch yourself to orbit just by looking at a wall the wrong way and pressing spacebar. Generally speaking, all frailty does is kill you when the physics decides to bug out, and this is boring. Vengance is at least interactive.
- Eclipse 8: Permanant damage removed, replaced with heavy exponential enemy scaling.
    The purpose of eclipse 8 for me is to loop as far as I possibly can, Permanant damage makes going past a few stages completely impractical, and effectivley kills the whole point of the mode in my opinion. While yes, this can be thought of as being a bit easier, that is only the case when your goal is the final boss. Generally speaking, at stage 16 the strength of all enemies is twice what it would be on monsoon with this change, and it keeps getting more insane from there. Reaching 30-40 stages should be borderline impossible, and thats what makes it fun.

### Visions of Heresy
- Now assigns a new crosshair to characters that use SimpleDotCrosshair (Huntress and Mercenary)
- Makes it easier to aim properly on those characters.
- (I will likely have some extra functionality added to this in the future to allow you to specify which crosshairs are replaced, potentially with an in-game console command)
- Swaps crosshair back to default when visions is not the active primary.
- Does not interfere with skills like Ballista, which change the crosshair for their duration. 

### Engineer Turrets
- Now inherits elite affix equipment from you.
- Tuned their blacklist for certain inherited items.
- New blacklist: Halcyon Seed, Rusted Key (this does nothing on turrets anyway), Focused Convergence, Warbanner, Beetle Gland, Lepton Daisy
- Vanilla blacklist: Warbanner, Beetle Gland, Lepton Daisy.
- Mainly added things that are similar to what vanilla disallows.

## Bugfix

### Bandolier
- Now properly refunds stock for skills that restore more than one stock per recharge.
- This is not the same as simply making bandolier automatically max your stock. It only applies to specific skills that recharge multiple stock at once on a timer.
- Examples are Scrap Cannon and Visions of Heresy.

### Self Damage
- Focus crystal can no longer apply to self damage.
- Crowbar can no longer apply to self damage.
- AP Rounds can no longer apply to self damage (Although not sure how you would manage this one)
- Self damage includes Tincture and Meteor.
- Rex self damage was never affected by these items.

### DoT Stacking
- Allowed a single hit to apply multiple stacks of a DoT.
- For example, an attack marked as PercentBurnOnHit when combined with FireAffix will now apply two stacks of burn instead of 1.
- This effects both enemies and players. Blazing elder lemurians are scarier, but so is sawmerang with tri tips.
- Generally this isn't a major change though, most runs you will never run into a situation where it becomes a factor.

## Balance
### Elites
- Base cost multiplier reduced to 5.75 from 6.
- Just a small change that makes the cost : hp ratio of elites a bit less horrible.

### Commando Secondary
- Phase round CD changed to 2s

### Corpsebloom
- Maximum reserved healing increased to 200% (+200% per stack) from 100% (+0% per stack).
- Base maximum healing per second increased to 15% from 10%.
- Maximum reserved healing is now calculated from: (Max Health + 25% of Max Shield) instead of just Max Health.
- Maximum healing per second is now calculated from: (Max Health + 25% of Max Shield) instead of just Max Health.

### Oneshot Protection
- Now only applies to your health. Both shields and barrier are simply subtracted from incoming damage.
- Hits for more than 360% of your maximum HP now bypass oneshot protection (So stacking health is still relevant)
- The window of protection in vanilla still works.
- This also means that shield generators no longer can cause weird situations with OSP.
- A different way to think about this mechanic: On losing more than 90% of your max health within a very short time, gain a temporary barrier for 270% max health that is placed between health and shield.

### Gesture of the Drowned
- No longer grants cooldown reduction
- Certain items now have no interaction with auto cast (crowdfunder and effigy)
- These changes are not applied if you have Equipment Durability by Jarlyk installed

### Blight
- Blight now resets stack timers on application (Just like bleed)
- Blight duration 5s -> 4s
- Blight is now applied by acrids primary
- Hopefully brings blight to a good spot where it can compete with poison

### Focused Convergence
- Cap increased from 3 stacks to 10 stacks.
- Teleporter radius is now multiplied by 0.75 per stack. (Exponential)
- Charge rate is now divided by 0.8 per stack. (Exponential)
- For reference. At 7 stacks the TP zone is the size of the teleporter itself. At 7 stacks the teleporter also will charge to full in roughly 21 seconds.
- Generally just gives you a reason to pick up the item.

### WillOWisp
- Damage increased to 400% + 100% per stack.
- Base radius increased to 15.
- Radius no longer scales with stacks.
- Let's be real, we all know that this item was busted...


## Changelog
### 2.4.4
```
    Adjustments:
- Eclipse 1 health boost: 30% -> 20%
- In eclipse 3, if the survivor does not have a doppelganger set up a commando doppelganger spawns instead (temporary fix until I do a larger thing here)
- Will o wisp starting damage: 400% -> 300%
- Will o wisp damage per stack: 100% -> 300%
    This is actually from a weird typo and misunderstanding.
- Captain utility cooldown: 14s -> 18s
    The buff given to utility was massive, a 50% damage increase. In order to keep captain from falling back into utility and M1 spamming this is 100% required.

    Bugfixes:
- Improved compatibility with other mods that use the eclipse modifiers
- Razor wire now properly scales bleed damage instead of duration
- Shatterspleen no longer applies two stacks of bleed on crit (still stacks properly with tri tip)

    Removed:
- Removed fix for captain repeat scrapping passive item as it was added to base game.
```

### 2.4.3
```
    New:
- Razor Wire:
    Now inflicts bleed for 2 seconds
    Damage multiplier on the bleed scales from 1.0 to 0.25 based on distance relative to max range of razor wire
    No longer deals damage
    No longer can crit
    No longer has a proc coef
        
        This should give razor wire a more clearly defined use than just "Imp overlord/void delete button"
        In particular, characters that tend to take hits at close range such as Acrid, Loader, Mercenary, and MulT (saw) will benefit greatly

    Adjustments:
- Captain:
    Utility damage reverted to vanilla values
    Utility cooldown: 12s -> 14s
    Primary base minimum charge time: 0.1s -> 0.05s
    Primary base max charge time: 1.2s -> 1s
    Primary delay: 0.9s -> 1.05s

    Bugfixes:
- Updated to match the r2api standard for networkmodlist entry format
- Fixed error with shock beacons after death
```

### 2.4.2
```
    New:
- Captain:
    Shocked enemies now take 400% damage when the shock ends from damage. (1.0 proc coef, also can hit nearby enemies)
    The damage portion of shock works against bosses
    Shocked now counts as a debuff for death mark
    Shock beacon now deals 100% damage with 1.0 proc coef per tick
    Primary damage per pellet: 120% -> 100%
    Primary proc coef: 0.75 -> 0.7
    Utility cooldown: 11s -> 12s
    Utility damage: (1500% | 500% | 500%) -> (750% | 750% | 750%)
    Passive: Now only given on the first stage (Scrap it once and its gone forever, your drones still get it though)

    The goal here is to spread strength from utility and primary to M2 and beacons, without destroying his core identity of limited use zone control.
    I am looking in to changes to the other beacons, but for now know that running even double shock is totally viable with this setup.

    Adjustments:
- Gesture break chance removed
- Gesture no longer grants any equipment cooldown reduction
    Gesture currently is an extremely unhealthy item. Its upside (the extremely high cooldown reduction) and its downside (auto cast) interact with eachother far too much.
    Auto cast is only a downside on some equipment, and the cooldown reduction is so powerful that rather than auto cast being seen as the downside of gesture, it effectively becomes a downside attached to all equipment that can't make use of the auto casting.
    In fact, some equipment like tonic end up with the auto cast being an upside in its own right.
    Decoupling the auto cast from the cooldown reduction is the best way to approach this issue without massively interfering with existing builds.
- This mod now has an interaction with Equipment Durability by Jarlyk.
    If Equipment Durability is present, gesture keeps its vanilla cooldown reduction
- Blight stacks applied for poisoning skills: 2 -> 1
    Bite retains ability to apply 2 stacks
- Blight damage multiplier: 1.0 -> 0.5
- Blight duration: 3s -> 4s
    These changes are actually not a significant nerf. Enemies tended to die far too quickly before you could really stack blight up, this addresses that.
- Acrid base jump power: 15 -> 20
    So you can hit wisps just a bit more easily
- Doppelganger health bonus: 900% -> 500%   (only on eclipse)
- Doppelganger damage multiplier: 0.04 -> 0.08 (only on eclipse)

    Bugfixes:
- Fixed character select errors with eclipse 3
- Fixed doppelgangers dropping 2 items
- Some general networking stuff
- Things that I likely am forgetting right now
```
### 2.4.1
```
    New:
- Bleed:
    Tri tip chance per stack 15% -> 7%
        Its not a purely early game item anymore, so it should take a bit more to get going
    Tri tip duration proc coef scaling now works off the square root of your proc coef.
        This is a substantial buff for attacks that have lower proc coefs.
    Tri tip chance proc coef multiplier now works off the square root of your proc coef.
        This is also a substantial buff
    Some odd stacking mechanics removed with sawmerang
        This should have minimal impact, it may be a very slight nerf in some cases, but once you start stacking tri tip and shatterspleen it is a buff
- Burn:
    Ignite, PercentBurn, and Fire Affix now all apply their burns independently instead of overwriting eachother.
        Arti is now able to use wake of vultures nicely, fire blazing elder lemurians are scarier.
- Blight:
    Blight now resets stack timers on application (Just like bleed)
    Blight duration 5s -> 3s
    Blight is now applied by acrids primary
    2 stacks of blight are applied by poisoning abilities

    Adjustments:
- Elite base cost multiplier: 5.5 -> 5.75
    5.5 was just a bit too extreme

    Bugfixes:
- Fixed fall damage issues
- Fixed networking
- Fixed acrid blight not working
```


### 2.4.0
```
    New:
- Elite base cost multiplier: 6 -> 5.5
    Their health is just too low for their massive cost compared to normal enemies, so rather than reverting the health changes I made them a bit less expensive. This means you will see them a bit more often. (for every 12 elites you will see 1 more)
- Eclipse 1: Starting health reduction removed. Monsters now have +30% max health.
    Starting health reduction is very low impact, especially for some characters (rex) switching to boosting enemy health has meaningful impact at all times and also doesn't lead to annoying deaths when your survivor pod lands on a flock of golems.
- Eclipse 3: Instead of enabling frailty, it enables vengance.
    Unity's physics engine was not all designed for games with lethal fall damage. You can launch yourself to orbit just by looking at a wall the wrong way and pressing spacebar. Generally speaking, all frailty does is kill you when the physics decides to bug out, and this is boring. Vengance is at least interactive.
- Eclipse 8: Permanant damage removed, replaced with heavy exponential enemy scaling.
    The purpose of eclipse 8 for me is to loop as far as I possibly can, Permanant damage makes going past a few stages completely impractical, and effectivley kills the whole point of the mode in my opinion. While yes, this can be thought of as being a bit easier, that is only the case when your goal is the final boss. Generally speaking, at stage 14 the strength of all enemies is twice what it would be on monsoon with this change, and it keeps getting more insane from there. Reaching 30-40 stages should be borderline impossible, and thats what makes it fun.


    Adjustments:
- Removed commando roll changes (Now in vanilla game)
- Removed death mark changes (Now in vanilla game)
- Disabled DoT stacking until I have a chance to fully test the major code changes in the base game in this area.
- Merged Hopoo's OSP changes and my own. (so now it has a maximum protection, works vs clustered hits, and treats your shield as barrier instead of health)
```

### 2.3.0
- Removed unneded R2API dependency
- Compatible with Artifacts update
- Added Blight balance
- Added Focused Convergence balance
- Added Death Mark balance
- Added WilloWisp balance
- Added DoT stacking fix
- Added Engi turret QoL
- Added Sacrifice QoL
- Made sure Gesture changes work properly with enigma (Gesture will not break enigma, I hope)

### 2.2.1
- Fixed bug with bandolier changes. (No longer gives credit towards next cooldown)
- Exponentially improved the overall balance of the character selection lobby. In fact, some might say it is *too* balanced, so I added a config option to disable this.

### 2.2.0
- Improved compatibility with Dilluvian Difficulty
- OSP max damage taken threshold increased to 211% from 180% (This number scales with OSP threshold, so dilluvians 99% threshold reduces it to 201%)
- Fixed Focus Crystal, Crowbar, and AP Rounds applying to self damage.
- Fixed crowdfunder constantly firing with gesture. (Crowdfunder was immune to breaking, and doesn't benefit from gesture upside, so I removed all interaction)
- Fixed effigy activating with gesture. Same reason as above.
- Added delay to equipment break for some equipment that have cast times or durations (Wings, tonic, preon, ect.)
- Sound will play on activation if equip will break, and sound plays a second time when it actually does break.
- During delay before being destroyed, if you switch equipment (by picking one up, or being MulT) the equip you were holding is destroyed immediately.
- Fixed errors with engineer turrets and visions of heresy.

### 2.1.0
- Added Corpsebloom balance changes.
- Added Visions of Heresy QOL.
- Added Overgrown Printer QOL.
- Added Bandolier bugfix.
- Fixed gesture break chance being 0.05% instead of 5%.
- Gesture break chance reduced to 2.5% (Mostly as a precaution. Very likely to go up to 5% in future)
- A sound now plays when your equipment breaks.
- Relocated the gesture break hook to improve compatibility and fix bugs.

### 2.0.0
- Total remake
- Expanded to cover both balance and bugfixes.

### 1.0.1
- Removed the walker turret attack speed scaling (devs added it to vanilla)

### 1.0.0
- First release
