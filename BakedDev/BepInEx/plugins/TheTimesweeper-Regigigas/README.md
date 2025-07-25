# Regigigas
- Adds Regigigas, a powerful new boss that spawns on Siren's Call, Sundered Grove, and post-loop Titanic Plains, Abandoned Aqueduct, Wetland Aspect and Rallypoint Delta
- Includes a somewhat balanced and playable version in config, disabled by default
- Fully multiplayer compatible!

[![](https://cdn.discordapp.com/attachments/469291841859092488/817547733132640326/unknown.png)]()

[![](https://cdn.discordapp.com/attachments/469291841859092488/817549094712901662/unknown.png)]()

[![](https://cdn.discordapp.com/attachments/469291841859092488/817550601503113238/texRegigigasIcon.png)]()

## Lore Friendly Skin

[![](https://cdn.discordapp.com/attachments/978884006785449996/1134046599606177852/image.png)]()

Now includes a custom skin + name that better fits into the Risk of Rain world, for those who don't want to break their immersion but still want to fight this boss!
This does have to be enabled in config, otherwise you get the normal Regigigas experience.


Note: This model was sloppily hacked together with Stone Golem parts, if any artist is interested in making a proper model for him feel free to contact me on Discord under @braindead_ape

## Skills

### Slow Start

For the first 2 minutes after spawning, `attack speed`, `damage` and `movement speed` are halved. `Armor` is doubled during this time.

For the playable version, this is changed to a 10 kill requirement, scaling down with stage count.


### Crush Grip

Grab a nearby enemy and crush them, dealing 50% of their max health, then throw them.


### Earth Power

Stomp with all your might, summoning pillars of flame that deal 600% damage. Inflicts burn.
    
### Revenge (usable below 50% hp)

Freeze up for 8 seconds, gaining 500 armor. At the end, release a massive blast for triple the damage receieved during this time. Radius scales up with damage taken, up to a limit.

## TODO
- Ancient Scepter support
- Void item displays

## Credits
YinDragon - [Skill icons](https://www.deviantart.com/yindragon/art/Pixelmon-External-Move-Icons-530204137)

## Known Issues
- Missing item displays for SOTV items

## Changelog

`1.4.10`
Thanks Moffein for this update
- Disabled Earth Power afterburn, added config to restore it
- Added config to remove Regigigas from the spawn pool for Artifact of Origination from Moffein's Risky_Artifacts

`1.4.9`
- Separated lore friendly configs for playable and boss versions, so you can have the boss as Stone Juggernaut and the player as Regigigas if you'd like (thanks Moffein for the suggestion)

`1.4.8`
- oops

`1.4.7`
- Added a config option to nerf the boss version's melee by making it punch instead of grab
- Adjusted the order of skills in the loadout so the default loadout isn't completely terrible
- Ancient Power damage per rock: 500% > 300%, max stock 8 > 5, cooldown 4s > 5s
- Heavy Slam minimum damage: 1400% > 800%
- Giga Impact damage: 1600% > 1200%
- Earth Power damage per wave: 600% > 400%
- ^^^overall damage was way too high after new Heavy Slam and Giga Impact
- Added skill: Ice Punch
- Added skill: Mach Punch- both these skills are kinda joke tier
- Added missing skin icons
- Tweaked Heavy Slam logic- less movespeed scaling, faster falling, less likely to hit the skybox with no items
- Updated Ancient Power skill icon
- Finished most of the missing item displays
- Added skin: King (sorry)
- Fixed hitstop not working on punches
- Fixed items falling through the floor when dropped via item drop mods
- Regirock skin now plays the proper Regirock cry

`1.4.6`
- Giga Impact renamed to Heavy Slam, damage changed to a scaling value based on speed, fall speed greatly increased
- Added new special: Giga Impact- charge up, then rush forward and explode in a burst of flames
- ^should provide some much needed flexibility as well as the ability to get through certain tight spaces
- Added character select animation
- Updated even more VFX and SFX
- Updated skill icons

`1.4.5`
- Added Slow Start icon
- Added new buff icons
- Ancient Power rocks now fly in a straight line ignoring gravity
- Ancient Power damage per rock: 400% > 500%, damage output wasn't rewarding enough to justify the risk
- Ancient Power crosshair updated
- Increased radius of Revenge- this thing was not threatening at all as a boss move with its short range
- Sped up jump animation outside of Slow Start even more
- Updated and cleaned up almost all VFX, adding lots more where it was missing
- Fixed Slow Start's text popups appearing multiple times in multiplayer

`1.4.4`
- Added compatibility for the Artifact of Origination from Moffein's Risky_Artifacts
- Added a text popup for Slow Start and its activation
- Base movement speed: 6 > 8 (this is still halved during Slow Start)
- Slow Start is now nullified in certain stages because fighting Voidling with it and traversing the Moon was just awful (lore reason: lower gravity or smth idk)
- Fixed an issue preventing player Regigigas from using certain interactables

`1.4.3`
 - fixed stone juggernaut disappearing

`1.4.2`
Thanks again to rob himself
- Fixed non-host players getting stuck when grabbed
- Fixed grab not working for non-host players
- Added a new alt skin for the lore friendly version, as well as a new character icon
- Added some missing hit feedback to Crush Grip
- Added tons of new SFX to everything
- Added more item displays :-)
- Slow Start's kill requirement now scales down with stage, all the way down to 0!
- Greatly reduced jump windup frames after Slow Start is deactivated
- Pressing sprint during Drain Punch will now buffer and enter a sprint when the attack is finished
- Ancient Power now has a visual display of how many rocks are ready to be fired
- Ancient Power no longer has extreme vertical knockback knocking enemies out of the attack
- Improved Ancient Power's aim mode
- Reduced size of playable version in character select and rewrote some flavor text
- Fixed oversight causing the AI to use Giga Impact instead of Revenge, oops!
- Fixed Hopoo Feathers doing nothing
- Fixed lore friendly logbook model
- Fixed networking on emission glow during certain moves

`1.4.1`
 - fixed conflict with Deputy relating to buffs being applied

`1.4.0`
Thanks to rob for visiting
- Added a new `Lore Friendly` config option, gives the boss an alternate name and skin to help it fit into the world a little better. This is off by default
- Nerfed Earth Power to only fire 5 waves; the original implementation didn't account for anything beyond a single teleporter boss, which was a mistake (old version can be restored via config)
- Players can now cancel Revenge early by reactivating the skill
- Revenge moved to Special slot
- Giga Impact moved to Utility slot and completely reworked into a leap with an explosive landing
- Fixed Hopoo Feathers not doing anything
- Fixed buff icons
- Fixed Slow Start not being applied to player Regi after the first stage
- Fixed enemy Regigigas spawned on stage load not having their Slow Start debuff
- Did a lot of minor code optimization that should help performance a bit

`1.3.3`
- remembered recalculatestatsapi submodule after I uploaded wops

`1.3.2`
- fixed mastery achievement for you shiny hunters
- attempt to optimize drain punch's two getcomponents
- regigigas is now immune to slows because he is made of the elements or something like that
- moved some buff stuff to recalculatestatsapi

`1.3.1`
- added weakpoint
- tweaked sounds

`1.3.0`
- updated for sotv. see known issues above
- made spawning animation for player regigigas only happen on the first stage (like acrid)
- fixed skill selection not being remembered
- fixed wife nagging about him not being fixed yet

`1.2.2`
- Revenge armor buff now lasts until the attack actually goes off
- Fixed weird Slow Start behavior in multiplayer

`1.2.1`
- Slow Start is now a stacked debuff that goes down as you score kills
- Fixed Slow Start not working in multiplayer

`1.2.0`
- Slow Start for playable Regigigas reworked- now visualized as a debuff, and is removed after getting 10 kills
- Now drops Pearls as its boss item
- Regigigas now has a 1/8192 chance to spawn as a Shiny and drop a guaranteed Irradiant Pearl on death- chance is configurable
- Base armor 40 > 20
- Revenge base radius increased
- Revenge base duration decreased
- Revenge damage return 200% > 300%
- Revenge postprocessing duration changed to match the channel duration
- Ancient Power projectile speed increased
- Reimplemented mastery skin achievement
- Added a few more item displays
- Fixed Giga Impact secondary explosion not doing damage
- Fixed a bug causing players to get stuck forever if they killed Regigigas while they were grabbed

`1.1.1`
- Fixed for latest RoR2 update
- Updated camera stuff, Ancient Power now has a crosshair

`1.1.0`
- Slow Start now doubles armor for the duration
- Slow Start duration now scales down with level
- Slow start now has a slight visual indicator when activated
- Earth Power damage 1200% > 600%- now inflicts burn
- Added new primary: Drain Punch
- Added new experimental secondary: Ancient Power
- Added new experimental special: Giga Impact
- Added placeholder skill icons
- Added area indicator for Revenge's radius
- Revenge channel duration no longer scales with attack speed
- Rebalanced base stats for survivor variant
- Increased spawn weight in Sundered Grove to 2
- Base armor 0 > 20
- Fixed item displays
- Fixed idle animation not looping after Slow Start had activated
- Fixed aim animation being slightly off-center
- Fixed Wax Quails not applying to jump
- Fixed buggy jump animation
- Fixed glow bugging out with multiple Regis on the map

`1.0.5`
- Fixed to work on latest RoR2 version
- Fixed a bug causing players to get stuck forever if they killed Regigigas during a grab
- Increased Revenge radius

`1.0.4`
- Fixed a bug causing Regigigas to never actually spawn as a boss

`1.0.3`
- Base health 2100 > 4200
- Base health per level 630 > 1260
- Base armor 20 > 0
- Added Mastery skin
- Added a different set of animations for when Slow Start is finished
- Added death animation
- Added alt primary: Brick Break
- Added some new sounds
- Added new Earth Power visuals
- Earth Power projectile count 5 > 14
- Earth Power damage 900% > 1200%, no longer rotates or applies Cripple
- Fixed oversized particles

`1.0.2`
- Fixed playable Regigigas always being enabled

`1.0.1`
- Fixed some networking issues
- Moved up aim origin so projectiles don't come from his crotch
- Crosshair is no longer hidden when Visions of Heresy is held
- Added item display for Visions of Heresy

`1.0.0`
- Initial Release