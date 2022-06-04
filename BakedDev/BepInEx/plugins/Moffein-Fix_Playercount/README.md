Fixes disconnected players counting towards run scaling.
To be specific, this mod prevents disconnected players from counting towards:

- Run difficulty scaling.
- Monster spawn scaling.
- Stage interactable spawns.
- Teleporter/Void Cell drops.

Server-Side and Vanilla-Compatible, only the host needs the mod.


## Installation

Place FixPlayercount.dll in /Risk of Rain 2/BepInEx/plugins/

## Changelog

1.2.2

- Updated libraries. Probably will have no effect on the mod itself, but updating to be safe.

1.2.1

- Fixed an issue where the mod would break when playing with ZetArtifacts with the Multitudes artifact disabled.

1.2.0

- Updated for DLC update.
- Added config option to only update playercount at the start of a stage.
	- Technically, this just makes it so that playercount can't decrease until a new stage starts.
		- Playercount can still increase when new players connect.

1.1.1

- Now compatible with ZetArtifact's Artifact of Multitudes.

1.1.0

- Simplified hook (based on Multitudes code from https://github.com/wildbook/R2Mods/blob/master/Multitudes/Multitudes.cs)
- Now compatible with Multitudes

1.0.1

- Fixed a typo in the internal plugin name.

1.0.0

- Release