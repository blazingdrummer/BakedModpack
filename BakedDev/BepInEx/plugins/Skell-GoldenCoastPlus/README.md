## GoldenCoastPlus
This mod aims to improve Golden Coast and make it more interesting and fun.

## Change list
- Allied Aurelionite is now three times as strong, and its health and damage scales linearly.
- Aurelionite can now drop three new items: Golden Knurl, Titanic Greatsword, and Guardian's Eye.
	- Golden Knurl grants the player +10% max health, +2.4 regen, and +20 armor.
	- Titanic Greatsword is an on-hit proc item that summons Aurelionite's sword when it triggers.
	- Guardian's Eye charges up a laser as you gain gold that fires at all nearby enemies when charged.
![](https://cdn.discordapp.com/attachments/662741163262083095/835753637807652874/Items_Screenshot.PNG)
- The unused Gold Elites now spawn in Golden Coast. They steal gold on hit and drop a lot of gold.

![](https://cdn.discordapp.com/attachments/662741163262083095/835753633680850964/Gold_Elite_Screenshot.PNG)
- Changes to Aurelionite's fight.
	- Only four beacons spawn, and Aurelionite is vulnerable as soon as it spawns.
	- Aurelionite now has 2x more health.
	- Aurelionite now becomes invulnerable and turns the beacons off for every third of its health it loses. There is a grace period of 20 seconds after the beacons are turned back on during which they cannot be turned off again, allowing extra damage during a cycle if your DPS is high enough.
	- Removing Aurelionite's invulnerability by turning the beacons back on will debuff it with 1.5x damage taken for 10 seconds.
	- As the fight progresses, Aurelionite's attacks become more dangerous.
		- In phase 2, it summons more swords for its sword attack, fires more lasers for its laser attack, and fires lasers more often for its rock turret attack.
		- In phase 3, it now summons even more swords for its sword attack, its rock turret fires even more often, and its cooldowns are reduced by 25%.
	- For every phase skipped, all players will get a stack of Aurelionite's Blessing, which increases gold gain by 10%.

## Known Issues
- Coven of Gold's icon and model are identical to His Reassurance. This is because I'm a hack and used them when His Reassurance was unimplemented, but I'll fix them at some point.
- Gold elites aren't actually gold. Their unused shader is black, assumedly because its unfinished. I'll get around to making them actually gold at some point.

## Future Plans
- Make Gold Elites more interesting mechanically and give them a new shader.
- Change the interactables in Golden Coast to make them more interesting.
- Update the function of Guardian's Eye to be a little more interesting.
- Continue tweaking the Aurelionite fight to make it feel more like a real midboss and less like a reskinned Stone Titan.
- Adjust the interactables on Golden Coast.

## Changelog
`0.6.3`
- Okay but this time I actually fixed it

`0.6.2`
- Fixed for the latest update.

`0.6.1`
- Fixed NREs caused by Golden Knurl's implementation.

`0.6.0`
- Updated for Survivors of the Void.
- Now uses RecalculateStatsAPI which should fix any weirdness or incompatibiltiy issues.

`0.5.30`
- I think I actually fixed the Thunderstore formatting this time.

`0.5.3`
- Fixed the names of Gold elites, should now say "Gold <character name>"

`0.5.2`
- Thank you swuff for offering to write lore descriptions for the items in this mod! Finally adding them in 2 months after I got them.
- Fixed an issue where Aurelionite was becoming invincible before its phase transitions.
- Maybe I'll start actually working on this mod again who knows heehoo

`0.5.1`
- Aurelionite will now use its third phase attacks if its first phase change happens when it is at the final third of its health.

`0.5.0`
- Changed the duration of the debuff Aurelionite gets upon its armor being broken to 10 seconds (down from 20).
- Increased Aurelionite's health by 2x.
- Changed Aurelionite's attacks as the phases of its fight progress (see Change List).
- Added a bonus reward for defeating Aurelionite in only 1 or 2 cycles.
- Fixed text color of Golden Knurl's description.
- Reduced Titanic Greatsword's damage from 2000% to 1250%.
- Added config for Aurelionite's fight changes and the items he can drop.

`0.4.2`
- Fixed issues with Golden Knurl's renderer materials (finally).
- Fixed Aurelionite's invincibilty triggering too early.

`0.4.1`
- Fixed the entire game breaking because I forgot to finish my TakeDamage hook.

`0.4.0`
- Reverted the changes to pickup and description text of the last update.
- Only Halcyon Seed contributes to allied Aurelionite's strength, like before, but it is still three times as powerful.
- Reworked Aurelionite's fight (see Change List).

`0.3.3`
- Updated pickup and description text of the items.

`0.3.2`
- All items that Aurelionite can drop now contribute to its allied version's strength. Only Halcyon Seed is removed from the player's inventory, and it now contributes 3 times as much to its strength.
- Updated icons for Golden Knurl and the Gold elite buff.

`0.3.1`
- Updated icon outlines (thanks to swuff for the icons themselves and rob for hooking me up).

`0.3.0`
- All items now have proper icons (thanks to Lamda Male) and item displays.
- Gold Elites now drop 5x the amount of gold that they did before, and have a proper buff icon (thanks to Lambda Male).
- Fixed issues with Coven of Gold's name tokens.
- Fixed issue with Golden Knurl not granting regen.
- Fixed issue with Aurelionite being unable to drop Halcyon Seed.
- Fixed plugin name.

`0.2.2`
- Fixed incompatibility issues with Aetherium.

`0.2.1`
- Golden Knurl now gives a 10% health increase rather than a flat 60.

`0.2.0`
- Gave the Gold Elites their unused skin.
- Updated Titanic Greatsword's model.
- Added Guardian's Eye.

`0.1.1`
- Fixed for RoR2 v1.1.1.2.

`0.1.0`
- Initial Unfinished Release

## Credits
- Lambda Male and swuff for the icons for the items and the Gold elite buff.