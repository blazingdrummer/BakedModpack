#LunarCoinShareOnPickup

	**Main Function:**
	╔══════════════════════════════════════════════════════════════════════╗
	║When one player in the lobby picks up a Lunar Coin, each player in the║ 
	║lobby will receive a Lunar Coin.                                      ║
	║                                                                      ║                                 
	║No more hate and envy against the person who grabs them the quickest. ║                                                                
	╚══════════════════════════════════════════════════════════════════════╝
	
	**Secondary Functions:**
	╔════════════════════════════════════════════════════════════════════════════════════════╗
	║Change the Lunar Coin amount that each player receives when a Lunar Coin gets picked up.║
	║Change the Lunar Coin amount that the person who picks up the Lunar Coin receives	     ║
	║(The shared and unshared amount of Lunar Coins stack, so the unshared part just gives   ║
	║extra Lunar Coins to the player who picks up the Lunar Coin)          					 ║             
	╚════════════════════════════════════════════════════════════════════════════════════════╝
	
	Working in singleplayer and multiplayer
	Fully configurable via config file.
	
#Config
	
	To change values in the config you have to start the game once with
	the .dll inserted so the config file gets generated.
	
![config](https://s6.gifyu.com/images/config.png) 

#Installation
	
   Drop the LunarCoinShareOnPickup.dll into \BepInEx\Plugins\
   
#BugReport
	
   To report bugs pls message me via the offical modding discord.
   My username is dan8991iel.

#Patchnotes
	v 3.6.0
		Updated the mod to work with the newest version of Risk of Rain 2.
		(Fixed a problem with picking up "Lunar Coins" and "Lunar Items")
	v 3.5.0
		Fixed a bug which falsely registered lunar items as lunar coins.
		(Fixed a problem with picking up equipment)
	v 3.0.0
		Checked and approved for compatibility with the newest version of RoR2		
	v 2.0.1
		Checked and approved for compatibility with the newest version of RoR2
	v 2.0.0
		Fixed a bug which stopped players from picking up lunar coins if another player is dead.
		Updated the dependencies in the manifest
	v 1.5.0	
		Added:
			Config to change the Lunar Coin shared and unshared amount.
	v 1.0.0
