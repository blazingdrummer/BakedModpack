# MMHOOK Standalone

This mod exists to provide a standalone MMHOOK_Assembly-CSharp for other mods to depend on. 

To use, simply add the dependecy string to your dependencies in your mod's manifest.json file.

You do not need to depend on this mod in your actual Bepinex plugin because it ensures it loads first.

Version History:

###v1.0.3
- Removed any active functionality and depends on HookGenPatcher, please switch your mods to use HookGenPatcher

###v1.0.2
- Updated for latest patch 

###v1.0.1
- Stop R2API from adding the dummy mod to the networkModList 

###v1.0.0
- Initial Release