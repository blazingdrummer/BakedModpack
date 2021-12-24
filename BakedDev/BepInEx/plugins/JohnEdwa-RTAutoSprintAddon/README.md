# RT AutoSprint Addon | Game ver. 1.1.1.4

---

### Latest Patch.

`1.0.0`  [2021-04-xx]

* First Release.

# Description

Additional module for [RTAutoSprintExtended](https://thunderstore.io/package/JohnEdwa/RTAutoSprintEx/) that adds patches for a few custom characters and skill packs, as well as a way to set them up as a configuration file entry.

### Mod compatibility and "API":

Included patches:

* Artificer Extended: Animation delay for ``IceShard``, ``LaserBolt`` and ``SnowBall``. Sprint disable for ``CastThunder``.
* MandoGaming: Animation delay for ``HeavyPistol2`` and ``BeamPistol``.
* EggsSkills: Animation delay for ``CombatShotgunEntity``, ``TeslaMineFireState``. Sprint disable for ``DirectiveRoot``.
* Playble Templar: Sprint disable for ``TemplarRifleFire``.
* The House: Sprint disable for ``Roulette``.

## Configuration

* ``EnableDebugLog``: If the addons spits out what it's doing in the console or not.
* ``SprintDisableEntityStates``: List of EntityStates that disable sprinting. separated by `,`.
* ``AnimationDelayEntityStates``: List of EntityStates that check for `duration` field for a delay, separated by `,`.

And individual on/off toggles for the included patches/addons.

---

**The rest is for RTAutoSprintEx, i.e what this addon is doing.**

You can use SendMessage to register an EntityState to the list of Sprint Disablers and Animation Delayers. 
Add a soft dependency to ensure RTAutoSprintEx (not RTAutoSprintAddon) is loaded before your mod.

```
[BepInDependency("com.johnedwa.RTAutoSprintEx", BepInDependency.DependencyFlags.SoftDependency)]

if (BepInEx.Bootstrap.Chainloader.PluginInfos.ContainsKey("com.johnedwa.RTAutoSprintEx")) {
    SendMessage("RT_SprintDisableMessage", "EntityStates.Mage.Weapon.Flamethrower"); 
    SendMessage("RT_AnimationDelayMessage", "EntityStates.Mage.Weapon.FireFireBolt"); 
}
```

`RT_SprintDisableMessage`  blocks AutoSprinting from activating when the player is in that EntityState.
`RT_AnimationDelayMessage` looks for a field called `duration` to use as a delay - useful for keeping wind-down animations from being immediately cancelled. 

## Changelog

`1.0.0`  [2021-04-xx]

* First Release.

Full changelog can be found in [CHANGELOG.MD](https://github.com/JohnEdwa/RTAutoSprintAddon/blob/master/CHANGELOG.md).

## Contact

Open an issue [at the Github repo](https://github.com/JohnEdwa/RTAutoSprintAddon) or find me on the RoR2 modding discord (JohnEdwa#7903).