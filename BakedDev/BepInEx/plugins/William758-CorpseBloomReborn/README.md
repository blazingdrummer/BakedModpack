# CorpseBloomReborn

![demo](https://i.imgur.com/br3CsIG.png)

Corpsebloom now grants a percentage of maximum health as reserve.

- Healing is stored into reserve and heals you over time.

Prevent healing multipliers from affecting healing twice while using Corpsebloom.

- Rejuvenation Rack double healing can be re-enabled with config.

Configure when healing goes into reserve. (these are disabled by default)

- HealBeforeReserve prioritizes healing into health before going into reserve.

- HealWhenReserveFull will cause any extra healing past full reserve to go back into health.

Reserve usage is modified by different situations.

- Reserve has a minimum and maximum usage rate.

- Reserve is not used while under the effect of Malachite HealingDisabled.

- Reserve is used at minimum rate when fully healed.

- Aegis causes usage rate to approach maximum as barrier fraction approaches 0.

- Reserve usage rate being divided by stack count can be re-enabled with config.

Current reserve is shown as a purple bar on the HealthBar of the HUD and AllyCards.

https://streamable.com/qh79ba

## Installation:

Requires Bepinex and HookGenPatcher.

Use r2modman or place inside of Risk of Rain 2/Bepinex/Plugins/

## Changelog:

v1.2.2 - ReserveBuff is now hidden. Aegis now effects reserve usage rate.

v1.2.1 - Fixed RestoreRejuvBehavior applying to ExportMult instead of AbsorbMult.

v1.2.0 - Updated for latest game version. Now only uses HookGenPatcher. ReserveBars for allies.

v1.1.1 - Fixed Eclipse artifact reducing healing twice.

v1.1.0 - Anniversary Update. Increased reserve amount. Healing now goes into reserve first by default.

v1.0.0 - Initial Release.

## Credits:

paddywan for creating CorpseBloomPlusPlus which I referenced to start this project.