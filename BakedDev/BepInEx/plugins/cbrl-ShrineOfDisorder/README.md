# Shrine of Disorder

Modifies the Shrine of Order behavior for more fun and less pain.

By default, this mod will make the Shrine of Order randomize items per-stack instead of per-tier. This means you will still have the same number of unique stacks after using the shrine, instead of one stack per item tier, meaning the shrine is not necessarily a death sentence any longer.

The Shrine of Order will now also have the ability to spawn on every map, giving more opportunities to use it.

Configuration options are available for most features, such as the shrine behavior, shrine spawn chance, whether the shrine can spawn on all maps, and whether to randomize special items (e.g. lunar, void, boss).

## Configuration

### Behavior

The following options modify the behavior of shrine effect, as well as where and how often it can spawn.

#### `ShrineBehavior`

- `RandomizeEachStack` - For each stack of items in the player's inventory, replace it with an equal size stack of a randomly chosen item in the same tier.
- `RandomizeEachItem` - For each item in the player's inventory, replace it with a randomly chosen item of the same tier.
- `SwapOneInventory` -  Swap the inventory of the player which activated the shrine with one other randomly selected player.
- `SwapAllInventories` - Randomly swap the inventories of every player.

**Warning:** The shrine behaviors which swap player inventories are currently untested.

Defaults to `RandomizeEachStack`.

#### `OnlyObtainedItems`

When determining which items to give the player, only consider the items that they have in their inventory as potential candidates.

Disabled by default.

#### `PreserveStackCount`

If using the `RandomizeEachStack` behavior, enabling this option will preserve the number of unique stacks a player has in their inventory. If disabled, the same item could be randomly selected for different stacks, effectively merging them.

Enabled by default.

#### `ShrineOnAllMaps`

Allows the shrine to spawn on all maps.

Enabled by default.

#### `ShrineSpawnMultiplier`

A multiplier on the shrine's spawn weight. Higher values will increase the chance for the shrine to spawn, and decrease the chance for other shrines to spawn.

### Items

Each of the options under the "Items" category will allow or disallow certain item tiers to be considered when randomizing items. The available options are as follows:
- `LunarItems` - Allows lunar items to be randomized if enabled.
- `VoidItems` - Allows void items to be randomized if enabled.
- `BossItems` - Allows boss items to be randomized if enabled.
- `VoidBossItems` - Allows void boss items to be randomized if enabled.

## Changelog

**1.1.4**
- Fixed a bug causing items to disappear from the inventory when using the shrine if they belong to a tier that is disabled in the configuration

**1.1.3**
- Documented the configuration options in the readme
- Updated some configuration descriptions
- Fixed some spelling errors
- Added a license

**1.1.2**
- Changed a configuration enum name to be a bit more accurate to its function.

**1.1.1**
- Added a list of stages the shrine will never spawn on, regardless of wether they have a shrines category or not.

**1.1.0**
- A good shrine weight is determined using the weight of shrines that are already in the rotation.
- Fixed the default behavior to match what is described.
- Fixed a bug that caused only one item of each tier to be given with the RandomizeItems behavior.

**1.0.0**
- Initial release
