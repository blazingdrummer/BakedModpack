## Changelog:
```
v1.1.17
Fixed log spam when using Sawmerang
Fixed Ice Spear fix not actually going through due to wrong config val.
Fixed Broken Flame Drones often clipping into the ground, sometimes being barley visible.

v1.1.16
Fixed an issue with my custom droptables and disabling DLCs.

v1.1.15
Fixed various objects on Helminth not being pingable due to missing Null Check.
Fixed mod unintentionally disabling Empathy Cores, Voidsent, Singularity and Ego for Phase 4 Mithrix.
Fixed evolving quantum state lemurians not actually working.

v1.1.14
Reverted Lunar Ruin fix because it made Ruin from lightning not get removed by geodes.
Warped Echo OSP fix now gives you 0.1s of invul like regular OSP.

v1.1.13
Fixed Lunar Ruin counting as 2 debuffs.
Fixed Elusive Antler not working on Devoted Lemurians (Wrong Auth Check)
Fixed Elusive Antler producing errors instead of working on Stationary Turrets (Missing NullCheck)
Tagged Unstable Transmitter as Healing (Barrier Items are all tagged as Healing)


v1.1.12
Fixed WEcho always bypassing OSP
Fixed Bazaar being able to select 2 Plains or 2 Roosts
Fixed a mod nullRef with HealthComponentToTransform

v1.1.11
Fixed missing orig() making only Eclipse count as wins.

v1.1.10
Fixed an issue with the way I added some bodyFlags

v1.1.9
Fixed Warped Echo ignoring Armor entirely.
Fixed Warped Echo not putting you into danger
Fixed Milky Chrysalis not doing it's flight animation due to mod.
Removed my Grandparent Rock fix that was too small and just added someone elses.
(This is technically fixed in vanilla, the rock is just 60x too small)


v1.1.8 : Part of mod was no longer running on accident
v1.1.7
Fixed Boosted Sear Oil Pools dealing 0% damage instead of 20%
Fixed Simulacrums Fog damage being far lower due to unrelated Void Fields balance changes and it being left forgotten.
Removed Chance Doll from Simulacrum as there are no Shrine of Chance. (If SimulacrumAdditions not installed)
Fixed Treeborn Canopy and Helminth Hatchery being blacklisted from RandomStageOrder
Fixed NegativeRegen not triggering OnDeath effects. (Happiest Mask would never trigger Ice/Mending OnDeath)


v1.1.6
Fixed REXs flower vine effect disappearing too soon.
-Should fix like 3-4 other effects but less noticible.
Fixed Grandparent mini rock being invisible.
Fixed Charging Father Laser spawning a Red line at 111,8,68
Fixed Halcyon Shrine often not having its tip golden.
Double checking for certain skin fixes.

 
v1.1.5
Fixed Boosted Cleaver proc to also be 1.5 

v1.1.4
Phase 4 fix is now off by default due to feedback.
Moved Gilded Corpse blazing fix here
Devoted Lemurian Log fix actually moved here.
Fixed Credit Card failing if you buy multi shops too quickly. (Because hopoo gave it a 0.1 cooldown for no reason)
Fixed Captain Beacons never critting
Fixed Eclipse not incrementing the Win counter.
Fixed some equipment displays added by mod not being present with SS2. 
Fixed Boosted Oil Spill description being gone (for english anyways)
Fixed Chronic Expansion on corpses constantly nullreffing
Fixed REX Syringe impact sound being gone. (Unexplainable)
Fixed some more item descriptions
Fixed Nkuhanas Opinion being too zoomed out
Fixed Ice Spear knocking enemies around due to being on wrong Phys Layer.
Restored Glass Mithrix skin


v1.1.3
Fixed the following no longer slowly appearing in their spawn animation, leading to it looking really ugly in some cases.
-Child
-Parent
-Vagrant
-Lesser Wisp
-Greater wisp
-Lunar Wisp
-Void Reaver
-void Devestator
-Voidling
-Engineer Turret
-Engineer Walking Turret
-XI (technically...)(his body is too broken to use it properly)

Fixed Charged Perferator rolling Crit instead of inheriting.

Added Helminth Tunnel fix as dependency
Added Gilded Chunk lag fix as dependency

v1.1.2
Added some config to bugs people are attached to.
Config will be in game If RiskOfOptions is installed.
Fixed Alpha Constructs from Defense Nucleus not using their unique skin
Fixed XI Construct laser not exploding at end as miscFixes removed it.


v1.1.1
Fixed latest patch breaking multiplayer with non mod owners due to Suppresed Scrap implementation.
Moved fixed Diebacks Mushroom fruit not being implemented correctly

v1.1.0
Fixed Warped Echo negating Eclipse 8 curse entirely.
Fixed Sawmerang projectiles not inflicting Bleed without the equipment.
Milky Chryslis being active will always have wings, regardless if you change or lose the equipment.
Fixed Path of Colossus stage skip.
Fixed Railgunner scope transperency being applied twice to one scope.

Moved from VanillaArtifactPlus :
- Artifact of Glass not making you glass.
- Twisted Elites not giving players and some enemies armor.
- Swarms + Vengence spawning 1 Umbra + 1 Enemy survivor
- 11 Devotion bug fixes.
Devoted lemurians now actually tagged as such.
- Means they spawn with a different sound
- - The check for that is also bugged, so that's another fix.
- Means they work with Spare Drone Parts
- - This is just intended.

Moved from SimulacrumAdditions :
Void Suppressor fixes
- Scrap being untiered
- Disappearing too close at camera
- Hud being too small
- Item being randomly too small



v1.0.1
Fixed Broken Scrappers due to a saftey check going missing in the transition.
Mod will now be where I do ItemTags and EliteDisplays

v1.0.0 
Split from WQoL
Moved some Simu fixes from SimuAdds
Children immune to the Sun