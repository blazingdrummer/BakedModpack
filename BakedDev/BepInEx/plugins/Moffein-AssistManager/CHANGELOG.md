`1.4.0`

- Added support for DamageSource and DamageTypeExtended
	- **FOR DEVS: THIS IS A BREAKING CHANGE, YOU WILL NEED TO UPDATE YOUR MODS.**

`1.3.0`

- For Devs:
	- Added empty constructor to Assist object.

`1.2.0`

- Fixed Bandit revolver skills being able to trigger assists twice.
- For Devs:
	- Killer is no longer added to the assist list.
	- Direct Assists now use separate HandleDirectAssist delegates.
	
	*Mods that rely on this will need to be recompiled with the latest AssistManager dll.*

`1.1.0`

- Added extra delegates that don't expose the Assist class, for compatibility with mods that use SearchableAttribute.
	- HandleAssistCompatibleActions
	- HandleAssistInventoryCompatibleActions

`1.0.0`

- Release