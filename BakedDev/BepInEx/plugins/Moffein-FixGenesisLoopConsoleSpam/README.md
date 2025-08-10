## FixGenesisLoopConsoleSpam

```[Warning: Unity Log] Particle System is trying to spawn on a mesh with zero surface area```

Prevents Genesis Loop from spamming the console with the above message by disabling the particle effects on meshes with 0 tri-count.

Certain modded skins have unreadable tri-counts, so the mod simply allows them by default since most work fine. If you are still getting console spam, disable this in the config. (Can also be changed in-game with RiskOfOptions)

## Installation

Place FixGenesisLoopConsoleSpam.dll in /Risk of Rain 2/BepInEx/plugins/

## Changelog

`1.0.0`

- Release.