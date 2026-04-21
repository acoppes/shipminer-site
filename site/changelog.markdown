---
layout: home
title: Changelog
---

Release notes history

0.7.11 - Local Co-op Fixes

* Added: support for continue game when playing multiplayer.
* Added: different ships and ui icons for each play.
* Fixed: keep each ship progress after travel when playing local multiplayer (can't continue co-op savegame yet)
* Fixed: removed camera audio listener when playing local multiplayer. 
* Fixed: in co-op friendly ships were not respawning in the location of the ship debris if pushed (note: can push debris to other locations and then respawn friends).
* Fixed: repair drone wasn't repairing anything.
* Fixed: minerals were multiplied when playing local co-op and jumping to next asteroid.
* Fixed: anomalies attacking ship debris in co-op.
* Fixed: "single" multiplayer game was overriding singleplayer savegame. 
* Fixed: blueprints now apply correctly to all players when picking them in local co-op 

0.7.10 - Local Co-op

* Added: Local co-op support to play with friends and family, but for now is a WIP, not done, and might not even be part of the game in the future but I wanted to play the game with my kids xD
* Changed: increased scout drone vision range and renamed to Mineral Scout to make his main task more clear.
* Changed: increased hp for all drones.
* Changed: increased repair drone search distance and fixed to consider all damaged allies. 
* Changed: UI for ship health moved to the center of the screen at the bottom.
* Changed: trying a new input configuration for gamepad dpad ui navigation to see if it improves some gamepads ui nav issues (xbox wireless controller, I am looking at you right now).
* Changed: important items now reveal vision once discovered, also emit particles and in some cases have some additional sfx in order to help finding them. 
* Changed: enemies can't attack the drones factory now.
* Known issue: when playing coop only first player progress is kept after travel to next asteroid

0.7.9 - Experience

* Changed: changed to use FMOD instead of unity default audio system, this will help in the future to have a better audio experience. 

0.7.8 - Quality Of Life

* Added: show saved asteroid information in continue button.
* Added: ship teleport in/out sfx when coming to asteroid and leaving.
* Changed: added again the try again button when ship destroyed, it restarts the level with all savegame data.
* Changed: continue game will start in the same asteroid when quit was selected.
* Changed: increased mining speed stat max levels to 8 and increment per level to 20% from 15%.

0.7.7 - Destination Selection - First Pass

* Added: now player can select next destinations in stargate.
* Added: current asteroid info in pause menu.
* Changed: more performance improvements.
* Changed: increased anomaly damage and accuracy, and separated a bit difficulty per anomaly level.
* Changed: reduced hull improvement costs but now it also uses scrap.
* Changed: increased miner drones mining speed and now they don't have friendly fire.
* Fixed: gamepad rumble on ship damaged.
* Fixed: don't show gamehud error feedback when stat at max level.
* Fixed: properly select first stat when tech menu is open for the first time. 

0.7.6

* Added: now some asteroids can be inverted which are more like caves in some way giving a different exploration.
* Changed: improved performance for some ui.
* Changed: changed visuals for boundaries to see if it feels better and/or make it more clear with not being part of the asteroid.
* Changed: improved general performance of the game.
* Changed: now artifact pieces should be autodestroyed once the artifact starts building.

0.7.5 - Small Adjustments

* Changed: anomalies are auto revealed when close to the ship.
* Changed: improved tech menu selected tab and element communication.
* Changed: tech menu can be opened from pause menu now.
* Changed: tech menu shows some ui to understand which element is selected for unknown technology.
* Changed: unstable terrain nodes (explosive ones) reveal vision now when they explode.
* Fixed: options menu navigation from close button.
* Fixed: anomalies can't attack the stargate (which is invulnerable right now so it makes no sense)

0.7.4 - Progression

* Added: the game can be completed again in the fourth asteroid.
* Added: now enemies should be able to move better in order to return to closer anomaly portal to deliver minerals.
* Added: new building, the artifact assembly (it reuses and old structure assets, will try to make something different in the future).
* Changed: had to force clear the run data to be sure the proper progression, so your current run progress will be lost (if you had any).
* Changed: updated to latest unity version.
* Hotfix: continue button was active even when savegame couldn't be continued. 
* Hotfix: new savegame with no run data was failing too.

0.7.3 - Travel

* Added: show how many artifact parts were collected, only applied after escaping the asteroid with it.
* Added: basic size, minerals and density progression when traveling to next asteroid. 
* Added: enemies have some basic threat progression when traveling to next asteroid.
* Changed: now drone factory is spawned close to the stargate and only after first asteroid.
* Changed: some internal optimizations for vision/fog.
* Changed: changed back to do small damage with unstable mining now there is an easy way to recover hp from debris. 
* Fixed: highlight and show error on mineral costs, again xD. 
* Fixed: Anomaly portal can absorb minerals (is absorbing blueprints as well... should it?).

0.7.2 - Travel

* Changed: Find artifact pieces in order to travel to next asteroid (work in progress). 
* Changed: Unstable mining reduced damage to 0, and increased a bit the pushback.
* Changed: Ship auto repairs itself when collecting scrap.
* Changed: Some stats have higher cap and some others lower now.
* Changed: Related to last one, ship starts with some lower base stats but upgrades changes are more powerful now.

0.7.1

* Added: basic mouse support with virtual cursor to interact with UI.
* Fixed: updated unity to fix vulnerability issue

0.7.0 

* Fixed: close confirm popups with back or escape was leaving the game unplayable in some cases.
* Fixed: navigation issues when selecting the outcomes tech window.
* Changed: initial gamepad disclaimer text.
* Changed: disabled tutorial mode for now since it doesn't say anything and the initial scroll works strange.

0.6.16 - DEMO RELEASE

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
