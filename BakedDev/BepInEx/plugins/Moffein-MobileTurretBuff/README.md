## MobileTurretBuff
Gives Engi's Mobile Turrets extra survivability and range.
- Mobile Turrets now sprint whenever possible, instead of only sprinting when far away.
- HP Regen values have been increased from 0.6/0.12 to 1/0.2
- Range increased 25 -> 45

Server-side mod. Only the host needs the mod.

## Installation
Place MobileTurretBuff.dll in /Risk of Rain 2/BepInEx/plugins/

##Config Options
The config can be modified in /Risk of Rain 2/BepInEx/config/com.Moffein.MobileTurretBuff.cfg
- Base HP Regen
- Level HP Regen
- Base Armor
- Level Armor
- Base Damage
- Level Damage
- Base Move Speed
- Laser Range

## Changelog

1.1.8

- Hopefully fixed Vanilla compatibility issues.

1.1.7

- Improved range modification code. (Now modifies the EntityStateConfiguration instead of using a hook)

1.1.6

- Updated for DLC update
- Removed base armor.
- Reduced health regen from 2.5 -> 1.0

1.1.5

- Swapped dependency to HookGenPatcher.

1.1.4

- Fixed lingering R2API dependency
- Increased range from 25 -> 45. For reference, stationary Engi turrets have a range of 60.

1.1.3

- Removed AOE resistance config option since Drones don't use it anymore.
- Turret base armor increased 0 -> 12.

1.1.2

- Removed unused Range setting. This simply changed the movement speed, and never had any code written for it at any point in time.

1.1.1

- Base armor reduced from 20 to 0 since Rose Bucklers are a free +30 armor.
- NetworkCompatibility stuff

1.0.1

- Disabled AOE Resistance by default. I was under the assumption it only affected Vagrant novas based on the patch notes that added it, but it turns out that it affects all explosions.
- Made Mobile Turrets sprint whenever possible

1.0.0

- Release