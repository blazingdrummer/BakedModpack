If you have any feedback or ideas, please put them into this google form https://forms.gle/PwdwL98AbTrVLsuKA! Alternatively, you can DM me on Discord @duck duck grey duck#0658

## Mod Overview
DeathMarkFix allows Death Mark to finally deal more than just 50% extra damage regardless of item stack, by allowing the buff to stack on application, which was what it meant to do in the first place.

### More Detail
Deathmark functions by checking how many stacks of its debuff are on the target body, then adding a damage multiplier for each one (+50% per debuff, of course). When the buff is applied, it tries to add multiple deathmark debuffs for each deathmark you have...

... however deathmark is defined as a non-stackable debuff, so in this case the item literally does nothing past stack 1. This is all DeathMarkFix changes.

It's important to note that DeathMarkFix does NOT change the debuff's inability to reapply when there are already deathmark debuffs on the target, meaning this mod does NOTHING to change multiplayer functionality, only to be a small bug fix.

### Changes
DeathMark BuffDef "canStack" property changed from false to true. No other functionality modified. 

## Changelog
### 1.0.2
- Added link to a feedback form for Thunderstore
- Improved the description of what this mod does
- Added credit to discord users who helped find and solve this bug
### 1.0.1
- Removed debug messages (no more Lemon Demon references :( )
### 1.0.0
- First release

## Credit where due
### to @Zoni Ramboni#6689 on Discord who helped find the bug
### and to @Lightning Laser#0732 on Discord who helped fix the bug
