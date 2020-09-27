### PLEASE read this page carefully before beginning to play the modpack! I get a lot of questions that have easy answers listed right here. I promise I kept all unnecessary information out of it and and won't waste your time.

#### Please don't bug other devs with issues or feedback! Go to the [Contact Info](https://thunderstore.io/package/blazingdrummer/BakedModpack/#contact-info) section and I'd be happy to help you! I'll pass on any information the others will need, so try steer clear of the #tech-support channel of the main modding Discord with Baked-related questions if possible. Thanks!

# Installation
  1. Install a mod manager that can automatically install dependencies **and** handle modpack (packages that include a `.modpack` file) installation. (Ebkr's excellent [r2modman](https://thunderstore.io/package/ebkr/r2modman/) is the **ONLY** manager that I know of that currently supports both of these. Using another manager might result in version mismatch and multiplayer issues.)

  2. Install the BakedModpack "mod" to automatically install all of the mods and configure them.
      - With r2modman, simply install the program, create a new profile, click the **Online** section, and search for "BakedModpack". Then click **Download**.

  3. Read the Overview below for a brief rundown on the changes you need to know about before playing the modpack and join the [Discord](https://discord.gg/CYYJdrz) to stay up-to-date with any changes.

  4. Click **Play Modded**.

## Updating
  1. Select the **BakedModpack** entry in r2modman and click **Update**.

  2. Check the **Changelog** section at the bottom of this page for a quick rundown of what's different. If there are any mods that have been removed, please manually uninstall them to prevent issues or create a new profile and follow the [Installation](https://thunderstore.io/package/blazingdrummer/BakedModpack/#installation) instructions again.

# Overview
If you've never played RoR2 before, or have only played a little, welcome and you're in luck! This pack is made with you in mind. I'd maybe recommend playing at least a couple of runs of vanilla before diving into the pack just to get into the swing of things, but honestly you should be just fine jumping right in.

If you're already a battered survivor of the storm, this pack should provide fresh new challenges and content, alongside much-appreciated QOL and balance changes. You can find all the details of everything that has been changed in the [User's Guide](https://github.com/blazingdrummer/BakedModpack/wiki/User's-Guide).

These are the basic changes/differences you'll need to know to get started with the pack. You should be able to learn everything else by just playing the game.

## IMPORTANT DISCLAIMERS

### Lunar Coins
This pack relies on lunar coins being a temporary currency that resets every run. You will be warned that your coins will be reset when you start a new game, and will need to type `TLC_AYE` in chat before you can move at the beginning of the run.

If you value your lunar coins or the integrity of your save file in general, I'd recommend creating a new profile to use when playing this pack. However, the risk should be relatively low, as I test pretty thoroughly before releasing, and, worst case, you can always edit your coins using the `give_lunar {number_to_add}` command or edit the save file directly (see the next paragraph for more information on this).

### Commands & Cheating Policy
Speaking of commands and save files, I've left all of the admin tools I use active for your use if needed. This does leave the door open for cheating, but I think the potential usefulness in cases where glitches or mistakes happen outweighs this. Ultimately, you are in control of your own fun anyways. See the [DebugToolkit commands list](https://thunderstore.io/package/Harb/DebugToolkit/#commands) and the admin keybindings below for more information. To use a command, press `F5` to bring up the console and then type the command in there. If you are copying the command from a Thunderstore page, make sure to ignore curly braces `{}` and replace them with the desired variable (e.g. `give_lunar {number_to_add}` becomes `give_lunar -5` to subtract 5 lunar coins). For information on how to edit your save file directly, check out [this guide](https://steamcommunity.com/sharedfiles/filedetails/?id=1704500228) or visit the [Discord](https://discord.gg/QRtdUbV) if you have questions.

### Modifying The Pack
This pack is meant to be a framework. The entire purpose of it is to give people who are new to the scene a starting point. Because of this, I am totally fine with modifying the pack in whatever way you desire... adding mods, removing mods, changing options, etc. I only have two requests if you choose to do so.

1. Please shoot me a message or something about why you chose to make a change. One of the biggest things that hurts a scene is when people don't give devs feedback, and I want to know if there's something that's a problem or just not fun. There's multiple way to get in touch in the [Contact Info](https://thunderstore.io/package/blazingdrummer/BakedModpack/#contact-info) section. We might have differences of opinion, but I'm not going to judge you, don't worry :)
2. If you make major changes (like not just disabling auto-sprint, the DPS meter, or something else client-side), then please mention that when asking for troubleshooting help. I'd be happy to help out however I can, but I won't take responsibility for something outside of my control.

"So how do I actually change things?" Well, that part's actually pretty simple. For example, if you don't like the DPS meter, the good news is that DPSMeter is a client-side mod and you can simply click it in **r2modman** and then click **Disable** without affecting anyone else. Some mods (eg RTAutoSprintEx) have in-game commands that let you adjust them. Other mods (eg ShareSuite) might affect multiplayer, so disabling them will affect your friends if you are the host. Still other mods have issues if not loaded on both sides (ie mods that add characters or other assets not in the base game). Installing new mods is as simple as going to the **Online** tab and clicking **Install**, running the game once to generate the config, and then using the config editor to adjust them.

Note: One quirk of a modpack set up like this is that disabling/uninstalling a mod will prompt r2modman to warn you that BakedModpack will also be affected. This isn't a problem, as the actual BakedModpack "mod" is just used as a dependency hook to load the other mods and doesn't have an effect on gameplay after installation. I'd recommend disabling mods rather than uninstalling, because then you can see when the BakedModpack entry needs an update by the little cloud icon next to it. Updating mods with that icon manually should be fine, but does have the potential to introduce new problems that I will not have tested.

## Recommended Settings
  - **Gameplay:** `sprint sensitivity reduction` = disabled
    - personal preference; this really messes with your sensitivity due to auto-sprint in my experience
  - **Video:** aspect ratio = 16:9, `HUD scale` = 100%
    - This is by no means required, but other aspect ratios may cause UI issues because the custom UI positions are all based on screen percentage. They should all be fixable, but will require you to adjust the configs to your own setup. Please ask me in the [Discord](https://discord.gg/CYYJdrz) if you need help doing this.
  - **Graphics:** `corpse clean-up` = immediate, `max corpses` = 0
    - I personally use this to remove clutter and increase performance. You don't have to do this, but I don't test without it, so your results may vary.

## New Keybindings
| Key      | Function                      |
| -------- | ----------------------------- |
| F1       | configure mods                |
| X        | reset DPS meter               |
| "sprint" | walk/cancel channeled ability |

## Admin Keybindings
| Key | Function                        |
| --- | ------------------------------- |
| F2  | macro: `god`, `noclip`          |
| F3  | macro: `no_enemies`, `kill_all` |
| F5  | open console                    |
| F7  | give players a starter pack     |

## Basic Changes
### [BakedLanguageEdits](https://thunderstore.io/package/blazingdrummer/BakedLanguageEdits/)
  - almost every item/equipment’s tooltips, as well as many menus and ability descriptions, have been modified to reflect any changes made by this modpack and give players more detail about mechanics
  - picking up items/equipment or hovering over them in the Tab menu shows a more complete description of what that item does, including exact damage values, cooldowns, and chances
    - don’t worry, there are still secrets hidden in the logbook ;)
### [RTAutoSprintEx](https://thunderstore.io/package/JohnEdwa/RTAutoSprintEx/)
  - your character will automatically sprint whenever the base game would normally allow you to sprint
  - inverts the "sprint button" behavior; the "sprint button" is now a "walk button" which also cancels some channeled abilities, like Artificer's flamethrower
  - stops the FOV from changing, eliminates the speedlines, and gets rid of the chevron crosshair when sprinting

| Command                            | Function                                                     |
| ---------------------------------- | ------------------------------------------------------------ |
| `rt_help`                          | list all possible console commands                           |
| `rt_enabled`                       | disable/enable most of the sprinting functionality           |
| `rt_fov`                           | changes CustomFOV variable {1 - 359, default: 60} |
| `rt_artificer_flamethrower_toggle` | sets the flamethrower mode                                   |

### [Pingprovements](https://thunderstore.io/package/pixeldesu/Pingprovements/)
  - there is no longer any limit to how many pings you can have active at once
  - ping duration now depends on type: interactable pings last a long time, allowing you to ping things like chests or the teleporter that you want to return to later; this also applies to items on the ground, so you can leave them for a teammate
  - pinging an item/equipment now shows its description as if you had picked it up
### [AllyPing](https://thunderstore.io/package/mistername/AllyPing/)
  - pinging an enemy now makes your minions target them
### [StartingItemsGUI](https://thunderstore.io/package/Phedg1Studios/StartingItemsGUI/)
  - earn credits by killing late-game bosses (currently only Lunar Scavengers) to gain a one-time boost for future runs
  - credits earned are based on the difficulty you play on (50 credits per kill, 2x/4x/8x multipliers for drizzle/rainstorm/monsoon respectively)
  - click the **Starting Items** button on the main menu to view earned credits and available items; the list is based on your discovered items, so flesh out your logbook to expand your options!
### [ShareSuite](https://thunderstore.io/package/FunkFrog-and-Sipondo/ShareSuite/)
**Multiplayer-Only**

  - picking up a white or green item gives every other **living** member of your party a random item of the same tier
    - red, yellow, and blue items are not shared
  - using 3D printers & cauldrons directly modifies your build, not the other players' builds
  - balance changes: bosses only drop 1 item, less interactables spawn in early rounds
### [Shrine of Dio](https://thunderstore.io/package/MagnusMagnuson/ShrineOfDio/)
**Multiplayer-Only**

  - replaces the Shrine of the Woods with the Shrine of Dio, which lets you resurrect a random fallen teammate for a high gold cost
  - each normal stage spawns with a Shrine of Dio
### [TooManyFriends](https://thunderstore.io/package/wildbook/TooManyFriends/)
**Multiplayer-Only**

  - Unlocks the multiplayer lobby size (default max = 16, adjustable in config)
### [SimpleRoll](https://thunderstore.io/package/hlista/SimpleRoll/)

  - for the MMO fans; adds a /roll command to chat (not to console) that gives a number from 1-100
  - useful for solving item disputes; other options include finding nicer friends ;)

There are dozens of other changes made to the game and additional content, including characters and items, that are not mentioned in this brief overview. As previously mentioned, they should all be discoverable and learnable just by playing the game, but if you would like a full spoiler-heavy rundown (EDIT: COMING SOON) of all of the changes made, you can find it in the [User's Guide](https://github.com/blazingdrummer/BakedModpack/wiki/User's-Guide).

# Known Issues
Many of these issues are marked in-game with a wrench icon to indicate they are known. Please refer back to this section if you see one.
## Impossible Challenges
Due to the nature of modded RoR2 and a lack of access to Prismatic Trials, there are 2 challenges from the base game that are currently impossible to complete while playing this pack. I'd recommend picking one of the presented solutions when you run into this situation.

  - `Prismatically Aligned`: Complete a Prismatic Trial
    - While you are playing a modded instance, prismatic trials are not available (to prevent cheating). Your options are: complete this challenge in vanilla RoR2 before returning to modded play, or modify your save file. For information on how to edit your save file directly, check out [this guide](https://steamcommunity.com/sharedfiles/filedetails/?id=1704500228) or visit the [Discord](https://discord.gg/CYYJdrz) if you have questions.
  - `Mercenary: Ethereal`: As Mercenary, complete a Prismatic Trial without falling below 100% health.
    - Same as `Prismatically Aligned`.

## Known Bugs/Problems
  - (not really a bug?) going to the next stage toggles `noclip` off and takes focus away from the console
### Multiplayer-Only
  - price labels on the modded portions of the Bazaar display as gold rather than lunar coins for clients (e.g. $1 instead of 1 lunar); reported to Magnus
  - [GitHub link](https://github.com/blazingdrummer/BakedModpack/issues/3): the red item cauldron in the Bazaar, the Overgrown printer, and the Cleansing Pool all give the player an item directly into their inventory, but also drop one on the ground, resulting in duplication
    - simply don't pick up this item; in the case that you accidentally do and want to remove it, simply use the command `remove_item {item_name} 1`

For a more up-to-date list, check the [GitHub issues page](https://github.com/blazingdrummer/BakedModpack/issues) and the `#known-issues` channel on the [Discord](https://discord.gg/CYYJdrz).

# TODO
- updating the  wiki to include a complete description of all of the mods and how they are setup, and a guide for handling save edits and other aspect ratios
- working on solutions for the impossible challenges
- possibly bringing back BakedMutators once I figure out what would still be fun #PvPModeIncoming
- possibly extending BakedLanguageEdits to allow me to edit the descriptions of items added by mods (ie Rampage, Wicked Ring)
- as always, I'm keeping a look at for new content and QOL mods...

# Contact Info
Join the [Baked Discord](https://discord.gg/CYYJdrz), or DM me on Discord or Twitter [@blazingdrummer](https://twitter.com/blazingdrummer).
**Please don't bug other devs with issues or feedback! I'd be happy to help you! I'll pass on any information the others will need, so try steer clear of the #tech-support channel of the main modding Discord with Baked-related questions if possible. Thanks!**

## Credits
I'd like to give a massive shoutout to all of the developers and other members of the RoR2 modding community for all of their help and support so far. This project started in January 2020 and has been immensely satisfying to work on, so I really hope everyone enjoys it.

In particular, I'd like to thank Ebkr, Moffein, Rein, Magnus, Sipondo & Funkfrog, Mythic, Harb, Fubuki, Phedg1, Rico, Sciman101, Atlas_, and KingEnderBrine for their hard work and graciously both providing and considering input. And, of course, a big thank you to Hopoo Games!

## Changelog
In order to not make this readme any longer than it already is, the pre-release changes can be found in the `#changelog` section of the [Discord](https://discord.gg/CYYJdrz).

`v3.0.0`

  - updated BazaarPrinter to v0.2.2
  - updated DeathMarkFix to v1.0.2
  - updated SpeedyBeetles to v1.0.5
  - added IlLine v1.0.0
  - added StartingItemsGUI v1.1.5
  - added OrderedItems v2.2.1
  - added Phase_Round_Lightning v1.0.0
  - added ArtificerExtended v1.2.1
  - added HarbCrate v1.0.2
  - updated GeneralFixes to v1.3.4
  - updated BanditReloaded to v1.2.0
  - updated RogueWisp to v2.1.5
  - updated TemporaryLunarCoins to v0.2.1
  - README: inverted changelog to make it easier to find changes

  - added ProperSave v2.1.1
  - replaced Bepinex ConfigurationManager (now v16.0.0)
  - removed FluffyLabsConfigManagerTools, BulletFalloffFix, InfusionStackfix, MacroCommands

  - updated R2API to v2.5.14
  - updated LighterPatcher to v1.0.4
  - updated DebugToolkit to v3.4.1
    - macros have been remapped using DebugToolkit's new system, replacing the functionality of MacroCommands
    BUG: command autofills can't be generated unless `Microsoft.CSharp.dll` is placed next to `DebugToolkit.dll`; Will this have an impact on pack installation?
    TODO: adjusted HarbTweaks config to disable redundant and undesired features; need to update to 1.0 compatible version, Harb indicated he would be updating the mod soon
  - updated Pingprovements to v1.7.0
  - updated ShareSuite to v2.3.0
  - updated ShrineOfDio to v1.4.1
    TODO: should Captain be able to hack Shrine of Dio?
  - updated TooManyFriends to v1.1.0
    TODO: add `mod_tmf {lobby size}` command to README; maybe make a section and move link to DebugToolkit commands there as well
  - updated ScannerPlusOne to v2.6.1
  - updated ItemExchangeNotifier to v1.3.1

`v2.3.2`

  - updated MobileTurretBuff to v1.1.0
  - updated R2API to v2.4.21
    - this fixed the bug with DebugToolkit concerning commands

`v2.3.1`

  - removed StartingItemsGUI & ItemDropList until issues (hopefully) can be resolved
  - added MULT_Buff v1.0.0
  - updated GeneralFixes to v2.3.3
  - updated SpeedyBeetles to v1.0.4

`v2.2.6`

  - emergency removal of ItemDropList due to a bug
  - forgot to disable console last time...

`v2.2.5`

  - README: removed confusing references to old mods
  - added DeathMarkFix v1.0.1
  - added SpeedyBeetles v1.0.3
  - added MobileTurretBuff v1.0.0

`v2.2.4`

  - removed ShowDeathCause
    - was causing certain setups to hang when closing to desktop
  - added PocketPrinter v1.1.0
    - *Shoutout to Sciman101 for working with me to balance this mod and resolve issues*
  - removed OrderedItems due to current UI issue
    - [GitHub link](https://github.com/blazingdrummer/BakedModpack/issues/2): OrderedItems currently causes the top inventory bar to improperly display items at times
    - currently working with the author to hopefully reach a solution
  - updated HarbTweaks to v1.3.0
  - updated TheSurgeon to v1.4.2
  - disabled the chat function for ScannerPlusOne
    - this option tended to spam the chat when you had low equipment cooldown
    - scanner icons are still color-coded, so learning the colors shouldn't be too hard
  - updated LunarCoinShareOnPickup to v3.6.1
  - added GiganticAmethyst v1.1.1
    - *Shoutout to Rico for working with me to balance this mod*
  - updated StartingItemsGUI to v1.1.3
    - increased prices slightly; based on average run yield and balanced around Consumable mode
  - added ItemDropList v1.1.2
    - this mod will be disabled in-game by default to prevent mass confusion; you can enable it in-game using its menu button
    - *Shoutout to Phedg1 for working with me to make these compatible with modpack default configurations and changing his config system to work with r2modman's editor*

`v2.1.0`

  - README: updated 1920x1080 resolution recommendation to 16:9 aspect ratio
    - thanks to CarlosPCMR for checking this for me!
  - updated BanditReloaded to v1.1.1
    - adds Vengeance support (both RogueWisp and BanditReloaded now have this)
  - updated Void_Reaver to v0.2.2
  - updated DiluvianDifficulty to v1.0.5
  - updated ShareSuite to v2.0.0(!)
    - fixes the scavenger bug
    - resolves issue with Sacrifice dropping way too many items
  - README:
    - added a notice about modifying the pack
    - added section headers to **Disclaimers**

`v2.0.4`

  - updated this page's link to direct to this project's GitHub
  - updated BepInEx to v3.2.0
  - updated R2API to v2.4.10
  - updated Pingprovements to v1.5.1
  - updated ShrineOfDio to v1.3.2
  - updated RTAutoSprintEx to v1.0.6
    - added console command notes to README, including FOV control
  - updated DiluvianDifficulty to v1.0.4
  - updated ShareSuite to v1.15.1
    - added player scale-back support for the Void Fields
  - updated BiggerBazaar to v1.9.3
    - increased price of chests from 1, 2, 3 -> 1, 3, 5
  - updated TemporaryLunarCoins to v0.2.0
  - removed No_Scrap_Launcher_Falloff; replaced by vanilla functionality
  - updated InfusionStackFix to v5.0.2
  - adjusted AI item blacklist to be more threatening and to account for new items
    - due to vanilla changes to Capacitor and the new counterplay potential, Capacitor has been enabled
  - updated Rampage to v1.1.4
  - updated BanditReloaded to v1.0.2
  - updated TheSurgeon to v1.4.1
  - adjusted HarbTweaks for vanilla changes
    - disabled First Stage Spawns; replaced by vanilla functionality
    - disabled Shorter Medkits; vanilla changes make this too strong
  - updated HarbTweaks to v1.2.2
  - updated StartingItemsGUI to v1.1.1
    - README: removed **Transferring Credits** section due to new r2modman update functionality
    - now compatible with DiluvianDifficulty
    - increased scrolling speed of the menu
  - updated DebugToolkit to v3.3.1
  - added SolidIceWall v1.1.0
  - added ShowDeathCause v1.0.2
  - added BazaarPrinter v0.2.0
  - added LighterPatcher v1.0.1
  - updated Void_Reaver to v0.2.1
  - updated LunarCoinShareOnPickup to v3.6.0
  - updated GeneralFixes to v2.3.0
  - updated RogueWisp to v2.1.4
  - updated AlternativeArtificer to v1.1.0
  - removed FasterTeleportCharge
    - with the addition of Focused Convergence, waiting for teleporter to charge is less of an issue, and I don't want to make it a useless item
    - I'll be testing and getting feedback on this change for the near future
  - removed FixedSplitscreen
    - menu is slightly buggy now, but usable
    - can still be installed separately
  - removed SavedGames
    - waiting on compatibility update
    - think it causes lunar drop rate to reset; no proof of this, not sure where the value is stored
  - removed NetLib
  - removed VanillaTweaks
  - removed PlayableSora
  - removed PlayableAkali
  - removed MakeMonsterToothGreatAgain
  - removed AcridM1Heal

`v1.5.3`

  - updated AcridPoisonBuffs to v0.3.0
  - README: added a notice for dealing with potential update issues until r2modman adds modpack support

`v1.5.2`

  - updated DebugToolkit to v3.2.2
    - solved the errors caused by dying during `noclip`
  - updated DiluvianDifficulty to v1.0.3
  - README changes
    - added instructions for running commands in the console
    - added the reference to the #known-issues section of the Discord
    - added a changelog starting from initial public release only
    - added an "Updating" section
    - added instructions for transferring Starting Items credits
  - updated "Known Bugs/Problems"
  - updated BanditReloaded to v1.0.1
    - this should resolve an issue where Smokebomb didn't make him invisible when playing as client

`v1.5.1`

  - initial release
