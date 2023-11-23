# Nemesis Rising Tides

Reworks and rebalances [Rising Tides](https://thunderstore.io/package/TheMysticSword/RisingTides/) elites that keeps the core functionality but with different execution. Ideas funded by the community (but mostly me still). Individually togglable. Not affiliated with starstorm despite its name. Also adds 2 new(ish) elites.

Also try: [Nemesis Spikestrip](https://thunderstore.io/package/prodzpod/Nemesis_Spikestrip/)

## T1: Magnetic Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483503826047036/texAffixMoneyBuffIcon.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482899317792768/20230720155826_1.png)
- Magnetic Elites will now create a zone that grants a buff to all nearby enemies. Getting hit by any of the enemies in the zone will sap money from you. This change is intended to screw melee less. Setting the zone to 0 will only apply this buff to the elite itself.
- Killing a magnetic elite will give more money based on the currently alive enemies in that area.
- Replaces On use with an explosion that saps money from all the enemies hit.

## T1: Oppressive Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483503050109008/OppressiveBuff.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482897052868608/20230720154746_1.png)
- **NEW**: Magnetic elite's on hit effect as a separate type.
- Creates a small cylindrical area that increases gravity around it. On hit, disables jump completely for a short period.
- On use: Forcefully drop enemies around you.

## T1: Buffered Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483502819430460/BufferedBuff1.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482897858183168/20230720155205_1.png)
- **NEW**: Barrier effects from Bismuth elites as a separate type.
- On hit, gains damage as barrier. When barrier is active, take less damage and no knockback. Barrier does not naturally decay.
- On death, give nearby enemies barrier.
- On use: gain barrier.

## T2: Nocturnal Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483504295817226/texAffixNightBuffIcon.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482899665924177/20230720155955_1.png)
- Upgraded to Tier 2 - Now renamed to **Anglesite** elite, on top of the existing effect, increases attack and movement speed to all enemies nearby. 
  - **UPDATE Rising Tides CONFIG!**
  - Health Boost Coefficient, Damage Boost Coefficient should be adjusted to fit T2 stats.
- On-use invisibility will now only trigger if a player uses it - effectively removing it from the enemy.
- Blind effect is replaced by the [Artifact of Blindness](https://thunderstore.io/package/HIFU/ArtifactOfBlindness/) version.

Yes this is literally [WRB](https://thunderstore.io/package/TheBestAssociatedLargelyLudicrousSillyheadGroup/WellRoundedBalance/) Celestine. I'm stealing my own code again :trollshrug:  
(**Disable WRB Celestine changes** if running with this for Double Celestine Moment - its actually quite fun)

Alternatively, you can disable the "zone" and have just the blind effect for T1 (configurable)

## T2: Aquamarine Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483504056750131/texAffixWaterBuffIcon.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482898621542430/20230720155541_1.png)
- Instead of being immune to damage, now releases a zone where every 3rd hit against the enemies in that area becomes nullified. This makes the debuff negatable by focusing on the elite first rather than being Plated Elite 2.
- Bubble attack is unchanged.

## T2: Bismuth Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483502509035530/BismuthBuff1.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482898172747776/20230720155351_1.png)
- Added a configurable debuff blacklist.
- Removed barrier related functions.
- Replaced on-use with a blast that applies 3 random debuffs around the enemy.
- Renamed affix equipment name.

## T2: Onyx Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483503305953352/texAffixBlackHoleBuffIcon.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482898961285181/20230720155657_1.png)
- Unchanged. we love onyx elite. (not that we dont love other elites but still)

## T2: Realgar Elites <img src="https://cdn.discordapp.com/attachments/515678914316861451/1131483503570210826/texAffixImpPlaneBuffIcon.png" width="24">
![Elite](https://cdn.discordapp.com/attachments/515678914316861451/1131482897405194330/20230720154900_1.png)
- Changes on-use to the spike summon (to the current position). if spike is summoned, previously spawned spike disappears.
- Renamed affix equipment name.

## Other Changes
- [Blighted Elites](https://thunderstore.io/package/Moffein/BlightedElites/): Renamed to **Obsidian** Elite. (fits the T2 naming scheme)
- Rising Tides compatibility with affix-in-logbook mods ([WolfoQoL](https://thunderstore.io/package/Wolfo/WolfoQualityOfLife/), [ZetAspects](https://thunderstore.io/package/William758/ZetAspects/)) and better-description mods such as [BetterUI](https://thunderstore.io/package/XoXFaby/BetterUI/).
- Ability to set cooldown / enemy usage for each aspect on-use.

## Credits / Thanks
- [Mystic](https://thunderstore.io/package/TheMysticSword/): i mean yeah, also stole codes (i still love you :cry:)
- [HIFU](https://thunderstore.io/package/HIFU/): Anglesite / WRB Celestine / Artifact of Blindness post-processing
- [William758](https://thunderstore.io/package/William758/): Aspect Description  
  **Message to will**: I haven't done full compat yet bc idk if you wanna make compat on your side. `NemesisRisingTidesZetAspectCompat.dll` only changes some RisingTides fragments based on config values. Your work is much appriciated. o7
- [Smxrez](https://thunderstore.io/package/Smxrez/): Idea guy (helped me come up with rework ideas somewhat)
- Somewhere Else <img src="https://cdn.discordapp.com/attachments/781570609729372253/1112438647036334100/SE.jpg" width="24">

## Changelog
- 1.0.4: added korean translation (thanks @ggang-b on git)
- 1.0.3: added config for blighted name change
- 1.0.2: fixed magnetic elites giving way too much money on death
- 1.0.1: VFX additions, icon changes, bugfixes, fixed typos