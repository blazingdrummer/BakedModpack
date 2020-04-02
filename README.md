#### Please don't bug other devs with issues or feedback! Go to the [Contact Info](https://thunderstore.io/package/blazingdrummer/BakedModpack/#contact-info) section and I'd be happy to help you! I'll pass on any information the others will need, so try steer clear of the #tech-support channel of the main modding Discord with Baked-related questions if possible. Thanks!

---

It's come to my attention that anyone who installs the modpack fresh might end up getting the latest version of a mod, rather than the one desired by the modpack. This is fine, except if you are trying to play multiplayer and end up with a version mismatch. Ebkr and I have worked out a fix for it, but until he has a chance to release a patch for the mod manager, we'll have to compensate.

To start with, I'll keep up with modpack updates as quickly as possible, even if the changes are a single mod update, so that we can avoid the mismatch situation. I realize this might get a bit spammy, so I apologize in advance if it gets annoying.

As for you users, I'd highly recommend re-updating the pack if you are going to play with someone who recently installed or updated it to make sure you guys end up with the same mod versions. As long as there isn't a mod update introduced that seriously breaks things, these measures should work fine.

---

# Installation
  1. Install a mod manager that can automatically install dependencies (I'd recommend Ebkr's excellent [r2modman](https://thunderstore.io/package/ebkr/r2modman/) manager).

  2. Install the BakedModpack "mod" to automatically install all of the mods and configure them.
    - With r2modman, simply install the program, create a new profile, click the **Online** section, and search for "BakedModpack". Then click **Download**.

  3. Read the Overview below for a brief rundown on the changes you need to know about before playing the modpack, join the [Discord](https://discord.gg/QRtdUbV) to stay up-to-date with any changes, and check out the [BakedMutators](https://thunderstore.io/package/blazingdrummer/BakedMutators/) addon package for some fun twists on the game.

  4. Click **Play Modded**.

## Updating
  1. Create a new profile in r2modman.

  2. Follow Step 2 in **Installation** above.

  (!) Before you do these last steps, if you would like to transfer your credit count for Starting Items GUI so you aren't starting over, skip to the **Transferring Credits** section below.

  3. Delete your old profile if you'd like.

  4. Check the **Changelog** section at the bottom of this page for a quick rundown of what's different.

### Transferring Credits
  1. Click **Settings** in r2modman. Then click **Change Profile**. Select your *old* r2modman profile and enter into it.

  2. Click **Settings** again. Then click **Browse Data Folder** to open Windows Explorer to the proper location.

  3. Navigate to `mods/profiles/<old profile name>/BepInEx/config/Phedg1 Studios/Starting Items GUI`.

  4. Inside this folder, you will find a folder(s) labeled with your save file ID (e.g. 1ab2345c-678d-90ef-gh12-3i4567j89k01).

  5. Copy this folder to your clipboard.

  6. Restart steps 1-3 using your *new* r2modman profile instead **OR** simply go up 5 directories to get back to `mods/profiles` and then continue into `...profiles/<new profile name>/BepInEx/config/Phedg1 Studios/Starting Items GUI`.

  7. Paste the folder into that folder. If you already have an identical folder due to entering the Starting Items menu at least once or starting a run on this profile, then simply delete it, so your old credit count is transferred in.

  8. Return to Step 3 of the **Updating** section.

# Overview
If you've never played RoR2 before, or have only played a little, welcome and you're in luck! This pack is made with you in mind. I'd maybe recommend playing at least a couple of runs of vanilla before diving into the pack just to get into the swing of things, but honestly you should be just fine jumping right in.

If you're already a battered survivor of the storm, this pack should provide fresh new challenges and content, alongside much-appreciated QOL and balance changes. You can find all the details of everything that has been changed in the User's Guide found in the `#links` section of the [Discord](https://discord.gg/QRtdUbV).

These are the basic changes/differences you'll need to know to get started with the pack. You should be able to learn everything else by just playing the game.


# IMPORTANT DISCLAIMERS
This pack relies on lunar coins being a temporary currency that resets every run. You will be warned that your coins will be reset when you start a new game, and will need to type `tlc_aye` in chat before you can move at the beginning of the run.

If you value your lunar coins or the integrity of your save file in general, I'd recommend creating a new profile to use when playing this pack. However, the risk should be relatively low, as I test pretty thoroughly before releasing, and, worst case, you can always edit your coins using the `give_lunar {number_to_add}` command or edit the save file directly.

Speaking of commands and save files, I've left all of the admin tools I use active for your use if needed. This does leave the door open for cheating, but I think the potential usefulness in cases where glitches or mistakes happen outweighs this. Ultimately, you are in control of your own fun anways. See the [DebugToolkit commands list](https://thunderstore.io/package/Harb/DebugToolkit/#commands) and the admin keybindings below for more information. To use a command, press `F5` to bring up the console and then type the command in there. If you are copying the command from a Thunderstore page, make sure to ignore curly braces `{}` and replace them with the desired variable (e.g. `give_lunar {number_to_add}` becomes `give_lunar -5` to subtract 5 lunar coins). For information on how to edit your save file directly, please visit the [Discord](https://discord.gg/QRtdUbV).

## Recommended Settings
  - **Gameplay:** `sprint sensitivity reduction` = disabled
    - personal preference; this really messes with your sensitivity due to auto-sprint in my experience
  - **Video:** `resolution` = 1920x1080, `HUD scale` = 100%
    - This is by no means required, but I've only done very limited testing with resolutions other than this. Other resolutions or aspect ratios may cause UI issues. They should all be fixable, but will require you to adjust the configs to your own setup. Please consult the [Discord](https://discord.gg/QRtdUbV) if you need help doing this.
  - **Graphics:** `corpse clean-up` = immediate, `max corpses` = 0
    - I personally use this to remove clutter and increase performance. You don't have to do this, but I don't test without it, so your results may vary.

## New Keybindings
| Key | Function |
| --- | -------- |
| F1 | configure mods |
| F9 | quicksave |
| F10 | quickload |
| X | reset DPS meter |
| "sprint" | walk/cancel channeled ability |

## Admin Keybindings
| Key | Function |
| --- | -------- |
| F2 | macro: god, noclip |
| F3 | macro: no_enemies, kill_all |
| F5 | open console |
| F6 | reload RPGMod config |
| F8 | give players a starter pack |

## Basic Changes
### [BakedLanguageEdits](https://thunderstore.io/package/blazingdrummer/BakedLanguageEdits/)
  - almost every item/equipment’s tooltips, as well as many menus and ability descriptions, have been modified to reflect any changes made by this modpack and give players more detail about mechanics
  - picking up items/equipment or hovering over them in the Tab menu shows a more complete description of what that item does, including exact damage values, cooldowns, and chances
    - don’t worry, there are still secrets hidden in the logbook ;)
### [RTAutoSprintEx](https://thunderstore.io/package/JohnEdwa/RTAutoSprintEx/)
  - your character will automatically sprint whenever the base game would normally allow you to sprint
  - inverts the "sprint button" behavior; the "sprint button" is now a "walk button" which also cancels some channeled abilities, like Artificer's flamethrower
  - stops the FOV from changing, eliminates the speedlines, and gets rid of the chevron crosshair when sprinting (adjustable in config)
### [Pingprovements](https://thunderstore.io/package/pixeldesu/Pingprovements/)
  - there is no longer any limit to how many pings you can have active at once
  - ping duration now depends on type: interactable pings last a long time, allowing you to ping things like chests or the teleporter that you want to return to later; this also applies to items on the ground, so you can leave them for a teammate
### [AllyPing](https://thunderstore.io/package/mistername/AllyPing/)
  - pinging an enemy now makes your minions target them
### [FasterTeleportCharge](https://thunderstore.io/package/TheRealElysium/FasterTeleportCharge/)
  - after the teleporter boss is killed, the charge rate is 1000x its normal speed; the saved time is still tracked and added to the run timer to preserve difficulty
### [Starting Items GUI](https://thunderstore.io/package/Phedg1Studios/StartingItemsGUI/)
  - You now earn credits based on stages cleared, game difficulty, and run ending (higher rewards for wins/obliterations)
  - Credits can be spent in the `Starting Items` section of the main menu for a boost on your next run
### [FixedSplitscreen](https://thunderstore.io/package/xiaoxiao921/FixedSplitscreen/)
  - better splitscreen support is available through this mod; see the [mod page](https://thunderstore.io/package/xiaoxiao921/FixedSplitscreen/) for details
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
### [VanillaTweaks](https://thunderstore.io/package/RyanPallesen/VanillaTweaks/)
**Multiplayer-Only**

  - In multiplayer, you no longer pick up items by moving through them; You must press `Interact` (default E)

There are dozens of other changes made to the game and addtional content, including characters and items, that are not mentioned in this brief overview. As previously mentioned, they should all be discoverable and learnable just by playing the game, but if you would like a full spoiler-heavy rundown of all of the changes made, you can find it in the User's Guide found in the `#links` section of the [Discord](https://discord.gg/QRtdUbV).

# Known Issues
Many of these issues are marked in-game with a wrench icon to indicate they are known. Please refer back to this section if you see one.
### Impossible Challenges
Due to the nature of modded RoR2 and how the pack uses lunar coins, there are 3 challenges from the base game that are nearly or completely impossible to complete when playing this pack. I'd recommend picking one of the presented solutions when you run into this situation.

  - `Prismatically Aligned`: Complete a Prismatic Trial
    - While you are playing a modded instance, prismatic trials are not available (to prevent cheating). Your options are: complete this challenge in vanilla RoR2 before returning to modded play, or modify your save file. For information on how to edit your save file directly, please visit the [Discord](https://discord.gg/QRtdUbV).
  - `Mercenary: Ethereal`: As Mercenary, complete a Prismatic Trial without falling below 100% health.
    - Same as `Prismatically Aligned`.
  - `Pause.`: Free the survivor suspended in time.
    - Because this challenge requires at minimum 10 lunar coins to complete, it is uniquely difficult in this modpack, because you'd need to achieve it in one run. Lunar coins' drop chance also decreases for that run every time one drops, making this challenge potentially nearly impossible. Your options are: disable the TemporaryLunarCoins mod in r2modman and play normally until you complete this challenge, use the `give_lunar 10` command to gain the necessary coins, or modify your save file. For information on how to edit your save file directly, please visit the [Discord](https://discord.gg/QRtdUbV).

### Known Bugs/Problems
  - spectral circlet has no texture and is invisible, making it nearly impossible to pick up if you didn't see it drop
  - loading into the Bazaar using a game save causes the BiggerBazaar chests to not spawn
    - simply don't save your game in the Bazaar or do your shopping beforehand
  - Playing on Diluvian is not properly counted as Monsoon by Starting Credits GUI, so you don't get any extra credits from the multipliers, only for the number of stages cleared. Options right now for getting lots of credits until Phedg can take a look at it are:
    - playing on monsoon instead of diluvian
    - doing the math yourself and adjusting your credit count manually by editing the config file that stores the credits
      - monsoon's consumable formula would be `({stage count} * {difficulty multiplier = 8} * {ending multiplier = 2.5 (win), 1.5 (loss), 2 (obliteration)}) - {stage count}`
      - monsoon's persistent formula would be `({stage count} * {difficulty multiplier = 4} * {ending multiplier = 2 (win), 1 (loss), 1.5 (obliteration)}) - {stage count}`
  - (not really a bug?) going to the next stage toggles `noclip` off and takes focus away from the console
#### Multiplayer-Only
  - price labels on the modded portions of the Bazaar display as gold rather than lunar coins for clients (e.g. $1 instead of 1 lunar); also affects fuel array chest
  - Scavengers and the Void Fields don't scale back items to compensate for item sharing, resulting in large power spikes for players
    - I'd recommend compensating by only picking up 1 item from the Void Field rewards instead of all of them; a similar approach could be taken with Scavengers, but they are more difficult to balance; maybe try picking up `{# of items}/{# of party members}` items
  - the red item cauldron in the Bazaar gives the player a red item directly into their inventory, but also drops one on the ground, resulting in duplication
    - simply don't pick up this item; in the case that you accidentally do and want to remove it, simply use the command `remove_item {item_name} 1`
  - when playing as Void Reaver as the client, you must use the alternate `Client Reave` ability available in his loadout for his special to function properly, albeit without the fancy effects

For a more up-to-date list, check the `#known-issues` channel on the [Discord](https://discord.gg/QRtdUbV).

# Contact Info
Join the [Baked Discord](https://discord.gg/QRtdUbV), or DM on Discord or Twitter [@blazingdrummer](https://twitter.com/blazingdrummer).
**Please don't bug other devs with issues or feedback! I'd be happy to help you! I'll pass on any information the others will need, so try steer clear of the #tech-support channel of the main modding Discord with Baked-related questions if possible. Thanks!**

## Credits
I'd like to give a massive shoutout to all of the developers and other members of the RoR2 modding community for all of their help and support so far. This project started in January 2020 and has been immmensely satisfying to work on, so I really hope everyone enjoys it.

In particular, I'd like to thank Ebkr, Moffein, Rein, Magnus, Sipondo & Funkfrog, Mythic, Harb, Fubuki, and Phedg1 for their hard work and graciously both providing and considering input. And, of course, a big thank you to Hopoo Games!

## Changelog
In order to not make this readme any longer than it already is, the pre-release changes can be found in the `#changelog` section of the [Discord](https://discord.gg/QRtdUbV).

`v1.5.1`

  - initial release

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

`v1.5.3`

  - updated AcridPoisonBuffs to v0.3.0
  - README: added a notice for dealing with potential update issues until r2modman adds modpack support