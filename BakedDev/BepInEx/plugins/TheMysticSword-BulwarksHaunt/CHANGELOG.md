## 1.1.3:
* The Crystalline Blade is now consumed upon entering the realm
* Enemies affected by Crystalline Blade (Unleashed) no longer receive healing
* Stacking Crystalline Blade (Unleashed) now stacks radius
* Dying while affected by an enemy's Crystalline Blade (Unleashed) should now properly undo its effects
## 1.1.2:
* Added ProperSave support
* Added configs
* Ghosts now spawn around the player instead of choosing random spots
* Ghosts now have flat extra health
* Added fallback out-of-bounds zone that teleports players back to surface in case all other out-of-bounds zones fail
* Fixed Wave Modifier - Calamity not working
## 1.1.1:
* Wave modifiers are now properly networked in Multiplayer
* Added more wave modifiers
## 1.1.0:
* Added extra rewards for the ending!
	* Completing once will add an extra function for the Crystalline Blade
	* Completing as one of the survivors will unlock a recolour skin for that survivor
* Added random modifiers that get activated for specific waves
* Added on-player item displays for the Crystalline Blade
* Ghost spawns are now a bit more frequent
* "Wave Complete" message is now more visible
* Moved out-of-bounds ceiling higher
## 1.0.5:
* Dead players are now respawned after each wave
* Changed the colour of the ghosts to green to make them distinguishable from Happiest Mask ghosts
* Reduced initial monster spawn director credits
* Reduced the credit gain for the elite wisp spawn director
* Fixed Russian language file encoding issue which caused all text from this mod to show up as question marks
* Fixed the wave break timer not showing up for non-host players
* Fixed the wave counter not increasing for non-host players
* Fixed the mod not being marked as "required for everyone" in multiplayer sessions
* Fixed ground enemies spawning mid-air
## 1.0.4:
* Fixed the stage replacing the destinations of all Lunar Seers after stage 8
* Fixed obscene EXP and gold drops from non-ghost enemies
* Fixed non-ghost enemy directors spawning enemies too infrequently
* Fixed ghost corpses not despawning if Corpse Clean-up was set to Hidden
* Added a hard enemy cap per wave to prevent waves that last too long
* The fallback enemy spawner is now closer to real gameplay, starting off with easier enemies in the first waves, and harder and more numerous enemies in the later waves
## 1.0.3:
* Fixed an issue with attempting to spawn enemies that lack a CharacterMaster, should prevent a softlock with modded enemies
## 1.0.2:
* Nodegraphs are now prebaked, significantly improving the load time
* Added an extra out of bounds enemy killer that should be consistent
* Tweaked wisp experience and money drops
* Tweaked wisp spawns
* Actions in Hidden Realms are no longer tracked for the event
* Improved dead/failed-to-spawn enemy detection to avoid softlocks
* Removed ghost health decay
* Moved the out of bounds ceiling zone lower
* Fixed error spam with MoonstormSharedUtils
* Fixed missing SurfaceDefs on trees
## 1.0.1:
* Updated README with screenshots and extra info
* Added extra fallback behaviour in case of getting to the stage too early
* Fixed a bug with enemies being spawned too quickly
