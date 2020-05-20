This mod adds:
A totally new survivor built entirely from scratch. Only reused one of hopoos meshes.

A new boss enemy that spawns late game (stage 8ish). Currently early in development and feedback is greatly appreciated. 

Note that in order to use this mod in multiplayer, everyone must have this mod installed and be on the same version. It takes the same networking approach as the vanilla game, meaning it assumes that every client has the same, or nearly the same, internal setup in order to greatly reduce the amount of network traffic. 

## Feedback
- I am extremely open to any kind of feedback, question, suggestion, bug report, or really anything.
- I have a simple discord set up to help keep bug reports and feedback organized for all my mods, feel free to join and all that.
- https://discord.gg/TgaDGNh
- I also will sometimes release beta versions of my mods ahead of time there in order to get feedback.
- You can also DM me on discord if that is easier. (@Rein#7551)

## Showcase video

[![Showcase video](https://img.youtube.com/vi/zCdGD_zaQKA/0.jpg)](https://youtu.be/zCdGD_zaQKA)


### Install
- Delete old versions. (You never know)
- Unzip the plugin zip.
- Copy all files to the plugins folder in Bepinex(in your game install directory)
- Bonus points if you create a separate folder inside the plugins folder for every mod

### Uninstall
- Delete the files that come with the mod from the plugins folder (Just RogueWisp.dll)


## New this update
### Minor patch 2.1.5
- Performance improvements across the board. Primarily for the boss.
- Added config for a low performance mode for the boss. This reduces the visual quality. Generally this should not be needed for the vast majority of people.
- Boss director cost increased to 4000 from 2000
- Adjusted boss base stats accordingly
- Adjusted minimum stage to account for addition of stage 5


## Testimonials
- "Thats kinda hot" -Violet Chaolan

## Character Information

### Lore
- Yeah... Maybe some day.

### Base Stats
- 110 ( +33 ) health.
- 12 (+2.4) damage.
- 1.0 ( + 0.2 ) health regen.
- All stats are identical to Commando.

### Skills
- Descriptions for the skills and passive can be found in game. Feel free to ask me if you have any questions.

### Playstyle
- Rogue Wisp is a short ranged, immobile, high-damage caster.
- They have an additional resource to manage called Flame Charge which is gained from primary, and from being within range of Utility while enemies are burning.
- Flame Charge increases the potency of abilities, but falls off over time if it is over a certain threshold.
- Flame Charge is visible as a UI element next to the crosshair. As it increases the bar goes from black (0) to white to red to green to blue to orange to teal to purple and then repeats (although it is exceptionally rare to increase it that high)
- All skills except primary consume Flame Charge on use.

### General tips for playing them
- You want to have your utility down as often as possible, and you also want to be inside with as many enemies as possible.
- Doing this will dramatically increase your damage output, with obvious risks associated.
- Remember that there is no upper limit to your Flame Charge, but the rate of decrease increases with the value. At extremely high charge values your damage can be multiplied by 30, or even more.

## Future plans
- Much of the balancing is still in progress to some degree. Feedback is incredibly helpful here.
- I am always looking to improve performance and fix bugs, so please inform me if you find anything.

### Longer term things
- Another new boss
- New stage
- New item(s?)
- Skill variants
- Improved animations
- A bunch of challenges for unlocking wispy, skill variants, and other content.


## Compatibility information
If you run into any kind of compatibility issues with other mods, let me know on my discord or via DM. I would very much like to avoid as many of these as I can.

With that being said, due to the scope of this mod I end up hooking and touching a very large portion of the game code. Because of this, there will be compatibility issues. In addition, not all issues can be resolved solely on my end. Sometimes it will require changes to the other mods as well.

As a general note: if your mod is working in an area where it may end up working with the wispy gameobject, make sure to air on safe side with null checks (which you should be doing anyway). Some of the character's structure is a bit unothodox from vanilla survivors, particularly around the model and skins area to accomodate my custom skin system, and allowing for the skinning of projectiles and other effects.

Also note that this mod does overwrite a few of the hooks in r2api to clean up their functionality. None of these hooks will cause behaviour any different from standard r2api, but they may log a warning for some networking issues that r2api isn't set up to detect, such as skills that are not registered fully (LoadoutAPI.AddSkill(typeof(YourStateHere)), before you call new SerializableEntityStateType)

To make things easier, I've listed all the methods I hook below.
### On hooks
- RoR2.CameraRigController.Start
- RoR2.CharacterBody.Start
- RoR2.CharacterBody.FixedUpdate
- RoR2.CharacterBody.RecalculateStats
- RoR2.CharacterSpawnCard.Awake
- RoR2.Projectile.ProjectileController.Start
- RoR2.UI.CharacterSelectController.Awake


### IL hooks
- RoR2.CharacterBody.RecalculateStats
- RoR2.UI.CrosshairManager.UpdateCrosshair
- RoR2.CameraRigController.Update
- RoR2.SetStateOnHurt.OnTakeDamageServer
- RoR2.GlobalEventManager.OnHitEnemy
- RoR2.CharacterModel.UpdateRendererMaterials
- RoR2.EffectManager.SpawnEffect void(EffectIndex EffectData Boolean)
- RoR2.Projectile.ProjectileImpactExplosion.FixedUpdate
- RoR2.UI.LoadoutPanelController.Rebuild
- RoR2.UI.CharacterSelectController.RebuildLocal
- RoR2.UI.CharacterSelectController.OnNetworkUserLoadoutChanged



## Changelog
### 2.1.4
- Moved death mark changes over to GeneralFixes (another mod)
- Wispy now interacts properly with Vengeance Artifact. (You have no clue how much work this was... I needed to extend the base game's AI system to support resource management and positioning logic)
- Adjusted visuals on many effects. Should be less bright, but also more visible for the darker skins.
- Adjusted visuals for burn effect. No longer makes entire enemy glow brightly.
- Barrier gain early on increased significantly, but it does scale up a bit less later on.
- Removed april fools skill names.
- Improved names of skills.

### 2.1.3
- Adjusted death mark stuff and added an option to disable all of it (except for the part that makes it detect modded buffs too)
- If disabled vanilla behaviour. if enabled, it requires 30 points to activate. 10 points per non-stacking debuff. 1 point per stack of stacking debuff.

### 2.1.2
- Fixed boss AI breaking while it switches to second phase.
- Death Mark now works with custom debuffs, rather than just the vanilla ones.
- Death Mark also counts multiple stacks of a debuff, but requires 6 debuffs to apply its effect instead of 4. (Basicaly this makes it more consistent earlier, and less consistent later. Reasoning for this is that it was basically a "Get 1 chrono, some tri tips, ect. and it is always up. Now it leans in towards focusing on a single enemy to stack it, but it doesn't depend on specific combinations of items to do so.)
- Reduced wispy base health to 110 from 130 (The recent patch made the game overall much more wispy friendly. Many items and artifacts play in to the type of gameplay wispy revolves around, so this is needed to keep things under control)
- Barrier gain from passive is now based on combined HP instead of max HP, meaning it takes shields into account. (The health vs shield distinction was kinda arbitrary and it is a good way to help compensate for the above nerf)
- Improved some ability names.

### 2.1.1
- Fixed Ancient Wisp visuals
- Hit detection should now work correctly with chaos artifact
- Added new enemies to the table of charge values
- Some minor optimizations.

### 2.1.0
- Compatible with latest RoR2 update. (Remove r2api if there are issues. This mod does not use r2api)

### 2.0.8
- Resolved same issue with minirpc...

### 2.0.7
- New showcase video.
- Charge gain from primary now occurs over a longer duration for the same amount (this is a good thing, charge decays slower while it is increasing)
- Adjusted barrier gain.
- Secondary multiple hit multiplier reduced to 35% from 50%.
- Secondary radius adjusted to match visuals.
- Hopefully improved some animation transitions with secondary cast.
- Special charge scaler increased to 85% from 80% (so just a tiny bit more damage based on charge)
- Boss health reduced to 6800 from 8000 (They were just a bit too tanky)
- Adjusted Glow Cracks option in skin selection.
- Custom color preview for skin selection now works properly.
- Initial skin settings now are applied to the model properly.
- Rewrote UV map generation code, it is now multithreaded and produces much higher quality results.
- General reorganization of code in preparation for next game update.
- The hook to r2api code now only is applied on older versions of r2api, since the bug it was fixing was solved in most recent update.

### 2.0.6
- Improved compatibility with MiniRPC

### 2.0.5
- Removed unneeded R2API dependency
- Removed config option for the boss spawning. Fairly confident that it is a balanced enough fight now.
- Crosshair charge bars now persist while sprinting.
- Skill bar charge indicator no longer visible on all characters.
- Added config option to hide the skill bar charge indicator.

### 2.0.4
- Switched some portions of code over to run on multiple threads.
- Worked out numerous bugs with new hit detection.
- Tuned texture generation algorithm.
- Removed placeholder display UI for passive.
- Added a new crosshair (that displays charge)
- Also added a bar above skill bar that displays charge.
- New skill icons for primary and special (Thanks to Tera again)


### 2.0.3
- Actually included the updated version of the .dll this time.....
- Also included the version with major performance fixes for hit detection (generally around 10x faster now, will be noticable later in runs)


### 2.0.2
- Resolved some bad behaviour in boss AI when low on health.
- Boss now has invulnerability during the transition between its two phases (It doesn't attack during this time, and it is only for a few seconds)
- Wispy base health increased to 130 (+39)
- Minor adjustment to primary vfx.
- Added 4 more item displays (No I won't tell you which, go find out!)


### 2.0.1
- Fixed compatibility with BepInExConfigurationManager. No, I don't know what was causing it.


### 2.0.0
- Added a new boss. Boss is intended to sit somewhere between Scavanger and Overloading Worm tier. Generally expect them to start showing up around stage 8 on monsoon.
- Added a new skin system that allows you to create your own skins through an in game menu. Fully networked.
- Remade every single material from scratch.
- Remade every single visual effect from scratch.
- Doubled the size of the codebase (over 30k lines at this point)
- Switched passive over to use barrier instead of shield (barrier is mechanically more logical to use here, similar to loader)
- Reduced base health to 90 (+27) from 100 (+30)
- Primary charge gain reduced slightly.
- Primary restores slightly less charge based on attack speed (Attack speed still increases the overall gain per second, just not by quite as much as before)
- Secondary hit detection reworked. Enemies take full damage from the first pillar that hits them, and reduced damage from subsequent pillars.
- Secondary cost increased to 20.
- Special cost per second increased to 20.
- Attack speed now increases the cost proportionally.
- Special charge scaler reduced to 0.8 from 1.
- Special minimum cast time reduced to 0.25 seconds from 1 second.
- Overall charge gain reduced.
- Hitboxes greatly improved.
- Now able to gain charge properly from the lunar scavangers.


### 1.4.1
- Improved compatibility with RTAutosprintEX.
- Forgot to add that I totally remade the teleporter boss HP bar to the patch notes. It now displays barrier and shield properly.
- Very much looking for feedback on the bar. Would you have noticed the change if I didn't mention it? Does the display of shield and barrier make a difference with some bosses?

### 1.4.0
- Primary reworked again. No longer uses a stock system.
- Primary damage decreased to 175%.
- Primary attack base duration decreased to 0.875 seconds.
- Primary VFX improved.
- Hit detection on primary optimized.
- (Primary changes make it into a more flexible charge gathering tool instead of a damage tool)
- Secondary base damage reduced to 125% from 150%.
- Secondary charge consumption reduced to 10% from 15%.
- Secondary charge scaler reduced to 50% from 75%.
- Secondary base cast time reduced to 0.75s from 1.0s.
- Secondary now applies effects like behemoth properly, even when hitting world.
- Hit detection on secondary optimized.
- (Secondary is now less heavy on investment to use, but also slightly lower impact)
- Utility base radius increased to 25 from 20.
- Armor during special increased to 75 from 50.
- Special radius increased to 2 from 1.
- Special charge consumption reduced to 15% from 20%.
- Special charge scaler increased to 100% from 90%.
- Special now applies effects like behemoth properly, even when hitting world.
- Special VFX improved.
- Hit detection on special optimized.
- Camera positioning during special improved.
- Sprint crosshair during special changed to standard crosshair.
- Streamlined networking of special.
- Tweaked particles on model.

### 1.3.5
- Added a warning during load if some parts of R2API aren't detected. It means you need to grab latest version of r2api.
- Should hopefully keep icon creation from erroring and breaking the character as well.

### 1.3.4
- Greatly improved visuals on utility.
- Added skin icons.
- Fixed feeling of slow movement.
- Greatly improved hitboxes.
- You now count as sprinting while firing special beam (For things like rose buckler and little disciple).
- Reduced shield regen rate from charge gain.
- Special armor bonus reduced to 50.
- Proc coef on special beam reduced to 0.8.
- Fixed numerous bugs with hit detection on Primary, Utility, and Special.
- Fixed bug with flame coloring on some skins.

### 1.3.3
- New showcase video
- Rewrote basically the entire mod in order to more easily add future content

### 1.3.2
- Under the hood tweaks
- Now works with dedicated servers

### 1.3.1
- Compatibility with Hidden Realms update.
- Skill icons (Huge thanks to Tera, who made all 4 of them)
- Improved compatibility with mods that hook RecalculateStats

### 1.3.0
- Reworked primary. Now has better range, deals more damage, and pierces enemies, and restores charge per enemy hit.
- Greatly improved hit registration on primary.
- Fixed Special beam giving the wrong damage location (this made numbers appear in weird places and made focus crystal non-usable)
- Reworked shield restoration to be based on maximum HP rather than shield.
- This is a massive nerf to transcendence, but a buff in most other cases, especially early game.
- New showcase video.

### 1.2.6
- Reduced armor while using special to 100.
- Flame charge bar now responds to screen resolution and hud scale.
- Health regen reduced to compensate for shield.
- Tickrate on special reduced from 6 to 5.
- Shield aura color now responds to skin.
- (Context)
- The shield changes were pretty major, wound up making the character a bit too strong.
- Decided that slight reductions to DPS output would be a better solution than reducing the shield.

### 1.2.5
- Reduced base health by 30.
- Gave 30 base shield.
- While regaining Flame Charge you regenerate a small portion of maximum shield per second per stack.
- This is overall a buff to survivability and will hopefully help out throughout runs but especially in the early game.
- Improvements to Blighted skin.
- Started work on elite overlays varying with skin (still in progress)
- Began process of major code restructuring under the hood.

### 1.2.4
- Fixed bug causing Special to not deal damage in multiplayer when you aren't host.
- Removed Iridescent skin and replaced with a fancy new skin. (Plan on finding ways to increase the max number from 8 in the future because there are a lot of cool effects I can add here)
- Some under the hood changes.
- Fixed typo in ability descriptions.
- New showcase video.

### 1.2.3
- Base armor reduced to 0 (Not really needed anymore)
- Armor during special reduced to 150 from 200 (Still extremely high)
- Stun grenade now scales chance and duration with proc coef (it does not in the base game)
- This was done to keep Utility from permastunning enemies with a single stun grenade.
- Re-tuned charge gain to take the class of the enemy (boss vs miniboss vs basic) and the elite tier into account.
- Generally tuned down overall charge gain to compensate for this.
- Special has a 25% larger radius.
- Utility has significantly nicer visuals now.
- Special now zooms camera in to help with piercing targets at close range.
- Ability descriptions improved.
- Character portrait.
- Icons for all skills (Primary, Utility, and Special are placeholder icons)
- Fixed weird textures in logbook display.
- Very likely some under the hood changes I am forgetting at the moment.

### 1.2.2
- Insert explitives about video here...

### 1.2.1
- Updated showcase video... Again...
- Fixed minor typo in ability description.

### 1.2.0
- Updated showcase video.
- Completely reworked special into a laser type attack that prevents movement but gives armor and deals heavy damage.
- For anyone who liked cremation, It will likely return as a variant in the future with some tweaks.
- Primary no longer scales damage with charge.
- Primary charge gain per attack doubled.
- Primary has some tweaked animations, hopefully feels more smooth.
- Fixed a bug causing small enemies to give more charge than expected on death.
- Removed the Ascendent skin and replaced it with Abyssal which is red and stuff.
- Compatibility with R2API and Bepinex updates (I hope, let me know if something conflicts)
- Super fancy beam particle effects for the laser.
- Very likely some minor things that I have forgotten... Ugh.

### 1.1.3
- You now gain 25% extra movespeed while within the range of Utility.
- Ability descriptions made even more clear.
- Item pickups now display on the character model (not all are positioned very well, but that will improve over time)
- Custom skin for the survivorpod.
- Charge UI now hides while game is paused.
- Sprint animation slightly improved (Just a temp fix until I can get all movement animations looking good)
- Fixed an animation transition bug from sprinting to standing still.

### 1.1.2
- Utility cooldown reduced by 0.00001 seconds. It is important, I promise.
- Fixed Special damage scaling once again... I'm roughly 46% certain the skill is cursed at this point.
- Special projectile now travels significantly faster.
- Special projectile now has a slightly smaller collider (hopefully will keep it from hitting the floor on fire at some angles?)
- Tuned the rate that Flame Charge is transferred from Utility to you.
- UV mapped the model (from script, please send help)
- Created a fancy custom material for the armor (It is animated!)
- Re-Scaled the character to not be like double the height of all other survivors... (They are now ~the same height as loader)
- Adjusted camera positioning and hitbox size to go along with the scaling.
- Particle effects on body fit to the shape a bit better.
- Added better visuals for aiming Utility.
- Made the in game ability descriptions more clear (I hope)
- Most likely other stuff I forgot... ugh.

### 1.1.1
- Base armor up to 10.
- Further reworked Utility.
- It now stacks Flame Charge inside it damages enemies, and as those enemies die.
- That flame charge is transferred to you over time as a buff while you are within the radius of Utility.
- In addition, damage ticks twice as often and also has a 0.05 proc coef while you are within the radius.
- Radius scales with flame charge.
- The above further reinforces the close range playstyle intended for this character.

### 1.1.0
- Fixed all known multiplayer issues (if you find more, tell me)
- Added two new buff types (one is the flame debuff on enemies, the other is a flame regeneration buff on you)
- Totally reworked Utility mechanics. Now creates one larger zone and applies stacks at an increased rate.
- The method of gaining Flame Charge from utility now operates through a buff and is overall easier early game and harder late game.
- Fixed bugs with ability damage scaling with flame charge. Bug was causing them to be much weaker than intended.
- Primary and Special totally rewritten with very similar functionality.
- New sounds for primary.
- All charge consumption is now percent based instead of flat. Abilities scale based on the amount of charge consumed.
- Special and passive both greatly buffed to have less trash names.
- Base damage reduced to 12 from 15 (because it was making equipment way too strong)
- Primary increased to 300% base damage.
- Range on primary increased to 40
- Primary cooldown increased to 2.5 seconds
- Secondary outer radius increased to 8, inner radius is now half the outer radius.
- Secondary damage reduced to 150% from 200% (The increased radius means you hit more times per enemy per wave, this is a buff against most enemies)
- Special increased to 437.5% - 1750% base damage.
- Special no longer slows at all and instead just prevents sprinting. This is overall very close to neutral, but feels better in game.
- Base armor increased to 5 (just a small nudge for survivability particularly early game)
- Ability descriptions updated...

### 1.0.3
- Even further primary cleanup
- Fixed compatibility issue with AutoItemPickup
- Reduced movespeed penalty while charging Special
- Camera position adjustments (Will include config for this setting in the future)
- Fixed a bug where flames didn't tick after spreading a certain number of times.
- Fixed a bug that prevented you from being frozen
- Validated that save file issues from skins are no longer occuring

### 1.0.2
- Further cleanup of primary behaviour
- Reduced time to charge special by 40%
- Actually updated the descriptions too this time!

### 1.0.1
- Added a Character Select display
- Tuned cooldowns and damage across the board to get damage output in line with other survivors
- Cleaned up primary behaviour to be more consistent
- Reduced radius on Special explosion, it was excessively large (may still be a bit too large, we'll see)
- In compensation for the damage changes (overall output is significantly higher than original) range on Primary and Utility are reduced.

### 1.0.0
- First release
