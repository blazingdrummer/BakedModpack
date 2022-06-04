Information:
Adds a playable Void Reaver into Risk of Rain 2. 

 - Primary fires 3 shots that stick to enemies and explode after a very short duration. Number of shots scaling with Attack Speed.
 - Secondary is derived from the the Void Reaver's only original attack. Its been modified to activate where you're looking, and has been given a shorter timer on explosions.
 - Utility helps Void Reaver avoid getting surrounded and heals a portion of health.
 - Special sacrifices half your health to deal a big burst of damage.

Multiplayer:
All players need the mod installed!
Let me know if there's any strange interactions!

-----

Known Bugs:
 - Performing no movement while using Utility sends you off in an odd direction.
 - Config file is broken for now, sorry!
 - When getting frozen, Void Reaver's feet fly up. This is a vanilla game bug.
 - Textures are flipped and off-screen in loadout tab.

(Please let me know if you find anything else!)

-----

Ver 0.0.1
 - First Release

Ver 0.0.2
 - Secondary now will summon bombs at the spot you're looking instead of in an area in front of you. With the added control, bomb number has been reduced and the area has been shrunk down.
 - Utility should now make you impossible to hit even when you're not the host
 - Scaled up Void Reaver's size a bit, let me know if this causes any issues but I didn't run into any while playtesting!
 - Reave now will leave you at 1HP rather than killing you when below 50% health
 - Added more detailed (and and colorful!) stats about each skill
 - Added a display model to the selection screen
 - General bug and stat fixes

Ver 0.1.0/0.1.1
 - Updated for the Artifacts update!
 - Added skill icons.
 - Removed debug messages (oops!).

Ver 0.2.0
 - Major quality update
 - Reticle changed so that there's a dot in the center (Helpful for pinging)
 - Secondary now has Proc Coefficient! Apparently proc coefficient is still broken for enemy Reavers...
 - Utility has been completely redone. Now is 100% identical to the item and works on clients!
 - Special got a bit wonkey with the latest update so I went over it and found I did a lot of things wrong, so I worked on effects and networking and fixed the health values so it should now function as intended!
 - Alt Special (Client Reave) is GONE!! Now Reave works on both host and client!!
 - I learned quite a bit since I last worked on Void Reaver and I made plenty of mistakes back then, so I took some time to really fix it up and give it some polish...!

Ver 0.2.1
 - Forgot to set immunity to executes! (Such as being frozen)
 - M2 now has an area indicator so you know where it'll fire!
 - Fixed the mod icon's outline to be the correct color.
 - Death animation now instantly explodes to differentiate it between the Reave ability.

Ver 0.2.2
 - Removed hitstun all together instead of making it "only if 100% health damage taken" due to a bug in Transcendence (Enemies who pick up this item should have issues in the vanilla game if I'm understanding correctly?)
 - Made Void Reaver's Collision Cylinder slightly smaller so they can fit in the legendary chest cave (Size and hitboxes should still be the same size)
 - Slightly altered how the M2 works. If no ground is nearby, it will spawn in the general area of the indicator.

Ver 0.2.3/0.2.4
 - Updated compatibility for Risk of Rain 1.0 update!

Ver 0.3.0
 - Currently testing increased armor during Void Reaver's special, let me know how it feels during runs!
 - Reave also takes away from 50% of your current HP, I may change the scaling of the damage too in the future depending on how much health you have...?

Ver 0.3.1/0.3.2
 - (Check Lunar Chimera Mod)

Ver 0.3.3
 - Split Void Reaver and Lunar Chimera into two seperate mods!

Ver 0.3.4/0.3.5
 - Skin support/bugfix!
 - 4 new custom skins!

Ver 0.3.6
 - Fixed a skin error that caused issues with all summonable allies (drones, beetle guards, etc)
 - Removed RyanSkinAPI hard dependency. You must download the mod seperately to get the skins to work.
 - Reduced recoil on alternate primary skill.

Ver 0.3.7/0.3.8
 - Forgot to register Ravenous Sweep, now should work online... Had no idea it was a quick fix!
 - Enemy void reavers now properly explode if the player had previously died, I thought I fixed this...

Ver 0.4.0/0.4.2
 - Quality of Life update!
 - Added configuration for stats, skills, and lunar item skill scaling. Even though I feel Void Reaver sits in a good spot balance-wise, people are doing lots of wild packs with specific needs and there's no real reason for me to lock Void Reaver as-is. I'll try to add this to my other mods in the near future!
 - Fixed some formatting errors. Delete the config file to fix!
 - Added a temporary scale config value, use at your own risk!

Ver 0.5.0/0.5.1
 - Very early update for EnigmaticThunder support.
 - Currently void reaver WILL kill all entities even as a player so watch out!
 - Gives you Strides of Heresy until I can fix the utility skill.
 - Adds Void Reaver at the very start of the list...?
 - Probably other bugs!!

Ver 0.5.2/0.5.3
 - And now after all that work, ported back to R2API...!

Ver 0.6.0
 - Total rewrite of the mod
 - Modular for quick fixes across all my mods
 - Modified attacks to be different from Heretic

Ver 0.6.1/0.6.2
 - Major bugfixes.
 - All skills should behave as intended??

Ver 0.6.3/0.6.4
 - Client bugfixes
 - All projectiles now have a fixed timer to prevent issues
 - Utility now has invisibility and healing over time applied
 - Fixed interaction range

Ver 0.6.5
 - Fixed a typo that caused the secondary projectile not to be registered.

Ver 0.6.6
 - Recreated an old alternate Primary.
 - Secondary now scales with attack speed.
 - Modified the Utility skill to absorb your vertical momentum.
 - Special now deals damage over time throughout the move. You are also immobile and invincible during this time. No longer scales with attack speed due to some bugs.

Ver 0.6.7
 - Config file reimplemented!
 - Configs added for the two new primary skills.
 - The broken loadout menu is FINALLY fixed!!!

Ver 0.6.8
 - Many camera override fixes (could have caused major camera issues under certain circumstances).
 - Fixed accidently overriding the duration of strides of heresy to 1.5 seconds.