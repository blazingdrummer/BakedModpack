- might be possible to add animation exceptions to `RTAutoSprintAddon` in order to prevent AA cancelling with characters like Commando or Acrid
- [x] tweak/test `ChensMinionRetarget` in combination with `Pingprovements`
  - turns out that the minion focus only lasts as long as the target ping, meaning it needs to be a reasonable length
- Greg brought up that sharing lunar coins might be affecting the percieved amount of coins available in multiplayer **IF** the drop rate is based on the number of players in-game
  - IIRC the drop rate is not affected, but if more enemies are spawning due to more players, this could be a factor; might be worth looking into

# Potential Bugs
- [ ] does `ItemExchangeNotifier` work properly with Scrappers? thought I noticed some strange chat formatting
- [ ] Greg got `ArtificerExtended` Temperature Drop unlock while hosting but not playing Artificer (I was)
  - unsure if this unlock normally requires you to be playing the character
  - also double-check that this issue isn't noted on the Thunderstore page yet; seem to maybe recall something about it
~~- Duck's mods don't support item discovery; could ask him to add it, or write a mod myself to add it to the profile~~
  - it seems like item discovery might not trigger when spawning items directly to inventory
- using Guillotine (equip) on a boss prevents the teleport charge skip and does not drop a boss item

# Custom To-Do
- while `ScalingBloodShrines` is good, blood shrines pose little actual risk to veteran players
  - randomize and hide the health cost of blood shrines and allow them to kill (inspired by `DiluvianDifficulty`)
  - could possibly implement as an artifact instead
- bring back the multi-shop improvements from `HarbTweaks`
  - consider that it technically does reduce RNG in builds slightly
- implement `Faster3DPrinters` for Scrappers; ideally would not close the UI every time you pick an item, allowing you to rapidly choose items (might have conflicts/interactions with `BetterUI`)
- recreate the QOL tweaks in `Raincoat`
  - allied Malachite patches are a different color
    - I think he actually used the purple translucent spikes from the Void Fields map?
  - the label color for Engi turrets is red to make them stand out
  - Capacitor (probably expand to any damaging equip) won't trigger while in the Bazaar and piss off the shopkeeper while using Gesture of the Drowned
    - need to make sure that tonic (and any other important ones?) will continue triggering
    - if GotD is an artifact instead, this probably isn't needed and should maybe be kept as a unique side effect
- recreate the noise alert before Engi shield drops; might be worth checking the archives for a random copy of `EngiShieldNotification` for somewhere to start
- bring back items from HarbCrate?
- bring back Corpsebloom fix from `GeneralFixes`?
- would be cool if keyword descriptions showed up in-game somewhere; maybe next to the description when hovering the ability like in character select
- implement `ShareSuite` behavior to deposit items from scrappers, printers, and cauldrons in singleplayer
  - `BiggerBazaar` does this already, might be able to copy it

## Language Improvements
- create a dynamic system for calculating proc chance **OR** modify the tooltips in `BetterUI` to reflect the changes made by mods
- use the rewritten descriptions from `BakedLanguageEdits`
- probably just worth searching the wiki for "correction" keyword
- [Weaken has wrong description in-game according to wiki](https://riskofrain2.fandom.com/wiki/REX#Natural_Toxins)
- [Ravenous Bite might also not be "Slayer" since the wiki seems to indicate only a 200% damage increase based on health](https://riskofrain2.fandom.com/wiki/Acrid#Ravenous_Bite)
- [couple of caveats to 'DIABLO' Strike](https://riskofrain2.fandom.com/wiki/Captain#OGM-72_.27DIABLO.27_Strike)
- [Orbital Supply Beacon doesn't mention the damage done when landing on an enemy in vanilla](https://riskofrain2.fandom.com/wiki/Captain#Orbital_Supply_Beacon)
- [Power Mode's slow doesn't match description](https://riskofrain2.fandom.com/wiki/MUL-T#Power_Mode)
- [Phase Round's damage description is off](https://riskofrain2.fandom.com/wiki/Commando#Phase_Round)
  - not sure if the math checks out on this?

# Potential Additions
- [CloakBuff](https://thunderstore.io/package/DestroyedClone/CloakBuff/)
