# Phedg1 Studios
# Item Drop List

## TLDR
This mod will allow players to choose which items can be found in chests and from boss drops.

## DESCRIPTION
The main menu will have a new button labelled "Item Drop List". Clicking it will open up the drop management interface. Every item and piece of equipment that has been unlocked (completed the requisite achievement) and discovered (been picked up at least once) will be listed here. Every item or piece of equipment that will be available when playing the game will be shown in full colour. Every item or piece of equipment that will not be available will be shown darkened. Left click and item or piece of equipment to toggle its availability. You are no longer required to have at least 1 item of every tier enabled. In fact, it is possible to play games with every single item disabled. Chests that are spawned will always give out an item. If every item a particular chest is able to spawn has been disabled that chest will no longer be spawned. This also applies unique interactables like Shrines of Order (if you have every item disabled), Scavenger Backpacks, Cleansing Pools and 3D Printers to name a few. All drones are also listed in this menu and enabled or disabled as well.

This mod does not change item rarity spawn chance, other than where certain tiers are completely disabled. Making an item available or unavailable does not change whether it has been unlocked or discovered on the player's profile. This mod can be enabled and disabled from this menu, should the player wish to play normally again.

## CONFIGURATION
After a player has opened the item shop interface for the first time a number of configuration files will be created. These can be found at "<RISK OF RAIN 2 INSTALL LOCATION>/Risk of Rain 2/BepInEx/config/Phedg1 Studios/Item Drop List/<YOUR PROFILE ID>/". If you desire to alter the configuration of the mod it must be done by editing these files. The intention is that this would only be necessary once, with the rest of the player's interactions being done through the shop interface inside the game itself.

Config.cfg
This file contains all of the settings which persist between profiles. It stores the whether the mod is currently enabled or disabled, whether all items (including items which have not been unlocked) should be listed and the multiplier for how many interactables should be spawned per stage.

ItemsToDrop.txt
This is the record of what items and equipment the player has chosen to make available, so that they can persist after the game has been closed.

## Changelog
v1.1.2
Changed configuration files and extensions to better support r2modman.

v1.1.1
Added ability to toggle whether spawning for each drone type.

v1.1.0
Now compatible with the Artifacts update.
Updated the visual style to match the new UI.
Fixed UI scaling at different resolutions and aspect ratios.
Increased the scrolling speed of the starting items menu.
Fixed a bug where unfinished items would show when show all items was enabled.
Decoupled the mod UI from the base game to a much greater extent.
Boss item drops, adaptive chests, scavenger backpacks, cleansing pools and many other interactables now working correctly.
Fixed chests given no items.
Added functionality to prevent chests from spawning if they have no items to give.
Added ability to scale the amount of interactables spawned per stage.

v1.0.0
Initial Release