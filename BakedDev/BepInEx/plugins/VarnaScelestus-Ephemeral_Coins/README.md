# Ephemeral Coins

This mod aims to rebalance the Lunar Coin mechanic as a temporary currency, rather than a farmable one, in the hopes of improving not only the balance, but also the general satisfaction involved in acquiring Lunar Coins. Now fully compatible with [ProperSave](https://thunderstore.io/package/KingEnderBrine/ProperSave/)!

**All changes are configurable!**

- All Lunar Coins are removed upon starting a run. The amount removed is displayed in chat. [^1]
- Awards an amount of Lunar Coins to all players after removing all previous coins (default 0).
- Lunar Coins drop rate changed to 5% / 0.95 falloff.
- Lunar Pods made free of cost.
- Bazaar Between Time Lunar Buds cost lowered to 1 coin, and refresh when the Slab (Lunar Reroller) is used, even if already purchased.
- Bazaar Between Time Lunar Seer cost lowered to 1 coin.
- Bazaar Between Time Slab (Lunar Reroller) made free of cost. Can only be used once.
- The chance for a Blue Orb to appear on stage start flattened to 37.5%, instead of decreasing for each visit to BBT.

[^1]: For players who wish to restore their Lunar Coins, it is easily done through editing the "<coins>" tag in the save profile.

You can reach me (Varna) in the [RoR2 modding discord](https://discord.gg/5MbXZvd) with any feedback!

## Known Issues

- Occasionally, players in a multiplayer lobby do not appear to lose their coins client-side, despite the message in chat. The server still treats them as having 0 coins, however. (possibly ping related, unsure at this time)

## Todo

- Settings for Newt Altars, possibly a rework to their behavior
- Brainstorming on what to do with Lunar Coins received from obliterating/beating the game.
- Automatic lunar coin pickup.

## Credits

[Magnus](https://github.com/MagnusMagnuson/RoR2Mods) - For the original code this was forked from. Not only was it an excellent starting point, it helped me learn a lot too!

[RoR2 modding discord](https://discord.gg/5MbXZvd) - For help in figuring out the Slab (Lunar Reroller)'s horrible, horrible internal structure, and just being awesome in general!

## Changelog

1.2.0 - Improved compatibility with [ProperSave](https://thunderstore.io/package/KingEnderBrine/ProperSave/).

1.1.0 - Added config setting for a starting amount of Lunar Coins per player (defaults to 0).

1.0.4 - Added logic to prevent Lunar Pods from having their cost changed in the BBT to avoid conflicts with [BiggerBazaar](https://thunderstore.io/package/MagnusMagnuson/BiggerBazaar/). (They do not spawn there in vanilla anyway.)

1.0.3 - Fixed the multiplayer name issue for real this time

1.0.2 - Fixed version number and wrong default setting for Slab cost

1.0.1 - Fixed multiplayer names displaying incorrectly

1.0.0 - Initial release