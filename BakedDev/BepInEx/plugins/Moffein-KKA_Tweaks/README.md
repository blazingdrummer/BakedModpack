Adds extra config options to KingKombatArena.

## New Config Options:

- Weaker Stuns (Default: True)
	- Players can attack during stuns.
- Disable Chain Stuns (Default: True)
	- Prevents players from being re-stunned if they're already stunned like vanilla enemies (requires Weaker Stuns).
- Disable I-Frames (Default: True)
	- I-Frames give armor instead of invulnerability during duels.
- I-Frame Armor (Default: 200)
	- Armor to give if I-Frames are disabled.
- Captain: Disable Defensive Microbots (Default: True)
	- Disables Defensive Microbots during duels.
- Damage Multiplier (Default: 1)
	- Multiplies player damage by this amount during duels.

## Installation

Place KingKombatArena_Tweaks.dll in /Risk of Rain 2/BepInEx/plugins/

## Changelog

`1.0.2`

- SotV update. Removed Heal Multiplier fix since I'm assuming that it's been fixed in KKA by now.
	- Noticing an issue with RecalculateStatsAPI's ModifyShieldStat hook. This might be an incompatibility with KingKombatArena itself? No clue. Modded shield items might not work.

`1.0.1`

- Fixed config not working?

`1.0.0`

- Release