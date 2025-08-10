#Changelog
```
v4.3.1
Stat showing what Minion type dealt the most damage
Tooltip for damage stats will show % of Total Run damage was done by that category. (ie 90% done by you, 10% done by minions)
Merc Eviscerate hit overlay effect now skin colored. 

Unlockables moved above RunRecap
Drones get Counted before a final boss instead of run end, to better represent the run. 
(Since often they kill quite a lot of drones)

Simu Stage logs now also visisble by having Void Fiend unlocked. (Some guy got confused)
Fixed Gummy Equipment Drone counting for Drone Collection.
Fixed some issues with Latest Wave Stat
Fixed Survivors with a Ending Quote, but not a Vanish Quote, not using the Ending quote. 
Fixed Item/Equipment tier color config not working.
Fixed Glowing Meteor effect not really being visible on Helminth.
Removed Looking Glass Stat Presets, that is being added over there eventually.
Arti Always in bazaar Config now default false. (Surprised by how many people think its confusing)


v4.3.0
Added Drone Collection
-More preperation for DLC3 where Drones will be treated more like items.
-Will show Drones/DroneEquipment
-Will show DevotedLems/DevotedItems/DevotedEquips


Added DoT Damage stat
-How good was Bleed/Poison/Blight/Burn in your run?
Added Damage Blocked stat (Host Only)
-Armor & Blocked entirely
-Clients do not get original damage values so can't be client side.
--Might remove either stat as they dont seem that impactful on most runs?

Minion Deaths -> Specifically permament deaths (Drones, Turrets, Devotion). 

Message for giving an item to a Lemurian Egg
Message for losing a Devoted Lemurian and what item they had. 
Eggs now count for "Drones Left Behind"
 
Death Loadout now shows Heresy replacements.
 
Inventories on the death screen now automatically use all space available.
-To better fit different screen sizes 
-And also fit the extras I add.

Sorted Blight recolor to as late as possible and default to false.
Fixed an AffixBeadBehavior_OnEnable nullref.
Fixed Most X stats lacking the monster name.
Made EliteBell IL cleaner.
 

v4.2.5
Added Minion Healing Recieved stat
Added Minion Death stat
Missed Chest & Drone stat now have a detailed breakdown of what was missed.
Fixed custom stats not using comma seperators
Fixed Fans counting as missed chests.
Fixed Pillar indicator looking weird
Fixed Most Killed/Hurt stats being able to select hidden monsters.
Fixed unlock area not expanding properly.
Fixed some console spam
Fixed Artifact Reliquary having a Scrapper Icon (???)
Fixed alcyon Shrine. (Happened due to style changes)
Removed Frozen Buff timer because clients have 0 info on the duration so it can't really be client side.



v4.2.0
Death Screen Update
-Most stats now 2 per row.
-New Stats
--How many Items scrapped
--How many Chests left behind
--How many Drones left behind
--How much damage Minions took. (How effective are the meat shields stat)
--How many Lunar Coins used 	(How much are you cheating)
--How many times you Jumped.
--What enemy you killed most
--What enemy hurt you most
-Unlockable section changed to general Run Recap
--Show Stages you went through
---Show off you beat all 3 final bosses
---Or went to Bazaar/Gilded 3 times
--Show Last Simu Wave
-Moved Loadout Stat higher
-Button to open/close Chat area.
--Chat closed by default again for Solo
-Put detailed death message & Victory quotes top right
-Increased size a bit because needed space
 
Added Simu Stages to Log.
-Needed a icon for the stage recap.
-`Unlocked` by beating them once no need to find
 
Chef Oil will now do a small effect when changing states.
Igniting Oil will now play sound effect like freezing.

Scanner icons now get removed upon purchase
Equipments now use wrench icon. 

MidAir Jumps now unlock movement if locked by Geyser.
-Some guy fucking died to Hopoo Feather on Eclipse due to a Geyser.
More skills now unlock movement if locked by Geyser.
-Commando Util
-Ion Surge
-Merc Util
-Eviscerate
-Loader Util
-Void Fiend Util
-Step Brothers
-Oil Spill
-Srides of Heresy

Made Sundered Grove, Abyssal Depths, Scorched Acres shadows slightly less dark by default.
Glowing Meteor effect slightly less dark.
ReAdded Twisteds Fire visual effect
ReAdded Freeze duration buff but client side.
Artificer will always shown in Bazaar as decor, just be unpurchasable if already unlocked.
Broken TC280s will not be snowed on non snowy stages.
Twisteds spawning does a little static False Son sound.
Changed buff icon of +1 to unused more fitting icon.
Multi shops show up as before on Scanner. (Technical issues)
Fixed Ally Ping not outlining most turrets.
Fixed effect replacers not having saftey check.

 
 

v4.1.3
MultiShop ping icon is now 3 chests stacked to differentiate them.
Fixed Engi Turret skin fix not working on Walking Turrets
Fixed Engi colored harpoons being broken.
Fixed Void Fiends Default neck not using correct material anymore.
Added Looking Glass presets just cuz I dont like their default settings.


v4.1.2
Made Prayer Beads+Consumed work properly with Looking Glass
Elite Equipment will now be viewable based on other unlock progression.
- Instead of just relying on the really rare chance to drop one.
- ie Beat game: Tier 1, Clover unlock Tier 2,
- They already didnt count towards progression.
Moved items teleporting if they fall of the map here because it seems fittingly small.
Removed duplicate elite display addition.
Fixed custom item orbs being gone.
Fixed Loadout stat on death screen being broken due to a last minute change.
Fixed Difficulty stat not working proplery with multiple people
Fixed MercInLobby sometimes breaking
Fixed one of the lights not being colored in MercInLobby
Fixed Detailed Death message using damagePostCalc instead of funny big number before OSP (Host-Only)


v4.1.1
Hopefully fixed stage load error.
-The code with issues was making a skin.
-Something about, loading an asset in the new way.
Split bug fixes into own mod.

 
v4.1.0 - Updated for Patch 4

MulT now shows his primary skill in the lobby.
Made Helminth fixed Lighting + Brainstalks not blindingly Red
Added Loadout to death screen at the bottom of the stats
Colossus Captain smooth armor.
Fixed obliteration ending format being wrong.
VanillaFix: Void items dont play sound when dropping.
VanillaFix: Scrapper not making sound
VanillaFix: Chef Boosted Ice Box not being cleared properly.
VanillaFix: Chef Cleaver Bonus having 2.25 proc instead of 1.5
VanillaFix: Railgunner overlay being less see through than in the past

Known issue : Acrid skin does not show up in lobby. Probably will be fixed by R2API updates.


v4.0.6
Replaced some ??? with actual names.
Fixed a mod issue where Phase 4 Mithrix would be immortal if revived by Dios.

v4.0.5
Fixed Prayer Bead Blessing saying BEADS_TEMP_
Blessing text not gets set every time to avoid any issues. (Losing items would often reset the text)

v4.0.4
Made run and lobby chat scrollable.
Asset Bundle optimizations
Pot & Fusion Cell kill icon (very important)
Newt Altar ping icon now Lunar Coin icon.
Added unique Radar Scanner ping icon.
Added config for Old Sots Elite icons that match the other elite icons.
Added Elite Ramp for Twisted Elites. (Vanilla uses Overloading)
Gilded Elites no longer lose their colors on death. (Vanilla shows as Blazing)
Fixed Scoreboard showing disconnected people
Fixed harmless? error for clients when changing equipment
Fixed LUNAR_CHIMERA english being gone.
Fixed Large MultiShop being called Equipment Multi shop, and that not having a name.
Halcyonite Shrine ping hitbox smaller after completion.
Gave PRIMEMERIDIANHEAD_BODY_NAME a name. (I don't think this could ever show up in vanilla)
Fixed Prayer/Blessing not displaying altered text if it wasnt first in the notifcations.
Added proper Plural to global reminder objectives.
Potion/Watch message now global by default.
Moved Kjaro/Runald being named here. (from LGT)

 
v4.0.3
Prayer Beads stuff
Put Newt instead of NewtAltar in the Bazaar Log so you can stare at him.
Fixed Halcyonite Shrines draining gold^2 faster than intended due to a Client fix running on Host.
Fixed? issue with mods that delete Newt Altars.

-4.0.2-
Sorted Bosses to end of Monster Logbook
Fixed wrong name being used to detect ExtrasMod, leading to wrong prayer beads getting the stat overlay

-4.0.1- 
Message for Sale Star, including Interactable it was used on.
Message for Recycling. (requested)
Void Fiend & Chef Boosted skills will be referred to as such.
Void Fiend Corrupted skills now have actual descriptions.

Green Merc Expose less bright
Fixed HostHasMod detection leading to Clients sometimes having duplicate mod messages.
Fixed wrong link in ReadMe
Fixed accidental removal Russian and German
Fixed assets not loading if downloaded manually


-4.0.0-: Split
Made entire mod Client Side, allowing use with people who do not share it.
Everything that couldn't be made Client Side will be in an Extras mod.
The other mod will NOT be downloaded automatically.

Moved the following Content:
-All informational buffs
-Consumed Keys & Prayer Beads

Config Reset, All config ingame via RiskOfOptions
Added various fixes as dependencies.


Helminth Lighting fix
Made a new Sprint UI, less intrusive than the previous. Same function of allowing "Spread" and "Charge"

Shrine of Shaping will now display a line in chat when used. (Like other shrines)
Shrine of Shaping will now play the shrine effect and sound on all players.
Shrine of Shaping and Seed of Life now use the Dios revive effect. (Seed is Serve Side)
-Instead of failing to spawn something unfinished, or nothing at all.

Made Item Reminders update/clearing Client sided.
Made Portal reminders clearing Client sided.
Made Mountain Shrine TP-Symbol Client sided.
Made Victory Message now Client sided.
Made Halcyon Charge objective updating Client sided.
Made Detailed Death Messages work without Host having mod.*
Made Killer Inventory work without Host having mod.*
Made Item Loss messages work without Host having mod.*
Made Scrap messages work without Host having mod.*
*Uses work arounds, hopefully doesnt display anything wrong, cant test well for net-lag.

Mission Pointers :
-Void Fields will show position of next cell you need to travel to.
-Commencement will briefly show positions of uncharged pillars after charging one.
-Gilded Coast will briefly show positions of unbought Beacons for the last 3
-Can be turned off whenever

 
Void Potential & Aurelionite Fragment
-Now have tiered particles like items  (Moved from SimulacrumAdditions)
-Show their Items in chat when Pinged  (Moved from SimulacrumAdditions)
-False Son now drops a Green or Red fragment.
--(Fixes Command if Host, else for Particles & clarity)
-Fixed vanilla bug where they don't spin for Clients
-Fixes Void Command essence not having particles  (Moved from VanillaArtifactsPlus)


Equipment Drone Equipment Name will now update with Enigma

ReRendered mod body icons with official icon rendering.
Ally Aurelionite will now have a blue outline too.
Halcyon Shrine will now have unique ping icon instead of Cube

Gameplay fixes:
-Prismatic Trial avaiable (Moved from LittleGameplayTweaks)
-Primordial Teleporter Destination can now be changed even after finishing it. (Host)
-Acrid invul during spawn
-Merc M2 fall damage fix
-XI construct laser fix

Pinging a Player will now be blue
Added option for Newt Altar reminder. (Some of you really need smth better to do each stage)

Added Elite Displays for XI Construct.
Added Perfected Displays for Sots Monsters.

Message for when someone uses Dio/VoiDio/SeedOfLife

Tab Scoreboard now shows dead peoples inventory too. (Why would they not allow this in vanilla??)

Scav Pickup message now mentions their Elite Type

Bazaar Storm Secret Mini Geodes now more noticible (Might be Server Side?)

If ServerMod not installed:
-Prayer Beads will show a transformation message with the stats. (But can't check stats afterwards)

Moved Sulfur Beetle Skin ReImplementation here (ClientSide now)(from LittleGameplayTweaks)

Sale Star effect now shrinks instead of vanishing upon buying.


Hopefully made ping icons for interactables part of stages more reliant for clients
Fixed Secret Geode Reminder not working on clients

Fixed Newt Altars being purchase able after Teleporter, or when Teleporter starts with Blue Orb.
Fixed new tokens for interactables being an issue if not everyone had the mod.
Fixed Titan pinging the particles instead of the body.
Fixed War Bonds playing sound even if you have 0 Missiles.
Fixed Prayer Beads stats often desyncing on clients.
Fixed Engi Spider Mines being loud as fuck and constantly beeping on clients

Switched to using R2API_Colors instead of own implementation
EffectCatalog trickery to make added effects work without being seperate indexes.
ProjectileGhost replacing instead of replacing entire Projectiles. (Always shoulda done this tbh)


```
### Pre ClientSided - RequiredByEveryone Split
```

v3.2.9
Fixed missing strings because I forgot to update the language files.
Regen Scrap reminder gets cleared when bosses start.
Regen Scrap reminder only appears on normal stages now.

Fixed chest reminders not spawning on Meridian anymore.


v3.2.8 - 
Fix for 1.3.7 and other stuff I was working on before.
Added config for individual Reminders. (Key, Shipping, Sale, Geode)
Added config for Regen Scrap reminder. (Off default)
Made "Chat always on death screen" it's own config.
Fixed issue where ArtifactWorld wouldn't spawn interactables if travelled to with commands.


v3.2.7 - Patch for 1.3.6
Consumed Equipment now have a grayer-orange color.
Made buff for Unstable Transmitter duration visible.
Removed extra line when proccing Chance Doll. (Official replacement)
Updated SotS elite aspect descriptions to match their new effects.
Moved "Burns ending all DoTs" bug fix here.
Moved "War Bonds untextured handles" bug fix here.
Added config to allow some buffs to work with nectar. (Disabled by default)


v3.2.6 
Added Russian Translation 
Added Config for objective pannel spacing.
Added Config for objective pannel font size.
(Can be changed mid-game via Risk of Options)

Made elite Children more distinguishable
Fixed Sale Star reminder not showing up in Simu.


v3.2.5 : Forgot there were Voids that eat multiple items and left a debug thing on whoops.
v3.2.4
If you pickup a void or a normal item if you have the void it'll show the quantity you'll have post corruption. (ie had 3 Bear, Safer Spaces(4) in pink)

If rusted becomes crusted or gets scrapped the reminders recheck how many rusteds are left compared to the reminder.
If sale star is scrapped reminder fails.

Fixed Sale Star reminder not getting cleared on Client.
Fixed Hosts Sale Star reminder being cleared by Clients.
Fixed Halcyon Charge Objective not updating on Client.


v3.2.3
Added colored Engi Harpoons to the alt skins as per request.
Fixed item loss messages not using correct token for second person.
Fixed item loss and detailed death messages having First/Second person reversed.
Fixed item loss messages getting the body name instead of the user name.


v3.2.2 - Quick Fix for 1.3.5
v3.2.1
Fixed Shipping reminder not being cleared.
Fixed part of the expanded death screen not being disabled with the config.

v3.2.0
Added Config to try and make mod able to be used with Clients/Hosts that do not have a mod
-(This of course means the mod is no longer tagged as "RequiredByAll")
-Features that will be disabled would includes Buffs/Items/Projectiles/Effects added by mod.
--This is because they all have an id/index. Different amounts of ids cause desyncs.
--This does mean Skin changes will be disabled. I can't realistically change that.
-Various features might not work properly if you're a Client with mod can't really do much about this either. 

Added Risk of Options support.
Added Language Files, so translations are possible.
Moved AssetPack out of dll for optimization.
Moved all images to AssetPack.

Added unique icon for Rebirth win.
Changed delayed green orb message so it doesn't show up full screen with MSU sometimes.
Added config for Lunar Seers stage name in display
Fixed menu selector not actually setting copied weather to active.
Fixde "Trial of ArtifactName" Objective not being in new artifact worlds.
Fixed Sale Star not working on Stage 5s. 
Fixed an issue with Blight Orb trails sometimes disappearing.
Fixed/Reenabled Elite Brass balls.

-Needed to change a fair amount of stuff with assets and strings so some things might be broken.


v3.1.9
Fixed Blight Acrid skin being black and not having mesh replacements set.
Main Menu selector config as per request.

v3.1.8
Green/Purple orb messages are now delayed by 1s so that they open chat box. (Shrine of Halc)
Eclipse display now automatically disabled if you have other Eclipse Display mod.

v3.1.7
Added a number displaying beaten eclipse level during Eclipse character selects.
Added a void outline for if having beaten Wave 50 on a character during Simu character selects.
(Bit function over form but it's usefull, can be turned off if undesired)

Equipment Drone Names now update properly on equipment transformation.
Fixed Sale Star reminder only working on stages it's not supposed to.
Fixed skin textures added by mod not being able to scale down.
Fixed ping icon with Verdant Falls guaranteed interactables.
Disabled Brass Elite Balls because changes to the effect system don't really allow for this. (Until they fix it)

v3.1.6
Added config to remove Scav/Gup on title screen.
Added friendly-outline to Devoted Lemurians

You won't get more Rusted Chest reminders than keys.
-If Devotees spawn 17 Rusty chests, but you only have 2 keys. You only have a reminder for 2.

Fixed bug where Devoted Lemurians are in the log instead of Wild ones. (Vanilla bug)


v3.1.5
Fixed SS2 interactables not having ping icon assigned anymore.
Doubled range at which Sale Star effect spawns.

Hopefully fixed issue with Prayer Beads Blessing having really long numbers sometimes.
Reminder for VanillaVoid Cornucopia
Made BlueTP objective disabled by default.
Fixed KipKip being named TwipTwip


v3.1.4 - Requests
Made Prayer Beads Blessing tell you how many stats you get in the full descrption.
Prime Meridian tells you how many Geodes are left to crack for the secret aurelionite fragment.
Saftey checked Acrid Blight stuff for mods that reuse Acrids parts.
Treasure reminders now get marked as failed when Mithrix/False Son fight starts & Voidling Phase 1 dies.


v3.1.3
Added Halcion Shrine charge percentage. (Automatically disabled with NoMath mod)
Added Unique line for when Chance Doll activates.
Added Prayer Beads (Blessing), to show you how much of a bonus you got. 
(The item notification and description tell you how many bonus levels you got from all blessings.)
Made the previous Red Printer ping icon the Green Printer one. Red Printer now has a more unique icon.
Death messages for Glass, Twisted and Echo conditions.

Removed Sale Star reminder for non-standard but timed stages. (ie Moon, Planetarium)
Fixed more guaranteed interactables using wrong interactables. (Verdant, Impact)
Fixed Blue Tp description not working multiple times.


v3.1.2
-Mod loads later for hopefully better compatibility with other mods that change strings.
(Changed name from com.Wolfo.WolfoQualityOfLife to just Wolfo.WolfoQualityOfLife)
-Made Opal/Shield cooldown buff get applied differently to support modded Warped Echo.
-Tagged used Keys as consumed.
-Fixed issue with previous blue tp objective.


v3.1.1
Added a objective reminder for Sale Star (I forgot I had this item so many times)
Made the Sale Star effect bigger.
Slightly less spacing between objectives so the list gets slightly less long.
Primordial TP objective text is now colored blue.
Teleporter Icon when the "Discovery" setting is enabled now start off as light-red.
 
Fixed Chests in Gilded still having loot bag icon. 
Fixed Rallypoint fans using vanilla Chest icon.
Fixed vanilla bug where Chance Dolls effect uses an invisible color.


v3.1.0 - Green Merc update
Added Green attack effects to Colossus Merc skin and skins ending in Green.
Merc Oni backup skin now disabled by default.
Sorting for Oni Backup skin should work properly again.
Fixed Colossus Engi Skin having the same problems as Mastery Engi.
Fixed a bug with the mod causing Colossus Engi Turret skins to be overwritten.
Gave Colossus Rex better Vine colors. (Automatic one looked pretty whack)
Fixed vanilla bug where half of War Bonds is pure black
New Elite Equipment proper item sprite, pickup quote and description.
Elite equipment are now sorted after Equipment. Shared Design is now sorted with the rest.

v3.0.0
Updated to Seekers of the Storm
-Buffs added by this mod don't contribute toward Nectar

v2.5.9 - (Unreleased)
Added icon for Egg 
Fixed vanilla bug where Chests show loot icon
Fixed Lunar enemy lore not displaying due to the name change.
Fixed strange issue involving Sawmarang infinitely duplicating.

v2.5.8 - Fixed storepage image being gone due to Discord.
-Gave Void allies cyan eyes for easier identifaction.
-Made Stomp/Freeze buff not get added when Risky Mod is loaded as they add their own.

v2.5.7
More various fixes for minor network oddities. (Equipment Drone names, Shock Beacon visible Radius)
-Moved backup Blue Sword Oni Merc to the end of the skin list and added config to disable it.
-Fixed an issue with mods using red merc effects.
Attempted fix for vanilla bug where Multishops would sometimes look closed for clients.

v2.5.6
Removed buff order manipulator because it seemed to cause issues for people.

v2.5.5
Fixed Blight Contagious Trail not being Blight colored on Clients
More ExpandedDeathScreen fixes
Loader Pylon will match the skins color again
//Moved Opal Cooldown buff next to Opal Ready//

v2.5.4
Added missing saftey check related to feather buff which could cause desyncs

v2.5.3
SimuAddtions Red Merc support
ReAdded Scrapping messages cuz I like much info. (configurable of course)
Lunar Coin amount backdrop is blue instead of pink

-Should be more consistent on Clients : 
--Equipment Drone with Equipment Names
--Portal Reminder messages 
--Feather buffs being not properly synced


v2.5.2
Fixed Brass Balls not getting elite skins on clients
Fixed Expanded Death Info not working in multiplayer when dying multiple times throughout a run.
Fixed Blight Acid Pool being a wrong projectile if used by Clients.
Elite Equipment won't be in the logbook if ZetAspects is enabled.

v2.5.1
Fix Text config not working.  
HistoryFix compatibility.   
(This mod does what that mod does anyways so i'm not sure why you'd have both)  
Watch message again and VV watch message.  
Loader hook fist changes with skin again.    

v2.5.0 - Cleanup  
-IL Code hopefully making it cleaner  
-Networking fixes  
--Messages are now subjected  
--Sometimes random stuff like Lockboxes having messed up visuals  
--Killer Inventory  
--Treasure Reminders  
--Red Merc Expose  
--Feather Buff not working on Clients   
--Extra Mountain Icons  
-Main Menu theme randomizer
-Death Messages are now one color and show up before the normal death message  
-Shield/Opal cooldown buffs won't show up on enemies  
-Abyssal Geyser  
-Void Highlights  
-Updated Printer Icons  
-Item Names Colored in Pings  
-Mod Support for SpikeStrip, Starstorm and VanillaVoids  
-Removed Goo River in Aquaduct  
-Removed Vagrant Predictor  
-Moved GameplayQoL to LittleGameplayTweaks  
--Slightly Faster Interactables   
--Married Elders using Bands  
--Prismatic Trial stuff   
--Random tiny bits  


```
## Really Old Changelog:
```
v2.0.5 - Updated for 1.2.4.1\
* Removed Lysate Cell Captain feature due to different official implentation
* Removed Void Allies having blue/green looks due to different official implementation

v2.0.4 - Bug Fixes\
v2.0.3
* Updated for version 1.2.3
* Vanilla Fix: Run History deleting essentially random runs instead of the oldest.
* Bug Fixes

v2.0.2
* Bug Fixes
* Regarding Buffs not showing up : Since i've heard mixed things, it works fine for some people and not for others, trying some generic fixes like resetting the config or using pre launch fix might help but I'm not sure. Just as always when reporting bugs send a log file.

v2.0.1
* Config for Lysate Cell Huntress stuff
* Config for Lysate Cell Captain stuff
* Config for Sprint UI changes
* Bug fixes

v2.0.0
* Updated to Survivors of the Void
* Blighted Default Acrid Skin and Blue Sword Oni Merc as seperate Skin
* Pings dont disappear over time anymore
* Lunar Seer Info QoL from my Artifact mod is now here too
* Lysate QoL for Huntress Ballista and it working for Captain
* Info Messages for Elixir, Delicate Watches, Benthic Bloom and Egocentrism
* Objectives for Portals, Lockboxes, Shipping Deliveries and more.
* Void Allies from Newly Hatched Zoea are now more Blue/Cyan/Green colored.

v1.6.5
* Moved Price Changing stuff, Boss Drop percentage to LittleGameplayTweaks

v1.6.4
* Allies can't steal Healing&Bandolier pickups anymore.
* Lepton Daisy appears on Pillars/Cells
* Visual fixes for Deskplant & Rachis
* Moved Family Event stuff to LittleGameplayTweaks
* Moved Beads and Convergence changes to LittleGameplayTweaks

v1.6.3
* Config to disable Third Seer/Commencement Seer (Commencement Seer disabled by default now)
* Fixed weird Tsunami incompatibility

v1.6.2 
* Oni Merc has red effects now
* Lots of touch ups didn't keep track
* Mountain Shrine icon stacking

v1.6.1 - Accidentally left testing stuff in.\
v1.6.0 - Fixes
* If the Killer has passive items, the Killers items and Equipment will be shown on the death screen

v1.5.9 - Fixes\
v1.5.8 - Fixes
* Beads of Fealty stacking

v1.5.7
* Third Lunar Seer
* Win messages will also be displayed in chat like death messages
* Small other fixes

v1.5.6
* Prismatic Trials stuff
* Rex attacks will now try to be correctly colored (Leaves, Vines)

v1.5.5
* Added ItemDisplays for all enemies for Shared Design(Lunar Elite) for PerfectedLoop/FixedSpawnDissonance
* Added ItemDisplays for normal elites for Engi Turrets & Lunar Chimera & Mithrix (vanilla elite only)
* Added ItemDisplays for Fuel Array for Engi Turrets
* Acrid Blight will now affect the looks of some attacks (if you have suggestions on how to make it look better please ping me)

v1.5.4
* Moved around and fixed up Family events where deemed necessary 
* Added new Clay & Solus Probe/Vulture & remade Parent Family event
* Elite Brass Contraptions have colored Balls
* Void Fields and Elder Lem tweaks

v1.5.3 - Fixed up alt skin Engi Turrets to have proper glow.\
v1.5.2
* Menu Theme config
* Equipment will be shown alongside items on death screen.
* Picking up a Boss Item now shows a yellow highlight instead of white
* Picking up a Equipment now shows a highlight
* Touched up some skins.

v1.5.1
* Ability to increase amount of White items from RedToWhite Cauldron (under price changer)
* All drone prices can now be changed.

v1.5.0
* Renamed Mod to more accurately reflect what it is. (and to hopefully get more traffic and feedback)
* Organized Config

v1.4.1
* More buff icons
* Hopefully fixed networking

v1.4.0
* Distant Roost now can't spawn without a Newt Altar.
* One Lunar Seer after Skymeadow will show Commencement.
* Ability to change Cost of TC Drone, Healing Shrine, Gold Shrine.
* Primordial Teleporter unique icon
* Equipment Drones use equipment more often

v1.3.9 - Bug fixes
* Description for Aspects, Fuel Array, Tonic Afflictions.

v1.3.8 
* Headstomper Buff Icons like Elemental Rings
* Feather Buff Icon for extra jumps
* Shield Regen Delay icon (Medkit icon)
* Config to change names of Lunar Chimera
* Added Consumed Rusted Key

v1.3.7 - Quick missed fix\
v1.3.6
* Acrid is intangible while sleeping.
* Fix LunarExploder not using subtitle, Pot/FusionCell using ? instead of PlanetDeathIcon. Unique Icon for Soul Wisps.
* Swamp Altar Skeleton will always be there and option to do the same for Locked Artificer

v1.3.5 - Minor Tweaks
* More buff visual config

v1.3.4 - Fixes
* Changed color of buffs that use same icon/color as other buffs. (ie Cloak Speed, Whip Speed)

v1.3.3 
* Tweaks to Limbo Ending
* Config to make Lunar/Boss equips use Lunar/Boss droplets instead of Orange droplets.
* Unique Icons for Empathy Core Probes, Updated Beetle Guard Ally and Missile Drone Icon

v1.3.2 - Hopefully more optimization\
v1.3.1 - "Quick" Lid position fix\
v1.3.0
* Debuff Icon added for Hellfire tincture. 
* Config to invidually change the Printer model to the old ones.

v1.2.8
* Unique Icon for Engineer Walker Turrets

v1.2.7
* Option for more Logbook entries
* Added more Ping Icons.

v1.2.6 - (actiually disabled by default)\
v1.2.5
* Module to change color of Lunar/Elite equipment if you want Yellow Elite Equipment or any unique color for either. (Disabled by default)
* Added more Ping Icons.

v1.2.4 
* More Icons & Config
* Twisted Scavengers now hold Beads of Fealty

v1.2.1 - 1.2.3 - Minor Fixes\
v1.2.0
* Added more Ping Icons

v1.1.2 - Minor Fixes?\
v1.1.1 - Made mod slightly faster

v1.1.0
* Added or Updated Ping Icons for many interactables
* Added Cost Hologram for Lockbox, Cleansing Pool, Broken Rex
* Added Position Indicator to Void Field Cells

v1.0.0 - Release.
```
```
v5.0.0

Drone buy message including count of drone
Drone upgrade message
```