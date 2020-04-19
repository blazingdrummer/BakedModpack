# Disclaimer & Usage
Hey, this is designed for use with the [Baked modpack](https://thunderstore.io/package/blazingdrummer/BakedModpack/). I would really appreciate if you checked it out!

Using these edits without the associated modpack might give you some confusing results (mainly descriptions that don't match behavior and some weird tooltips), but you are welcome to use it as a template for personal use or other packs if you'd like. Do your best RedRiot impression and add funny names or pop-culture references, I don't care. Use it however you want!

## What Does It Do?
BLE (BakedLanguageEdits) makes changes to the in-game text to support changes made by the modpack and to give users more information while they are playing.

Hovering over an item in the Tab menu or picking it up gives you more exact stats as to what it does, where in vanilla, this would simply say something like "increases attack speed". Normally, this information is only available in a wiki while you are playing, or in the logbook. It could be argued that this is a skill aspect of the game, and I agree that memorizing what items do is important, but personally I think that it's an unnecessary step. If you have to read every description, you'll be keeping a slower pace than if you already have an item's function memorized. And having this resource allows you to potentially theorycraft build options on the fly (eg figuring out if your current build will support infinite tonic).

![ItemHoverDescription](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/ItemHoverDescription.png)

Assuming you are playing with the highly recommended [Pingprovements](https://thunderstore.io/package/pixeldesu/Pingprovements/), pinging an item gives you a similar description.

![ItemPingDescription](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/ItemPingDescription.png)

Equipment also shows more exact numbers, as well as the base cooldown.

![EquipmentHoverDescription](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/EquipmentHoverDescription.png)

And supports pings.

![EquipmentPingDescription](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/EquipmentPingDescription.png)

This becomes particularly useful with something like Spinel Tonic, which has a lot of effects. I've done a large amount of formatting and editing on longer descriptions like this in order to ensure they don't run offscreen. This might have problems on different resolutions, which I could consider looking into potential solutions for.

![SpinelTonic](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/SpinelTonic.png)

I also moved the negative effects onto the description for Tonic Affliction. There are many other small tweaks like this.

![TonicAffliction](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/TonicAffliction.png)

Where this all really shines is with an item like Gesture that is affected by a mod (in this case, GeneralFixes). Gesture's default description does not mention it having a break chance, but with BakedLanguageEdits, it does now.

![GestureOfTheDrowned_Modded](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/GestureOfTheDrowned_Modded.png)

There's also some custom additions I did to the game's lore. I tried to keep these as subtle as possible, and not tread on any toes, while also respecting the original game's lore. Because it's not truly canon, I tried to focus on highlighting the existing known lore as much as possible instead of going crazy with my own ideas.

![SPOILER](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/SPOILER.png)

## How Do You Make Something Like This?
This might be a useful example for how to use AssetPlus to replace the game's language files in a non-destructive way. Feel free to mess around with this mod without having to worry about messing up your game.

I've also included a file named "styles.txt" that I used as my personal notes when creating this that contains all of the formatting syntax I (and originally Hopoo) used. If you are interested in doing any language edits yourself, I hope you will find that useful.

# Contact Info
Join the [Baked Discord](https://discord.gg/CYYJdrz), or DM me on Discord or Twitter [@blazingdrummer](https://twitter.com/blazingdrummer).
**Please don't bug other devs with issues or feedback. I'd be happy to help you and can pass on any information that they will need. Thanks!**

If you do find something that looks off or needs editing, please send me a screenshot like this. I only have two eyes and am sure I miss a lot of detail.

![EXAMPLE](https://raw.githubusercontent.com/blazingdrummer/BakedLanguageEdits/master/Images/EXAMPLE.png)

## Credits
  - Harb for creating and helping me figure out the AssetPlusRequester
  - ontrigger's ItemStatsMod for the original inspiration that I expanded upon

### TODO
  - considering making a mod specific to this pack that would allow me handle the cases that AssetPlus can't, such as editing the tooltips of modded items at runtime or calculating the current proc chance of items (ie replicating the function of ItemStatsMod)

## Changelog
`v1.0.0`

  - initial release

`v1.0.1`

  - changed example armor values on Rose Buckler from 1, 10, 50 to 100, 200, 300
    - the old values weren't that useful when Rose Buckler gives 30 armor per stack

`v1.0.2`

  - changed Fuel Array explosion condition to "health bar" rather than "maximum health"

`v1.1.0`

  - corrected "logarithmic" stacking to "hyperbolic"
  - removed exact drop rates from bandolier due to its custom formula
  - added "(+0% per stack)" to Harvester's Scythe, Wicked Ring, and Predatory Instincts
  - added the 5% crit chance to Predatory's descriptions
  - added base cooldowns to equipment
  - changed Acrid poison description from "maximum health" to "current health"
    - plus additional highlighting

`v1.2.0`

  - changed Acrid poison description from "based on current health" to "5% of their maximum health"
    - removed the stacking behavior to match the switch to using AcridPoisonBuffs instead of AlternativeAcrid
  - clarified that Commando's grenades explode "on impact"
  - added a note about "pinging enemies" to Engineer's turret tips

`v1.2.1`

  - removed the reference to SkipWelcomeScreen from the welcome screen due to distribution changes (can't automatically disable mods)
  - removed the notes on the character select screen about "mutators" due to transferring those to BakedMutators
  - removed the wrenches from the multiplayer button

`v1.2.2`

  - added AssetPlusRequester as a dependency :facepalm:
  - README: updated formatting

`v2.0.2`

  - Artifact 2.0 update
    - gave all of the new items and descriptions the same treatment (more complete in-game descriptions, cleaned up a couple typos, equipment cooldowns, etc)
  - updated for new GeneralFixes changes, removal of AcridM1Heal, poison nerfs from AcridPoisonBuffs, removal of VanillaTweaks, and removal of MakeMonsterToothGreatAgain

`v2.0.4`

  - fixed README images... uhh again

`v2.0.5`

  - updated this page's link to direct to this project's GitHub
  - started to modify a few character's ability descriptions; this is just the start of a large process of adding more detail to character select
  - fixed wording on Recycler to be more clear
  - clarified that the pack's User Guide is on the wiki

`v2.0.6`

  - added credit for new authors that I've worked with to the Welcome screen
  - slight edits to the Thunderstore page to clear up confusion with the synergy with Pingprovements
  - changed Bandolier description to clarify it only restores 1 charge, instead of completely resetting skills
  - removed chat readout reference from Scanner to reflect modpack change
  - sneaky Mad Max: Fury Road reference...