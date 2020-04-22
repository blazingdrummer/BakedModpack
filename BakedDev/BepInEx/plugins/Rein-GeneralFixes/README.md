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

### Minor update
- Fixed compat with latest ror2 version.
- Improved some logic with how death marks from multiple sources stack (if you have more of the item than someone else, you will write over their debuff with your stronger one)
- Acrid blight damage now is based on distance to the enemy. This should help keep it in line with certain items.
- Disabled Sacrifice cloaked chests changes, as I have yet to run numbers with recent changes to sacrifice.
- Death mark now requires 35 total instead of 30 (so rex can't apply it with a single chronobauble...)
- Slightly toned down the rate bonus for focused convergence to match the decrease in radius more accurately.

### New this update
- Removed unneeded R2API dependency
- Compatible with Artifacts update
- Added Blight balance
- Added Focused Convergence balance
- Added Death Mark balance
- Added WilloWisp balance
- Added DoT stacking fix
- Added Engi turret QoL
- Added Sacrifice QoL
- Made sure Gesture changes work properly with enigma (Gesture will not break enigma, I hope)


# What's Inside

## QOL

### Commando Tactical Dive
- Roll no longer interrupts sprinting, and you count as sprinting while rolling.
- Base range reduced (But the fact that you are sprinting causes the distance to end up exactly the same)
- This means that items like Rose Buckler and Little Disciple are active while you are rolling.

### Visions of Heresy
- Now assigns a new crosshair to characters that use SimpleDotCrosshair (Huntress and Mercenary)
- Makes it easier to aim properly on those characters.
- (I will likely have some extra functionality added to this in the future to allow you to specify which crosshairs are replaced, potentially with an in-game console command)
- Swaps crosshair back to default when visions is not the active primary.
- Does not interfere with skills like Ballista, which change the crosshair for their duration. 

### Overgrown Printers
- No longer blacklisted from certain special items.
- This means Halycon Seed, Pearls, and Iridescent Pearls can all appear in overgrown printers.
- Reasoning: Overgrown printers are just as rare as Military Printers. They should have a similar potential to change your run.

### Engineer Turrets
- Now inherits elite affix equipment from you.
- Tuned their blacklist for certain inherited items.
- New blacklist: Halcyon Seed, Rusted Key (this does nothing on turrets anyway), Focused Convergence, Warbanner, Beetle Gland, Lepton Daisy
- Vanilla blacklist: Warbanner, Beetle Gland, Lepton Daisy.
- Mainly added things that are similar to what vanilla disallows.

### Sacrifice
- Cloaked chests are no longer blacklisted from spawning when sacrifice is enabled.
- They also will spawn a bit more frequently. Very good chance there is at least 1 on every stage.
- This helps smooth out periods of poor RnG, and also gives radar scanner a use case when Sacrifice is on.

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

### Commando Secondary
- Swapped the cooldowns on Phase Blast and Phase Round.
- (This means phase round has 2s, and phase blast has 3s)
- Significantly closes the dps gap between them.

### Corpsebloom
- Maximum reserved healing increased to 200% (+200% per stack) from 100% (+0% per stack).
- Base maximum healing per second increased to 15% from 10%.
- Maximum reserved healing is now calculated from: (Max Health + 25% of Max Shield) instead of just Max Health.
- Maximum healing per second is now calculated from: (Max Health + 25% of Max Shield) instead of just Max Health.

### Oneshot Protection
- Now only applies to your health. Both shields and barrier are simply subtracted from incoming damage.
- Hits for more than 211% of your maximum HP now bypass oneshot protection.
- This effectively resolves glass stacking for immortality.
- This also means that shield generators no longer can cause weird situations with OSP.

### Gesture of the Drowned
- On equipment use you have a 2.5% chance per stack for your equipment to break.
- Cooldown reduction increased to 50 + 50% instead of 50% + 15%.
- The break chance is non-linear. Mathematically it works out to each stack halving the average number of uses before break.
- Example: one gesture = 40 uses on average. 2 gestures = 20 uses. 3 = 10 uses.
- This effectively turns equipment into consumable items.
- In addition, this change opens up numerous options for me to add entirely new equipment that would be overpowered with the vanilla version of gesture.

### Blight (Acrid alternative passive)
- Blight is now applied by all of acrids attacks including Primary.
- Attacks that already applied blight now apply 3 stacks instead.
- Blight damage reduced by 30%.
- This change is intended to offer a reason to go melee range on Acrid when you take Blight.
- Only applies to Blight because poison is already plenty good overall, and caters more specifically to the ranged kiting playstyle anyway.
- This makes melee Blight Acrid into a significant DPS powerhouse, which is fitting for his lack of defensive tools relative to other melee survivors.

### Focused Convergence
- Cap increased from 3 stacks to 10 stacks.
- Teleporter radius is now multiplied by 0.75 per stack. (Exponential)
- Charge rate is now divided by 0.75 per stack. (Exponential)
- For reference. At 7 stacks the TP zone is the size of the teleporter itself. At 7 stacks the teleporter also will charge to full in roughly 12 seconds.
- Generally just gives you a reason to pick up the item.

### Death Mark
- Now activates at 35 debuffs.
- Each stack of a debuff is counted seperately.
- Debuffs that cannot stack count as 10 debuffs.
- This change is aimed at making Death Mark more accessible without needing hyper specific combinations of items.
- At the same time, it also is aimed at making it more difficult to apply death mark to large numbers of enemies at once (because you need multiple stacks of some debuffs)

### WillOWisp
- Damage increased to 400% + 100% per stack.
- Base radius increased to 15.
- Radius no longer scales with stacks.
- Let's be real, we all know that this item was busted...


## Changelog
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
