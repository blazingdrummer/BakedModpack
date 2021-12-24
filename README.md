- might be possible to add animation exceptions to `RTAutoSprintAddon` in order to prevent AA cancelling with characters like Commando or Acrid
- [ ] tweak/test `ChensMinionRetarget` in combination with `Pingprovements`
- Greg brought up that sharing lunar coins might be affecting the percieved amount of coins available in multiplayer **IF** the drop rate is based on the number of players in-game
  - IIRC the drop rate is not affected, but if more enemies are spawning due to more players, this could be a factor; might be worth looking into

# Potential Bugs
- [ ] does `ItemExchangeNotifier` work properly with Scrappers? thought I noticed some strange chat formatting
- [ ] Greg got `ArtificerExtended` Temperature Drop unlock while hosting but not playing Artificer (I was)
  - unsure if this unlock normally requires you to be playing the character
  - also double-check that this issue isn't noted on the Thunderstore page yet; seem to maybe recall something about it

# Custom To-Do
- while `ScalingBloodShrines` is good, blood shrines pose little actual risk to veteran players
  - randomize and hide the health cost of blood shrines and allow them to kill (inspired by Diluvian)
  - could possibly implement as an artifact instead
- bring back the multi-shop improvements from `HarbTweaks`
  - consider that it technically does reduce RNG in builds slightly
- implement `Faster3DPrinters` for Scrappers; ideally would not close the UI every time you pick an item, allowing you to rapidly choose items (might have conflicts/interactions with `BetterUI`)

## Language Improvements
- create a dynamic system for calculating proc chance **OR** modify the tooltips in `BetterUI` to reflect the changes made by mods
- use the rewritten descriptions from `BakedLanguageEdits`
