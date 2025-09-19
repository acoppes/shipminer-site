---
layout: home
title: Changelog
---

Release notes history

0.6.16

* Added: Analytics and Crashes Opt-in popup on main menu (only once)
* Added: Analytics and Crashes Opt-in toggle in options menu (disabled by default)
* Fixed: Added more delay between open/close tech and pause menu to see if the xbox controller issue is solved.
* Fixed: Main menu press any key is any key now.
* Fixed: Instructions now says press submit to continue.
* Fixed: Feedback on UI when not enough resources wasn't working.
* Fixed: Anomaly had extra difficulty after adjusting projectile spawn position, reduced projectile speed and spawn position a bit and added some vfx to show incoming attack.
* Changed: Cheats are now disabled by default (can be activated with -cheats command line).
* Changed: Reduced a bit chance of blueprints per level.

0.6.15

* Changed: Increased chance of getting blueprints but also limited to 3 to 4 per asteroid.
* Changed: Don't show more blueprints after unlocking all tech.
* Changed: Tech menu navigability with left/right buttons.
* Changed: New icons for Iron and Scrap minerals.
* Fixed: Enemy attacks were being rendered over the fog.

0.6.14 - DEMO WIP

* Added: Confirmation when starting new game if there are run that can be continued.
* Changed: Activated Steam Cloud Save.
* Changed: Separated tech menu (select button) from game pause (start button).
* Changed: Show LB/RB or A/D for tab navigation depending the current input.
* Changed: Anomalies attacks don't hit each other, so now there are more bolts traveling to the player.
* Fixed: Sometimes basic minerals were pushed far away instead of picking them.
* Fixed: special case where music playlist failed to set, it was failing when trying to play next.
* Fixed: Visual issue with game mode selection.

0.6.13

* Added: New Tech Tremble Device (or how I call it: ball of destruction).
* Added: Gamepad rumble toggle in options menu.
* Added: Gamepad rumble on picking minerals. Tested rumble on mining but didn't like it yet.
* Added: Started Steamworks integration (for now just open wishlist link in steam itself).
* Changed: Now scrap can be seen when destroying debris with the ship, added a small collect delay to both scrap and iron.
* Changed: Adjusted a bit scrap and iron spawn and pickup to make it more satisfactory. 
* Changed: Now options is menu is a separated popup to start adding more things to configure.
* Changed: Added a bit of deadzone for both sticks since some old gamepads are a bit more sensible and ship was showing the ray all the time (might be an option in the future)
* Fixed: Forever gamepad rumble if game paused during a rumble. There are still some edge cases with rumble in some devices that I am trying to fix but at least the obvious one was fixed. 

0.6.12

* Added: New Tech Dkeeper available to unlock in tech menu.
* Added: new upgrade to improve ray distance.
* Added: mineral names in instructions popup as a temporary solution to name minerals.
* Changed: selected palette is saved now so it is the same after restarting the game.
* Changed: hud minerals order, now scrap is the second mineral in the ui.
* Changed: removed select destination popup for now, level is generated from game mode parameters.
* Changed: adjusted initial vision around ship and slowed down fade out.
* Changed: notification is now incoming anomaly not warning: incoming enemy, don't want to say anything at first of being an enemy.
* Changed: company logo splash now reacts to selected palette.
* Removed: experienced miner upgrade which wasn't working fine and wasn't clear (gonna re add it as a tech maybe in the future). 

0.6.11 

* Added: new placeholder game mode selection after pressing new game.
* Added: main menu has access to some options now.
* Changed: enemy miners attract and collect basic minerals (iron and scrap).
* Changed: ship is vulnerable again after pressing keep playing.
* Changed: more sound effect changes.
* Fixed: fix to cover the screen borders in some resolutions, I hope this time works xD. 
* Fixed: savegame bug when started new game and game was force closed after that (without leaving with save and leave).
* Fixed: now ui sound effects volume is affected by sfx slider too.
* Fixed: special case of trying to travel (and save the game) after completing the game. For now the game will allow that but in the future that will change. 

0.6.10

* Changed: reduced a bit the extra empty size for asteroids.
* Fixed: blueprint tech unlock after loading savegame.

0.6.9

* Added: first version of save game and continue, for now just keeping the ship progress only (upgrades, tech, minerals) but not the asteroid.
* Changed: improved explosions performance when spawning lots of basic mineral.
* Changed: added more window open/close animations.
* Fixed: tech panel was failing when all possible tech was found.
* Fixed: installing again installed tech was consuming minerals again.

0.6.8

* Changed: removed trading station for now, and reduced tech install costs.
* Changed: levels have more empty space around asteroids now to make small levels more enjoyable by reducing the confinement feeling.
* Changed: Vsync is on by default now, later I will add more graphics options.
* Fixed: unstable mining ship damage reduced to just 0.1hp (it was doing 2hp but was a bug) only if inside some close distance, otherwise it just does the pushback.
* Fixed: dpad navigation inconsistencies on Steam Deck.
* Fixed: control instructions now visually cover the game.

0.6.7 

* Added: exit dialog when quitting the game.
* Added: ui navigation and buttons sound effects (wip)
* Changed: a lot of new sound effects.
* Changed: can press esc/back to escape from upgrades scroll in outcome window now, that window needs some work for sure but at least the normal esc reaction works now.

0.6.6 - Demo WIP

* Added: Icons for steam and discord links.
* Changed: Show outcome window with game stats when quitting.

0.6.5 - Demo WIP

* Added: more tech placeholder to give idea of other tech the game is going to have but not available in demo. 
* Changed: travel station can't be killed by anomalies now.
* Changed: use d3d11 by default in windows instead of d3d12 to try to solve some graphic device issues.
* Changed: show outcome window after pressing keep playing the game and then decide to leave.
* Fixed: ship hp ui not showing ship at max hp after drone repair.
* Fixed: music loops again after defeating the game and select keep playing.

0.6.4 - Demo WIP

* Added: toggle to invert colors to start showing the game allows color changing.
* Added: button to randomize palette (not gonna be like this in the final game) and reset to default.
* Added: confirmation dialog to delete stats.
* Added: confirmation dialog to quit game.
* Added: wishlist call to action in multiple places, for now just the link, in the future will be with steam overlay.
* Added: play game sub menu, to show multiple game options like continue (doesn't work yet), new, sandbox, custom.
* Added: some Not Available in Demo popups for Custom mode and Sandbox mode (not implemented yet).
* Changed: space portal is never spawned close to the ship now.
* Changed: disabled arrow keys tabs navigation in the pause menu since it had some issues, added TAB as button now, and will add a way to move the cursor to the tab itself and change it from there with arrow keys. 

0.6.3

* Changed: allied miner drones collect minerals directly to the player.
* Changed: reduced a bit ship and drone hit points to make it a bit more dangerous to take damage. 
* Changed: internal changes to support palette swap in the future and also different resolutions.
* Changed: game should adapt better to different resolutions now, and more pixel perfect.
* Changed: terrain is more resistant now, quick test to see how to make the void ray and ray upgrade more important and to also not be able to complete the game in 3 mins.
* Added: can change the game scale in the options ui.
* Added: small extra vision where the ship starts to show a bit more of the surroundings.
* Fixed: enemy outside screen indicators are now always in the screen borders.
* Fixed: procgen sometimes placed the ship too close to the artifact and made it outside the terrain or even not spawned.

0.6.2

* Added: player stats in main menu with different data like how many runs, time played, asteroids visited, etc.
* Added: gamepad right stick can navigate ui now.
* Changed: stars have multiple parallax layers, this is a test, not sure about it yet.
* Changed: repair drones try to move better to repair targets.

0.6.1

* Changed: Inverted trade station ui to show first what you want and then the cost.
* Fixed?: Added extra checks to try to avoid bug happening when drones attach minerals to bring to ship or anomaly.

0.6.0 - Space Stations

The objective is to get test a bit how it feels having to explore to discover useful buildings and also how it feels to have to go back and forth, and not having all the actions in the ship.

* Added: Factory Space Station, spawned somewhere around the asteroid, removed drones from ship's tech menu. Build a drone takes some time now.
* Added: Trader Space Station spawned somewhere in around the asteroid, allows you to trade minerals (for now).
* Added: Friendly Miner Drone.
* Changed: Removed try again button which wasn't allowing to try again same level, it was just restarting everything, changed the continue to main menu to be explicit.
* Changed: Now drones have less hp and are targetable by anomaly attacks.
* Changed: Healing drones now heal like before, consume minerals while doing that. 
* Changed: All Space Stations have a lot of hp but can be destroyed and drop lots of debris. Repair drones can fix them.
* Changed: Removed iron cost from all tech installs.
* Changed: Enemy miners visuals are a bit more different than friendly miners now.
* Fixed: Anomaly attacks now consider closest target.
* Changed: Configuring an internal crash report tool to check for errors. 

0.5.4 - More stuff to do

This is a work in progress change, but wanted to upload something after so much time.

* Added: Enemy miners spawned from anomalies.
* Changed: Now anomalies don't fire random attacks.
* Changed: Increased a bit some mineral shape sizes in order to try to help a bit more to identify them visually.
* Changed: Drones and enemy miner spawn scrap mineral directly on death instead of spawning debris.
* Changed: Proc gen now tries to target different densities for each main mineral type.
* Changed: Space portal to travel to other asteroids is spawned with level generation.
* Added: new song named Shards by Unf0ld.

0.5.3 - Stability (bug fixing)

* Fixed lots of small internal bugs that might be making the game a bit unstable after playing some time.

0.5.2 - Replay & Progress value (content update)

* Fixed: try again button regenerates level now.
* Changed: Reduced portal cost to not require 1 anomaly core.
* Changed: Disabled ship collision damage for now.
* Internal: Minerals generation is integrated as new step in new procedural generator. 
* Changed: Disabled mineral core spots generation for now.
* Changed: Healing drone now heals the ship for some amount and autodestroys itself after that, doesn't consume drone slots.
* Changed: Hud for ship hitpoints now show some bars instead of a number and % to see if that helps a bit more understanding the current hp, did some damage rebalance too.
* Changed: Scout drones now explore the asteroid and reveal minerals.
  - They don't consume minerals anymore.
  - They die after some time.

0.5.0 - Replay & Progress value

* NEW: now asteroid shape is being generated with procedural generation and then the minerals are added over that shape.
  - Used seed and asteroid size debug in pause menu to regenerate in case there are some bugs.
* Added: buildable Travel Portal to allow the player to travel to next asteroid.
  - It is an initial exploration of "starting the asteroid in a better state", but the solution will probably change.
* Changed: terrain fill to try to reflect its current resistance. 
* Fixed: now playlist continues with next song if game is paused.
* Fixed: Don't show multiple artifact in the terrain, first one found becomes the main one (the others are deleted).
* Changed: Mineral core spots now show different states based on their current resistance.
* Fixed: some elements were being spawned at 0,0 on start and overriding themselves sometimes and/or being auto destroyed if no terrain there.
* Chest generation is removed, it is cool but not changing gameplay yet so I prefer to have it off for now.
* Fixed: advanced scanners stat.

0.4.2 - Content & Experience Update 2

* Added mineral core spots where you can get multiple of the same mineral.
* Added small particle for reveal mineral attachments. 
* Added chests that provide multiple random minerals.
* Removed supply boxes for now.
* Now blueprints are generated randomly in the asteroid like everything else.
* Fixed asteroid nodes having multiple elements inside at the same time (or not?, maybe it is not fixed).
* Added some small variation to the level generation.
* Performance improvements

0.4.1 - Content & Experience Update 1

* Added error feedback when no minerals to buy stat or tech.
* Added camera shake options to set intensity or even disable it.
* Added Radio Station to the pause menu showing current song name, time and duration.
* Added two new songs and now songs are now shuffled.
* World is a bit smaller now to experience finding stuff easier.
* Can continue playing after beating the game.

0.4.0 - Artifact & Interactables

* Artifact 
  - Has to be found in the asteroid now and manually activated. 
  - Now Ship collects minerals normally after activation, and artifact process collected minerals from it.
  - Manual activation popup contains artifact info but also in pause menu after activation.
* Trying some mining asteroid experience improvements 
  - Terrain nodes are bigger now. 
  - Particles on terrain node mined 100%.
  - Terrain nodes tremble while being mined.
  - Terrain nodes are unattached and can be pushed away, etc, when no neighbours (base for another idea in mind)
* Changed tech and stat costs, now installs use anomaly cores.
* Others
  - Scrap is heavier now to push it less distance while mining.
  - Highlight minerals in hud for selected stat or tech cost.

0.3.5 - Tech Update - 3rd Pass

* Changed tech menu to have the Stats Window that can be upgraded with minerals from the beginning.
  - Stats costs are incremented per stat level.
* Removed xp bar and level up popup window.
* Improve tech menu motivation/usage
  - Added hud notification to motivate opening menu first time.
  - Changed to not say which tech you picked up when finding blueprints.
* Added supply boxes with some random minerals inside (and sometimes blueprints too)
* Other changes:
  - Mining ray now applies small force to targets.

0.3.0 - Tech Update - 2nd Pass

* Level up by mining and select basic upgrade to improve in popup window, no minerals cost.  
* Tech (build and install) and Upgrades are in different tabs.
* Changed a bit costs between Buildable and Installable Tech Modules.
* Changed a bit mineral icons to try to make them more clear what is what.
* Terrain nodes are a bit bigger now in order to better show the minerals and other things inside it.
* Trying to improve damage feedback
  - Screen flashes now on getting damage.
  - All explosions have pushback now.
  - Damage numbers animations are a bit slower too.
* Other changes
  - Hud is always visible now, might add a special key or option somewhere at some point to toggle it again.
  - Added more background songs to the game
  - Terrain explosive cracks deal less damage to ship now.
  - Fixed some weird behaviors with terrain explosive cracks.

0.2.0 - Tech Update - 1st Pass
* Tech is unlocked by finding blueprints in terrain.
  - One idea for the future is to level up by mining 
    to upgrade normal stats and find blueprints for 
    tech in the terrain to install modules or build stuff.
* More tech.
* Some UI Style changes to make more clear with tech is selected.
* Auto select last unlocked tech when tech menu is opened.
* The Artifact needs minerals to charge now to make last part more active.
  - Idea in the future is to have to find parts of the
    artifact instead of building it.
* Changed Asteroid layout to increased exploration space
  - Idea is to take advantage of this in the future, like 
    adding spaceships, supplies, etc. 
* Other changes:
  - Speeded up opening screens.
  - Removed refinery tech for now.
  - Don't show tech level for now since it can't be upgraded.
  - Reduced attraction range to have to go for minerals.

0.1.6
* Game starts in fullscreen now.
* Hud auto opens faster now.
* Added a small enter/leave animations for hud.
* Changed Toggle HUD button in Gamepad to left shoulder.

0.1.5
* Quality of life auto movement when almost mining terrain. 
* Reduced cost of The Artifact.
* Removed game timer for now.
* Hud auto opens after some time now.
* Scout Drone:
    - Starts with ability loaded.
    - Reduced detect minerals cost and cooldown.
    - Changed visuals to make it different from other drone.
* Added feedback form link to main menu. 

0.1.4
* Added the what's new window.
* Bigger Anomaly has bigger range now.
* Music changes to action one when The Artifact is built.
* Fixed restarting level sfx muted.
* Fixed restarting level asteroid size was a small one.
* Fixed Healing Drone destroyed while healing.
* Fixed Anomaly couldn't collect minerals while in big state. 
* Fixed discord invite url.
    
0.1.3
* Artifact is more expensive now (still ~15 mins to complete)
* Ending (after The Artifact) is more intense now.
* Added refinery to convert anomaly cores into minerals.
* Reordered hud layout.
