# AI Blacklister
Lets you blacklist certain items and equipment so that Scavengers and enemies in the Void Fields will never receieve them.

## Installation
1. Move `AIBlacklister.dll` to `Risk of Rain 2\BepInEx\plugins`.

*You may optionally make a folder and put the .dll file inside of it for organizational purposes.*

## Configuration
1. Install the plugin.
2. Run the game and a configuration file will be generated at `Risk of Rain 2\BepInEx\config`.
3. Open `com.unordinal.aiblacklister.cfg` with any text editor.
4. Edit the settings to your preference.

### Settings
*Valid item code names can be found [here](https://github.com/risk-of-thunder/R2Wiki/wiki/Item-&-Equipment-IDs-and-Names). By default, all blacklisted vanilla items are set in the config. Removing them from the config will allow the AI to receive these items. The equipment are ones I personally put in to lessen the amount of deaths by Scavengers that were out of the player's control or were just useless, such as the Scanner.*

`ItemBlacklist`: A comma-separated list of item code names. Items here are blacklisted for the AI, which means they'll never receive them in events such as the Void Fields or Scavenger's item gain ability. The default items here are also blacklisted in vanilla, aside from `ShockNearby` (Unstable Tesla Coil).

`EquipmentBlacklist`: A comma-separated list of equipment code names. Equipment here are blacklisted for the Scavenger AI, which means they'll never spawn with any of these equipment items.

## Changelog
### `1.0.0`
- Initial release.
