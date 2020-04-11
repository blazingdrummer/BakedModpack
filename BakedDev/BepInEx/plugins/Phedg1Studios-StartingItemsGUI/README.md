# Phedg1 Studios
# Starting Items GUI

## TLDR
This mod will allow players to use a GUI to select which items will be given to them at the start of a run. There are 3 modes: Free, Earnt Persistent and Earnt Consumable. Works in both singleplayer and multiplayer (if the host and the client have the mod installed, enabled and are using the same mode).

## INSPIRATION
This mod was inspired by features in other roguelike games such as Undermine, Dungreed and Dead Cells. The goal was to give a returning player a sense of progression, to give them a boost to make them more formidable the more they play.

## DESCRIPTION
The main menu will have a new button labelled "Starting Items". Clicking it will open up the shop interface. Every item and piece of equipment that has been unlocked (completed the requisite achievement) and discovered (been picked up at least once) will be listed here, alongside how many times it has been purchased. To purchase an item or piece of equipment, left click it. The same item can be purchased multiple times. To sell an item or piece of equipment, right click it. Three buttons, labled "Earnt Consumable", "Earnt Persistent" and "Free", are displayed on the bottom right of the interface. Clicking these will allow the player to change the mods mode. The differences of these three modes are detailed below. Another three buttons, labled "Profile: 1", "Profile: 2" and "Profile: 3", are displayed in the bottom center of the interface. Clicking these will allow the player to change the current item loadout. Buying an item in one profile does not effect the others, this is so a player could configure each profile differently to easily switch between them between games. Each of the 3 profiles is unique to each mod mode. This mod can be enabled and disabled from this menu, should the player wish to play normally again. When a game begins the items from the currently selected mod mode and profile will be spawned into the players inventory.

Mode: Earnt Consumable
Players will earn credits for every stage they have cleared. The amount of credits awarded per stage cleared will vary based on the game's difficulty and how it ended (win, loss, obliteration). Players WILL NOT be accredited for any stages completed before adding this mod. Credits will be earnt regardless of the current mode of the mod. Items in the shop interface will have a price associated with them. Buying an item will cost credits, selling an item will refund the full amount of credits. When a game is played while this mode is active the credits that were spent on items will be used up and consumed. The current profile will also have its items removed, they will have to be purchased again with the players remaining credits if they want to be spawned again in subsequent games.

Mode: Earnt Persistent
Players will earn credits for every stage they have cleared. The amount of credits awarded per stage cleared after the mod has been installed will vary based on the game's difficulty and how it ended (win, loss, obliteration). Players will also be accredited for all stages completed before adding this mod, though the amount of credits awarded per stage will be a flat rate uneffected by the diffulties and endings of those previous games. Credits will be earnt regardless of the current mode of the mod. Items in the shop interface will have a price associated with them. Buying an item will cost credits, selling an item will refund the full amount of credits. When a game is played while this mode is active the credits that were spent on items will NOT be used up and consumed. The purchases will persist between games, as a kind of permanent upgrade to the players character.

Mode: Free
Items in the shop interface will have no price, they can be purchased as many times as the player wishes. The purchases will persist between games and will not be reset.

## CONFIGURATION
After a player has opened the item shop interface for the first time a number of configuration files will be created. These can be found at "<RISK OF RAIN 2 INSTALL LOCATION>/Risk of Rain 2/BepInEx/config/Phedg1 Studios/Starting Items GUI/" and "<RISK OF RAIN 2 INSTALL LOCATION>/Risk of Rain 2/BepInEx/config/Phedg1 Studios/Starting Items GUI/<YOUR PROFILE ID>/". If you desire to alter the configuration of the mod it must be done by editing these files. The intention is that this would only be necessary once, with the rest of the player's interactions being done through the shop interface inside the game itself.

Enabled.cfg
This is the record of whether the mod is enabled, so that it can persist after the game has been closed.

Mode.cfg
This is the record of which mode the player was last using, so that it can persist after the game has been closed.

Profiles.cfg
This is the record of which profile the player was last using in each mode, so that it can persist after the game has been closed.

ShowAllItems.cfg
When this file is blank the player will only have access to the items and equipment that they have unlocked and discovered. If anything is written inside this file, they will have access to every item and piece of equipment in the game.

ItemPrices.cfg
Contains the number of credits (in integers) that the different types of items cost, separated by a comma. These prices apply to both the Earnt Consumable and Earnt Persistent modes. These types are, from left to right; tier 1 items (white), tier 2 items (green), tier 3 items (red), boss items (yellow), lunar items (blue), equipment (orange), lunar equipment (blue), elite / hidden equipment (orange). Editing these values will update them in the store.

RewardMultipliersConsumable.cfg
Contains the multipliers for how many credits are earned for each stage cleared based on the games results. From left to right these are: win, loss, obliteration, easy, medium, hard. The amount of credits earned for an medium obliteration game would be  gameStages x medium x obliteration.

RewardMultipliersPersistent.cfg
Contains the multipliers for how many credits are earned for each stage cleared based on the games results. From left to right these are: default, win, loss, obliteration, easy, medium, hard. The amount of credits earned for an medium obliteration game would be  gameStages x medium x obliteration. The default multiplier is used for all stages completed before this mod was installed, the amount of credits earned would be previousStages x default.

CreditsConsumable.cfg
This file contains the number of credits (as an integer) that the player has earnt for the Earnt Consumable mode mode. Editing this file will update the credits in the mod.

CreditsPersistent.cfg
When this file is blank the player will only be accredited for the credits they have earnt in the Earnt Persistent mode. Enter a number of credits (as an integer) to override the number of credits this player has. Internally players will still earn additional credits as they play, but the amount of available credits will not grow, it will stay fixed at the amount entered in this file.

CreditsPersistentAdjust.cfg
When this file is blank the player will only be accredited for the credits they have earnt in the Earnt Persistent mode. Enter a number of credits (as an integer) to augment the number of credits this player has. If the player feels they have too many credits they can enter a negative number in this file, this amount will be subtracted from their total. Entering a positive number will add to the total. The number of credits the player has will continue to grow as they play, this will adjust the total instead of completely overriding it.

CreditsPersistentAdjust.cfg
When this file is blank the player will only be accredited for the credits they have earnt in the Earnt Persistent mode. Enter a number of credits (as an integer) to override the number of credits this player has.

UserStages.cfg
Contains the number of stages (as integers) that the player has completed since the mod was installed, broken into the 9 possible game types. These types from left to right are: easy win, easy loss, easy obliteration, medium win, medium loss, medium obliteration, hard win, hard loss, hard obliteration. Editing these values will update the number of points a user has in the Earnt Persistent mode.

ItemsEarntConsumable.cfg
This is the record of what items and equipment the player has purchased in the Earnt Consumable mode, so that they can persist after the game has been closed.

ItemsEarntPersistent.cfg
This is the record of what items and equipment the player has purchased in the Earnt Persistent mode, so that they can persist after the game has been closed.

ItemsFree.cfg
This is the record of what items and equipment the player has purchased in the Free mode, so that they can persist after the game has been closed.

## Changelog
v1.1.2
Fixed GUI scaling for different resolutions and aspect ratios

v1.1.1
Added a new config file to adjust / augment the amount of credits a player has in the Earnt Persistent mode.

v1.1.0
Now compatible with the Artifacts update.
Updated the visual style to match the new UI.
Increased the scrolling speed of the starting items menu.
Added support for additional difficulties added by other mods, so credits are now earned while playing them.
Fixed a bug where items could not be removed when in the Free mode.
Fixed a bug where unfinished items would show when show all items was enabled.
Decoupled the mod from the base game to a much greater extent.

v1.0.0
Initial release.