Allows certain on-kill effects to trigger off of kill assists. Everything can be toggled in the config.

## Affected Things

- Bandit's Specials

- Topaz Brooch
- Chronic Expansion

- Berzerker's Pauldron
- Hunter's Harpoon
- Infusion

- Brainstalks
- Frost Relic
- Resonance Disk
- Soulbound Catalyst
- Wake of Vultures

## For Devs

Changes from this mod can be toggled in-game by calling `SetEnabled(false)` on the change.

To add an assist, add to `AssistManager.HandleAssistInventoryActions` or `AssistManager.HandleAssistActions` depending on whether or not you need the inventory to run your code. Use `AssistManager.HandleAssistInventoryCompatibleActions` or `AssistManager.HandleAssistCompatibleActions` if you do not want to have the `Assist` class in your code (ex. code is using SearchableAttribute).

You will need to explicitly check to make sure killerBody is not the same as Assist.attackerBody. This is required since there are a few niche cases where you might not want to do this.

If you want an "on kill with slight grace period" effect, use `AssistManager.instance.AddDirectAssist()`, refer to Bandit's Specials to see how it's set up, and subscribe to the `HandleDirectAssist` delegates instead. This needs to be called **BEFORE** the damage is processed.

`DirectAssists` check for a perfect match on:
- DamageType
- ModdedDamageTypes
- DamageTypeCombo