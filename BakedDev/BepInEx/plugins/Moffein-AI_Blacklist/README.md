Lets you blacklist items from Monsters, Vengeance Doppelgangers, Scavengers, and Mithrix.

Vanilla blacklists can be disabled in the config.
Unstable Tesla Coil, N'kuhana's Opinion, and Razor Wire are blacklisted by default in the config.

Default Blacklist:

- Frost Relic
- Unstable Tesla Coil
- N'kuhana's Opinion
- Razor Wire
- Regenerating Scrap
- Shipping Request Form
- Spare Drone Parts
- Ben's Raincoat
- Shuriken

To blacklist items, enter the internal item names separated by commas into the config.

You can view a list of item/equipment codenames using the list_item/list_equipment command from [DebugToolKit](https://thunderstore.io/package/IHarbHD/DebugToolkit/).

Server-Side and Vanilla-Compatible, only the host needs the mod.


## Installation

Place AI_Blacklist.dll in /Risk of Rain 2/BepInEx/plugins/

Config can be found in /Risk of Rain 2/BepInEx/config/com.Moffein.AI_Blacklist.cfg

## Changelog

`1.5.3`

- Removed dead links to the modding wiki.

`1.5.2`

- Internal changes related to ItemTags.
	- Now properly adds/removes the items from the game's internal itemIndicesByTag array, since certain in-game functions refer to that instead of checking the actual tags on items.
	
	*Let me know if this causes any errors.*

`1.5.1`

- Vengeance code is less intrusive.
	- Hooks CharacterMaster.Start instead of OnInventoryChanged now.

`1.5.0`

- Vengeance Leveling
	- Now uses Player Team level instead of Ambient level.

`1.4.5`

- Added Frost Relic to the default blacklist.

`1.4.4`

- Fixed Vengeance blacklist not working (DLC update broke previous method).

`1.4.3`
- Added Shuriken to default blacklist.
	- If you are updating from a previous version, you will manually need to add PrimarySkillShuriken to the list.

`1.4.2`

- Hopefully fixed Vanilla compatibility issues.

`1.4.1`

- Added Ben's Raincoat to the default blacklist.

`1.4.0`

- Updated for DLC update.
- Removed R2API dependency.
- Disabled Elite Equipment Replacement since it was buggy.
- Added Regenerating Scrap, Spare Drone Parts, and Shipping Request Form to the default blacklist.

*I haven't been able to do much in-depth testing on this since DebugToolkit isn't fixed yet. If there's any issues or bugs, let me know!*

`1.3.3`

- Fixed a regression in Vengeance code that caused it to be applied to everyone. This should be the last of the issues with Vengeance.

`1.3.2`

- Added back Vengeance Blacklist code that got lost during the plugin restructuring.

`1.3.1`

- Added back Vengeance Leveling code that got lost during the plugin restructuring.

`1.3.0`

- Added option to use a separate blacklist for Scavengers.
- Internally restructured the plugin.
- Merged Mithrix Blacklist into the mod.
- Added config option to disable the Vanilla AI/Mithrix blacklists.

`1.2.1`

- Fixed Vengeance changes applying to everything.

`1.2.0`

- Equipment Blacklist no longer affects friendly allies (Equipment Drones, Goobo)
- Vengeance Clones now properly scale with level (can be disabled).
- Added support for blacklisting items from Vengeance Clones (separate from the AI Item Blacklist).
	- Blacklisting items completely removes them from their inventory, so they won't be able to drop blacklisted items.

`1.1.0`

- Added support for blacklisting equipments. (Code based on Unordinal's AI Blacklister https://github.com/Unordinal/UnosRoR2Mods/tree/master/AIBlacklister)
	- It's possible to blacklist Elite affixes, but this may be buggy.
		- It will attempt to reroll an elite affix that isn't Perfected/Malachite/Celestine.
		- The elite's stat boosts may be different from what's intended (ex. banning Malachites will reroll the elite, but it will keep its original Malachite stat boost).

`1.0.1`

- Accidentally a word in the manifest description.

`1.0.0`

- Release