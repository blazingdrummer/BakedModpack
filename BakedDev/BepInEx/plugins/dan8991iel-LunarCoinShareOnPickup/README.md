#LunarCoinShareOnPickup
- - - -

###Main Function:  
╔══════════════════════════════════════════════════════════════════════╗<br>
║When one player in the lobby picks up a Lunar Coin, each player in the║<br>
║lobby will receive a Lunar Coin.                                      ║<br>
║                                                                      ║<br>                                 
║No more hate and envy against the person who grabs them the quickest. ║<br>                                                              
╚══════════════════════════════════════════════════════════════════════╝<br>
	
###Secondary Functions:  
╔═══════════════════════════════════════════════════════════════════════════════════════════╗<br>
║Change the Lunar Coin amount that each player receives when a Lunar Coin gets picked up.	║<br>
║Change the Lunar Coin amount that the person who picks up the Lunar Coin receives	     	║<br>
║(The shared and unshared amount of Lunar Coins stack, so the unshared part just gives   	║<br>
║extra Lunar Coins to the player who picks up the Lunar Coin)								║<br>
║Change if dead players should also receive the shared Lunar Coins             				║<br>
╚═══════════════════════════════════════════════════════════════════════════════════════════╝<br>
	
	
Working in singleplayer and multiplayer.
**Only the host needs to have the mod installed.**
Fully configurable via config file.
	
	
#Config
- - - -
	
To change values in the config you have to start the game once with
the .dll inserted so the config file gets generated.
	
![config](https://s7.gifyu.com/images/4.2.0-config.png) 


#Installation
- - - -
	
You need to have the BepInExPack installed. If you don't have it installed yet you can get it [here](https://thunderstore.io/package/bbepis/BepInExPack/).
   
Drop the LunarCoinShareOnPickup.dll into \BepInEx\Plugins\
   
   
#BugReport
- - - -
	
To report bugs pls message me via the offical modding discord.
My username is dan8991iel.
   
   
#BugReport
- - - -
	
To report bugs pls message me via the offical modding discord.
My username is dan8991iel.
   
   
#Contributors
- - - -

Thanks to [Faustvii/Faust(Thuen)](https://thunderstore.io/package/?q=Faustvii&ordering=last-updated) and [FunkFrog](https://thunderstore.io/package/FunkFrog-and-Sipondo/) for feedback, suggestions and help in testing the mod to version 4.2.0.	


#Patchnotes
- - - -
* v 4.2.0
	* Fixed the store page
* v 4.2.0
	* You can now toggle in the config if dead players should receive Lunar Coins as well
	* Removed "com.bepis.r2api" as a dependency so now only the host had to have the mod installed
* v 4.0.0
	* Fixed issues with the mod not working after the latest update
	* Corrected the dependencies list on thunderstore
* v 3.6.1
	* Corrected the dependencies list on thunderstore
* v 3.6.0
	* Updated the mod to work with the newest version of Risk of Rain 2. (Fixed a problem with picking up "Lunar Coins" and "Lunar Items")
* v 3.5.0
	* Fixed a bug which falsely registered lunar items as lunar coins. (Fixed a problem with picking up equipment)
* v 3.0.0
	* Checked and approved for compatibility with the newest version of RoR2		
* v 2.0.1
	* Checked and approved for compatibility with the newest version of RoR2
* v 2.0.0
	* Fixed a bug which stopped players from picking up lunar coins if another player is dead.
	* Updated the dependencies in the manifest
* v 1.5.0	
	* Added:
		* Config to change the Lunar Coin shared and unshared amount.
* v 1.0.0
