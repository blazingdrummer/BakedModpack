Various QoL tweaks to make Bandit more fluid to play.
I recommend installing https://thunderstore.io/package/Moffein/BackstabRework/ (not Vanilla-Compatible) to go along with this.

Vanilla-Compatible.
Everything is client-side EXCEPT for Special Grace Period and Hemorrhage Ignores Armor, which is server-side.

Settings can be changed in the config.

- Primaries
	- Shot radius has been increased to match other bullet skills.
	- You can now hold M1 to autofire.
		- Can be swapped between an accurate slow-firing mode and a rapidfire burst mode by using the Scroll Wheel.
- Secondaries
	- Serrated Dagger now lunges while sprinting and has a bigger hitbox.
	- Serrated Shiv now stuns on hit.
	- Hemorrhage ignores positive armor.
- Utility
	- Fixed Cloak sound persisting if you teleport while cloaked.
	- You can now hold down Shift to activate Smokebomb as soon as it finishes its cooldown.
- Specials
	- Only fires once you release the Special button.
	- No longer cancelled by sprinting.
	- Both specials now have a 1.2s grace period to trigger their on-kill effects, so that they work with Elemental Bands.
	
Mod icon taken from a comic by R_Neophyte (https://r-neophyte.tumblr.com/)

## Installation
Place BanditTweaks.dll in /Risk of Rain 2/BepInEx/plugins/

## Changelog

1.7.1

- Hemorrhage now ignore adaptive armor.

1.7.0

- Serrated Shiv (Throwing Knife) now stuns on hit.
- Hemorrhage now ignores positive armor (server-side).

1.6.1

- Added missing NetworkCompatibility tag.

1.6.0

- Updated for DLC update.
- Removed Backstab tweaks. They're now in a separate mod: https://thunderstore.io/package/Moffein/BackstabRework/

1.5.2

- Serrated Dagger now has a minimum duration of 0.3s to prevent the lunge breaking at high attack speeds.

1.5.1

- Mod now does not run if RiskyMod's Bandit changes are enabled, due to heavy incompatibilities with it.

1.5.0

- Equipped Commando Pro.

1.4.4

- Mod compatibility stuff.

1.4.3

- Added a check to prevent the Crit Backstab code from running if Backstab Crit Bonus is set to 1 in the config.

1.4.2

- Internal changes to the Slayer fix. Calculation now occurs before Crit Backstab bonus is calculated.

1.4.1

- Fixed 1.3.0's Crit Backstab change ignoring the Crit Backstab Multiplier config setting.

1.4.0

- Slayer (bonus damage to low hp) now affects procs (it doesn't in vanilla).
	- This will affect Acrid's bite as well.

1.3.0

- Added a fix for Crit Backstabs causing weak attacks to trigger bands. (Can be disabled in config)
	- If the attack is >=400% damage, simply multiply the damage by 1.5x
	- Otherwise, hit a second time for 50% of the initial hit's damage (0.5 proc, no hemmorhaging)
- Renamed Burstfire config options to Spamfire to prevent confusion with Bandit's Burst (Shotgun) skill.
- Reduced default Spamfire fire rate from 0.1s per shot to 0.12s per shot since it more closely matches a normal spamming fire rate.
- Greatly improved Quickdraw code.
- Fixed Bandit's Primaries sometimes being able to hold 5 shots.

1.2.5

- Fixed Burstfire Button config option not working.

1.2.4

- Added Client-Side tag on the Thunderstore page.
- Increased default Special grace period from 0.5s -> 1.0s to make it work better online.

1.2.3

- Burst bullet radius increased 0 -> 0.3
- Blast bullet radius increased 0 -> 0.4

1.2.2

- Fixed Smokebomb multi-hitting online.

1.2.1

- Rewrote Quickdraw code to improve compatibility with custom skills.

1.2.0

- Added config option to assign buttons to swap directly to a specific firemode.
- Smokebomb anim is now enabled on the ground by default like Vanilla. This can be disabled in the config.

1.1.0

- Fixed Disable Autofire config option not working.
- Autofire settings are now disabled when BanditWeaponModes is installed (https://thunderstore.io/package/Vl4dimyr/BanditWeaponModes/).
- Added config option to enable BanditReloaded's Quickdraw feature (disabled by default).
- Added config option to enable BanditReloaded's Special Execute feature (disabled by default).

1.0.2

- Now only depends on MMHook for real.

1.0.1

- Now only depends on MMHook
- Added NetworkCompatibility tags

1.0.0

- Release