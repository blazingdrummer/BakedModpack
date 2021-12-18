JOIN THE DISCORD AND STUFF https://discord.gg/yFRx3E6Yep

HUGE thanks to Rein for getting me into modding, and recently letting me reference and use his passive stuff from the long-gone AlternativeArtificer!


## Mod Overview
ArtificerExtended introduces a handful of new skills for Artificer with the intention of adding new, varied gameplay styles in creative ways. Currently introduces 10 new abilities, all arranged in a pretty pattern!

[![](https://media.discordapp.net/attachments/390713656259772417/830297527655989298/unknown.png)]()

# BALANCE ADJUSTMENTS AND REWORKS

On top of new the content, ArtificerExtended also gives balance changes to help keep Artificer a cohesive whole. They are as follows:

- ENV Suit: Movement speed and fall speed while hovering increased. The hope is that this will help the Hover feel better next to the new passive content.
- Charged Nano-Bomb: Max damage coefficient reduced to help stay in line with Nano-Spear and reduce power creep
- Snapfreeze: Base cooldown duration reduced to better fit inside Artificer's skill cycle
- Flamethrower: Now scales duration and tickrate with attack speed. Reduced base total damage coefficient to compensate
- General: Artificer Base Damage increased. Ending quote rewritten.

[![](https://media.discordapp.net/attachments/390713656259772417/830299249349754900/unknown.png)]()

## Ion Surge rework (Full credit to Rein, including this description)

- Three shorter dashes occur automatically after first activation. Triggering it again will end the skill early.
- The direction of each dash is controlled by the direction you aim, along with movement keys (including jump)!
- During the time between each dash, you hover in the air.
- All other skills can be cast at all times during the dashes, or while hovering.
- No longer deals damage or stuns.

[![](https://media.discordapp.net/attachments/390713656259772417/830299751752269848/unknown.png)]()
[![](https://media.discordapp.net/attachments/390713656259772417/832489069976092702/unknown.png)]()

## Chill Rework

The 80% "Cold Slow" has been repurposed into "CHILL" for ArtificerExtended! It can now stack up to 10x, with potential bonus effects! Not only can her cold-based skills apply CHILL, but certain items can as well.

[![](https://media.discordapp.net/attachments/390713656259772417/830305414679494696/unknown.png)]()

# CONTENT!

### Brand new skills!

FOUR new Primary skills: ICE SHARDS, FLAME BURST, LASER BOLTS, SNOWBALLS
TWO new Secondary skills: CHANNELED NANO-METEOR, FOCUSED SHOCKWAVE
THREE new Utility skills: NAPALM BARRAGE, ROLLING THUNDER, TEMPERATURE DROP
ONE new Special skill: FROSTBITE

The skills design of ArtificerExtended is focused around accessibility and depth. There is something for everyone here! Melee skills, long ranged skills, armor, mobility, cooldowns, attack speed - you name it, AE has some of it!

### And more!

New passives, and new unlocks! 

[![](https://media.discordapp.net/attachments/390713656259772417/830298690149023754/unknown.png)]()

Any unlock can even be bypassed via config if you desire.

# Known Issues

- None of the NEW passives work in multiplayer. Sorry!
- By default, modded alt skills do not contribute towards Power for Energetic Resonance and it's unlock. If a modder wants to add compatability, they should contact me and I can help them set it up.

## Changelog
### 3.1.8
```
	Passives:
- Actually properly removed the Nebula passive

	Other:
- fixed a bug
```

### 3.1.7
```
	Passives:
- Moved Nebula passive to a separate mod.
```

### 3.1.6
```
	Other:
- fixed a couple bugs
- happy birthday artificer
```


### 3.1.5
```
	Energetic Resonance:
- Updated 'Power' counting system to accomodate for secret synergies in the last patch. 
* Now has a fifth "UNFATHOMABLE" power level
- Increased stacks of Chill applied by Freezing attacks (3 -> 4)
- Modified proc chance for Chilling attacks to apply Chill

	Snapfreeze:
- No longer Freezes twice per pillar, double dipping on Chill stacks

	Temperature Drop:
- mightve fixed fall damage issues on clients in multiplayer lobbies
	
	Other:
- Attacks that Ignite no longer apply only one stack of burn with the Red Affix buff
- Extended Arti head length by 0.6%
```

### 3.1.4
```
	Energetic Resonance:
- Added a couple secret synergies
- Fixed a bug where the Arctic Blast portion of the passive was leaking into other passives
	
	Other:
- Extended Arti head length by 0.6%
- PIE
```

### 3.1.3
```
	Energetic Resonance:
- Updated Arctic Blast colors to be more distinct from glacial elite novas
- Changed elemental counting system to be more consistent, hopefully fixing a bug or two with the unlock?

	Frostbite:
- Fixed Cryostasis buff not properly displaying the spinning shields
```

### 3.1.2
```
	Flame Burst:
- Fixed casting/cooldown behavior to act like other channeled skills

	Laserbolts:
- Removed damage falloff
- Now uses the correct damage coefficient from the correct skill (130% -> 220%)
- Increased base cooldown (1.3s -> 2s)
- Increased base attack duration (0.4s -> 0.45s)
- Replaced tracer VFX (uglier, no longer leaks memory)
	
	Snowballs:
- Fixed an error where BetterUI would list the cooldown as higher than it was supposed to be
- Reduced attack duration (0.6s -> 0.55s)

	Napalm:
- Reduced burn stack requirement for its unlock (30 stacks -> 25)
- Fixed self knockback behavior to apply as all the projectiles are firing, not after

	Ion Surge:
- Reduced CDR granted from Ancient Scepter upgrade

	Frostbite:
- Added a separate buff from its Ancient Scepter upgrade, Cryostasis
- Increased armor bonus from Cryostasis
- Increased damage and range of Cryostasis novas
- Increased base cooldown of Cryostasis
- Fixed interrupt behavior so both versions can no longer cancel its own cast

	Other:
- Primary animations now properly alternate between hands
```

### 3.1.1
```
	Bug Fixes:
- Fixes an issue where the Ion Surge replacement would not occur if Ancient Scepter wasnt installed
```

### 3.1.0
```
	ENV Suit:
- Slightly increased speed bonus

	Nebula Mind:
- Reduced regen from life boosters

	Nano-Meteor:
- Fixed casting behavior to match other 'nano' skills

	Napalm:
- Improved VFX
- Doubled "dot" fire frequency

	Other:
- Improved skill replacement method (ie alt ion surge)
- Artificer head length extended by 999.99%!
```

### 3.0.1
```
	Nebula Mind:
- Increased the power of every nebula booster, especially the blue

	Bug Fixes:
- Fixed a bug where all new skills were pausing their cooldown when they werent supposed to
- Fixed a bug with the "Stunning Precision" unlock not working
- Added a little bit of logic to avoid having the "Elemental Intensity" unlock and Energetic Resonance passive break from skills with improper language tokens
- Changed Flamethrower and Temperature Drop to REQUIRE a key press to activate so that they no longer break with additional charges

	Other:
- Adjusted a few keyword tokens and descriptions to more accurately/descriptively reflect in-game behavior
```

### 3.0.0 - Passives and Unlocks!
```
	General:
- Increased Artificer's base damage to 13
- Added a buff that increases Artificer's movement speed by 15% while hovering.
- Changed Artificer's flavor text after the game's main ending!
- Added unlocks/achievements for every single skill! (configurable)
- Updated systems to be more modular (increased support for future versions + future projects)
- Lang fixes, all kinds of lang fixes! I even fixed a vanilla grammar error on nanobomb's description!
- Updated config system to only generate "Enable Config"-dependent settings if Enable Config is turned on
- Added compatability support for RTAutoSprintEX
- Improvements to loading speed!

	Ice Shards:
- Fixed cooldown not matching firebolts/plasmabolts
- Slightly reduced damage of each bolt to help compensate for the base damage increase (80% -> 70%)

	Flameburst:
- Now explodes when the projectiles expire

	Laserbolts:
- Fixed cooldown not matching firebolts/plasmabolts
- Increased base duration (0.3 -> 0.4)
- Increased base recoil (1 -> 1.6)
- Adjusted recoil calculations to be more accurate with higher attack speed

	Snowballs:
- Proc coefficient reduced (1.0 -> 0.8)
(*I didn't want to have to nerf snowballs, but they were simply too good for the new ice passive.
This should hopefully keep them from getting too crazy too quickly without feeling worse as a skill.)

	Shockwave:
- Fixed a bug where it would launch enemies into the air when they got hit
- Now requires a key press to activate (so it doesnt spam when you hold the key)

	Rolling Thunder:
- Increased starting velocity (17.5 -> 22.5)
- Adjusted velocity + delay behavior to make it easier to hit + stun monsters with
- Increased blast radius (7 -> 8)
- Increased blast force (50 -> 250)
- Fixed a bug where the thunder bolts would launch sideways when aimed against surfaces with vertical normals
- Fixed area indicator to match the bolt blast radius

	Other: 
- Patch notes of old versions moved into a seperate text file in the AE download folder
- Artificer head length extended by 999.99%!
```

[![](https://media.discordapp.net/attachments/390713656259772417/831787191633838080/oldicon.png)]()
[![](https://media.discordapp.net/attachments/390713656259772417/831787194389102602/oldicon2.png)]()
