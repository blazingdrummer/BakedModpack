`1.2.1`

- Increased default damage multiplier from 3.5 -> 4.0 to match EliteReworks. (Existing config unaffected)

`1.2.0`

- Fixed wrong elite tiers sometimes being selected.
	- Now only selects from Vanilla affixes. Mods can add to the list by adding to `AffixBlightedComponent.tier1EliteDefs` and `AffixBlightedComponent.tier2EliteDefs`.
	
- Gilded and Twisted elites are now disabled by default. (Can be re-enabled in config)

`1.1.10`

- DLC2

`1.1.9`

- Recompiled for Devotion update.
- Chinese translation (Thank MushroomEl!)

`1.1.8`

- Korean translation (Thanks p157157!)

`1.1.6` to `1.1.7`

- Added BR translation (Thanks Kauzok!)

`1.1.5`

- Added Russian translation (Thanks Адский Шкед!)

`1.1.4`

- Affix reroll (active equipment effect) now only works for player-controlled entities.
- Sound now has a 3s cooldown.

`1.1.3`

- Added missing PrefabAPI depdendency.
- Fixed incompatibility with mods that add the affix to the logbook (ex. WolfoQoL).

`1.1.2`

- Fixed T2 elite affix option ignoring EliteDef.isAvailable checks.

`1.1.1`

- Fixed Blighted Elites being able to roll Blighted when enabling T2 elite affixes.

`1.1.0`

- Fixed damage multiplier being set to the Affix drop chance (really low).
- Can now enable T2 elites to be selected in the config. (untested)

`1.0.1`

- Removed unnecessary dependency from manifest.

`1.0.0`

- Release.
	- Thanks to Swuff for giving me permission to use LiT's assets!