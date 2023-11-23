## AccurateEnemies

Adds projectile aim prediction to elite enemies and bosses. Server-side and Vanilla-compatible.

## Affected Enemies

- Lemurian
- Elder Lemurian
- Beetle Guard
- Alloy Vulture
- Brass Contraption
- Greater Wisp/Archaic Wisp
- Lunar Exploder

- Wandering Vagrant
- Clay Dunestrider
- Grovetender (Chains)
- SCU/AWU
- Scavenger

- Blind Pest
- Alpha Construct
- Clay Apothecary
- Void Jailer

Certain enemies were ommitted due to the prediction not performing well on them.
Based on playtests, I've found that enemies still struggle with hitting airborne players, but get a decent accuracy boost against basic ground movement.

## Installation

Drop AccurateEnemies.dll into \BepInEx\plugins\

## Changelog

`1.0.9`

- Added config option to always enable prediction on bosses that support it. (Default: true)

`1.0.8`

- Remembered to add Inferno to the SoftDependency list so the mod can actually run its compatibility code.
- Changed default settings to Elite-Only since that seems to be the most popular setup. This will NOT change existing configs.
	- Elite Only: false -> true
	- Lemurian Loop Only: true -> false
	- Blind Pest Loop Only: true -> false

`1.0.7`

- Fixed Elite Only config option not working.
	- Was checking if victim is elite instead of attacker.

`1.0.6`

- Fixed Elite Only config changing the wrong setting.

`1.0.5`

- Added Elite Only config option (disabled by default).

`1.0.4`

- Added config options for each enemy to restrict projectile prediction to post-loop.
	- Restricted on Lemurians and Blind Pests by default.

`1.0.3`

- No longer attempts to predict against cloaked targets.

`1.0.2`

- Now attempts to predict against jumping players.

`1.0.1`

- Fixed manifest.

`1.0.0`

- Release.