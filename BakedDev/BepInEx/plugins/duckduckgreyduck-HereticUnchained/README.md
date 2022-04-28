JOIN THE DISCORD AND STUFF https://discord.gg/b6aezQv54w

Big thanks to Rob for helping set this project up a long time ago! Couldn't have done it all without him.
Another big thanks to FOG for helping with icons!

## Mod Overview
HereticUnleashed aims to bring an overhauled Heretic experience to bird enthusiasts. In the same vein as ArtificerExtended, this mod improves existing content with stat changes and bug fixes, on top of adding new content to toy with. Not only that, but each new alt skill will allow you to change the skill replacements provided by each Heresy item, enabling a much more diverse selection of skills between the entire cast!

[![](https://media.discordapp.net/attachments/867999470439243806/869682486395936788/unknown.png)]()

# BALANCE ADJUSTMENTS AND REWORKS

On top of new content, Heretic Unleashed also tweaks and fixes existing Heretic content. The changes are...

```
	General:
- Reduced base max health to 260 (+78)
- Increased base regen to -4 (-0.8)
- Reduced base damage to 16 (+3.2)
- Increased base armor to 30
- Root and Nullify now also prevent victims from jumping

	Secondary:
- Reduced Slicing Maelstrom "slice" DPS, increased proc coefficient (600% and 6x0.5 per second)
- Increased Slicing Maelstrom "blast" damage and radius (900% and 17m)
- Changed Slicing Maelstrom "blast" falloff model (Linear)
- Increased Slicing Maelstrom charge duration (3s)

	Utility:
- Fixed Shadowfade healing behavior (now 15 ticks of 1.67% healing, or 25% total)

	Other:
- Fixed negative regen multiplier behavior 
* (regen multipliers now add/subtract a portion of the absolute value of regen, so negative regen is worsened by Monsoon's regen penalty for example)
- Numerous fixes to display text
```

# Content!

### Primary Skills!

Sanguine Verdict:
```
Costs 5% HP to cast. Up to 3x per second (+2 per stack), fire a laser that deals 150% damage. Deals up to 3x more damage to low health enemies.

Has no cooldown.
```

### Utility Skills!

Duskwarp:
```
Dealing damage heals you for 8% of the total damage dealt while this skill is ready to use. Activating the skill causes you to dash backwards, leaving a storm where you were standing that deals 400% (+400% per stack) damage per second for 3 seconds.

9 second (+3 per stack) cooldown.
```

### Special Skills!

Weeping Lesions:
```
Hold to root yourself in place, channeling a barrage of blades that bleed EVERYTHING in sight (including yourself) for 3 seconds (+2 per stack).

15 second (+5 per stack) cooldown.
```

# Known Issues

- Probably has conflicts with other Heretic based mods
- Doesnt remove duplicate logbook entry (how do i get rid of this???)

## Changelog
### 1.3.1
```
- Fixed a bug where Sanguine Verdict would fire every frame
- Fixed a bug where Heretic's level damage was much lower than it shouldve been
- Hopefully fixed a bug where the Heretic would sometimes be unplayable after spawning in
- Fixed a bug where stunning/freezing the Heretic could break the game
```

### 1.3.0
```
	General:
- Heresy items now change their descriptions (to reflect skill preferences and their stacking behavior) when you pick them up

	Weeping Lesions:
- Slightly adjusted damage formula
- Corrected grammar in description
```
###  1.2.0
```
	General:
- New Special skill: Weeping Lesions!
- Increased base max health (240 -> 250)
- Increased base armor (20 -> 30)

	Sanguine Verdict:
- Reduced damage (200% -> 150%)

	Duskwarp:
- Now only fires away from the aim direction, instead of away from movement 
- Updated Interrupt Priority so it can now be used during other attacks
```

### 1.1.2
```
	General:
- Updated R2API submodule dependencies

	Sanguine Verdict:
- Added new icon, courtesy of FOG!

	Duskwarp:
- Added new icon, courtesy of FOG!

	Other:
- Fixed a bug
```
### 1.1.1
```
	General:
- Increased max health (200 -> 240)
	
	Sanguine Verdict:
- Changed falloff model (None -> DefaultBullet)
- Reduced health cost (6% current -> 5% max)
- Reduced spread bloom (0.5 -> 0.2)
- Updated VFX

	Duskwarp:
- Changed cooldown behavior (8(+4) -> 9(+3))
- Updated description to more accurately portray passive behavior

	Ruinous Wake:
- Updated description to more accurately portray passive behavior
```

### 1.1.0: Finally, heresy alts!
```
	General:
- Added 2 new heresy alt skills: Sanguine Verdict and Duskwarp!

	Other:
- Fixed a bug where Slicing Maelstrom was dealing 9x as much damage as intended.
```

### 1.0.2
```
	Other:
- Fixed a bug where Ruin would fail to be consumed
```

### 1.0.1
```
	General:
- New adjustments to Slicing Maelstrom behavior
- New icon for Dissident Will (courtesy of FOG)
```

### 1.0.0 - Release Ver
```
	General:
- Initial release!
```