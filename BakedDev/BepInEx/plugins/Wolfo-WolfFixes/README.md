Various bug or overseight fixes that I found.
 
Better to keep it bundled in it's own mod

Some fixes are Server Side, some are Client Side, some are Client Specific. Generally recommended for everyone.

#
### Fixes the following :

## Survivor Fixes
Chef Cleaver Bonus Proc being 2.25 instead of 1.5.\
Chef Boosted Ice Box not clearing properly.\
Chef Boosted Sear Oil Puddles dealing 0% instead of 20% damage.\
If OilSpill is cancelled, brief fall damage immunity is maintained.

Mercenary sometimes breaking his legs with M2.

Artificers Ice Spear throwing enemies around.

Acrid not having spawn invulnerability.

Captain Beacons being unable to crit.

 
## Monster Fixes
Child being burnable by the sun.

XI Construct Laser not exploding at the end.
 
(Off by default)\
Mithrix Phase 4 being skipable because the game thinks he has 0 health.

## Item Fixes
Corrects various wrong item descriptions.

Warped Echo ignoring Armor.\
Warped Echo ignoring OneShotProtection\
Warped Echos first hit being ignored if OSP was triggered.\
Warped Echos first hit no longer putting you into danger.\
Warped Echo no longer inflicting Eclipse 8 curse.

Elusive Antler producing an Error instead of working for Stationary Engi Turrets.\
Elusive Antler not working on Devoted Lemurians due to wrong check.

Happiest Mask Ghosts not triggering OnDeath effects. (Ice Explosion, Healing Core, Malachite Urchin)

Charged Perferator rolling for crit instead of inheriting like other procs.

Some item tags were changed.
- Hunters Harpoon missing OnKill.
- Bison Steak still being OnKill.
- Planula still being Damage.
- Infusion & Nkuhanas AIBlacklisted

## Equipment Fixes
Back-Up Drones not scaling with ambient level like other drones.
 
Executive Card no longer fails if buying multi shops really quickly.

Twisted Elites not being able to give armor to some enemies and all players.

For Retool, Enigma, Bottled Chaos
- Sawmerang not bleeding if you don't have the equipment.
- Milky Chrysalis flight will always have wings.

## Misc Gameplay Fixes
Simulacrums Fog ramping up 25x slower than what is intended.

Removed Chance Doll from Simulacrum, as there are no Shrine of Chance. (Unless SimulacrumAdditions is installed)


Being able to skip right to Prime Meridian by entering 2 portals at the same time.

Newt Altars will no longer purchasable after Teleporter. (Like pre SotS)\
Newt Altars will not be purchasable if Teleporter starts with Blue Orb.

Bazaar Seers being able to select 2 Plains/2 Roosts.

Fixes Vengence + Swarms spawning one of them as not an Umbra/Without any items.

Fixed 10 bugs or errors with Artifact of Devotion leading to :
- Lemurian evolution no longer results in all but 1 Lemurian having less items than intended.
- Lemurian wont randomly lose item effects such as Opal, Focus Crystal, etc.
- Lemurians gotten from Trials will be able evolve into elites.
- Lemurian evolution wont fail anymore if 1 or more Lemurians are in a quantum state.
- Lemurian inventories get properly deleted on all run ends.
- Devoted Lemurians now being tagged as such.
- - Different spawn sound + Works with Spare Drone Parts. (Yeah that's intended)
- - They just put it on the normal Lemurians instead of the Devoted ones.


Treeborn Canopy & Helminth Hatchery being blacklisted from Random Stage Order.

## Client specific fixes
Prevents Halcyon Shrine entityState nullref on Client.\
Removes the log spam from Halcyon Shrines on Client.

Aurelionite Fragments & Potentials now spin for clients.\
Prayer Beads desyncing for clients, leading to various issues.\
Spider-Mines constantly beeping for clients

Simulacrum teleporting Clients into the void instead of the Focus.\
Simulacrum not pointing out enemies at the end of waves for Clients.


## Visual
Adds various missing item displays :
- Perfected Elite Displays for all Monsters
- Elite Displays for XI Construct, Mithrix.
- Fuel Array Display for Engineer Turrets.
 
Fixes some monsters not slowly appearing during their spawn animation:
- Child, Parent
- Lesser, Greater, Lunar Wisp
- Void Reaver, Devestator, Voidling
- Engineer Turret, Walker
- Vagrant

Defense Nucleus Alpha Constructs no longer being Gold.

Gilded Elite corpses no longer look like blazing elite corpses.

REXs flower vines disappearing quickly

Mercurias Rachis visual radius not matching the actual buff radius.

Deskplant Visual being made too small after being too big.

Railgunners Scope being more opaque than in the past

Void Command Essence not having particles.\
Deep Void Signals Beam being flat.

Shrine of Shaping and Seed of Life not using the revive effect. (Instead of failing to spawn a unfinished object)

Artifact of Glass will now make you and minions appear as glass.

Stone Titan pinging the particles instead of the body.\
Mithrix Hammer/Nothing pinging instead of the body.

Lunar Exploder not having a subtitleToken.

Halcyon Shrine often not having its tip golden due to a redundant check.

Broken Flame Drones often spawning in the ground.

## Audio
Void items not playing the drop sound.\
Scrappers not playing sound.\
REX m1 not playing impact sound.


War Bonds should no longer play the Horn if 0 missiles would be fired.

Scavengers not playing their Spawn Sound

Soup not playing their Soup sound

## Misc
Log Fixes : 
- Eclipse not incrementing Wins / (Thus not unlocking logs)
- Bazaar Diorama being empty
- Sulfur Pools Diorama having a red base.
- Void Locust Diorama, Void Devastator being too zoomed in.
- Nkuhanas Opinion being too zoomed out.
- Devoted Lemurians being in log instead of wild.
 

Adds 'simu_softlock' softlock command to forcefully end wave and start next, or otherwise spawns Portal.

Green Orb message will now pop up as you load into the stage so you can actually see it.

NullRef from Corpses with Chronic Expansion

Golden Diebacks fruits not dropping healing orbs or playing effects.

Regenerative Scrap being scrapable

Invincibility and Chef Boost showing stacks of the buff.

Item/Survivor description fixes can be turned off in case you play with rebalance mods.\
But should work fine even if you don't.
 
## For Other Mods

Glass Mithrix is Glass again instead of naked.

Void Eradicators are less unfinished:
- Enables some particles
- Adds price transform
- Item models wont randomly be shrunk down a ton.
- Doesnt vanish when too close to camera
- Suppresed Scrap is tiered and usable, but kept hidden from log.
- Suppresed Items tab wider so item icons arent clipping

Multiple of my mods have Perfected nonLunar enemies or add Void Suppressors and rely on better AIBlacklist.\
But those changes dont affect vanilla much, if at all.

## Commands
 
Testing Commands
- scanner | Radar Scanner equip + 100 BoostEquipRecharge
- godenemy | Sets enemy level absurdly high making them basically unkillable.
- goto_boss | Teleports you to Mithrix/FalseSon/Teleporter
- no_interactables | For clean stage screenshots.
- evolve_lemurian | Evolves all Devoted Lemurians.
- set_damage | Set damage.
- set_health | Set health and disable regen
- Various list_ commands



Report bugs to @Wolfo.wolfo in the Risk of Rain 2 discord or RoR2 Modding discord.\
If you're reporting a bug that isn't something obvious include the log file.





