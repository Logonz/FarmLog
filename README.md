# FarmLog
World of Warcraft Classic addon that logs loot, monster kills, honor and instances. Know exactly what your farm session has yielded.

### What it is for
You can track your farming session and know how much gold/hour you make. Good for general grinding, instance item farming, rep farm, tradeskill work, honor farm, know how many you killed in a rare BoE farm, etc etc.

### What it does
* Tracks 
    * Shows Gold/Hour of active farming session
    * Farm session time with a stopwatch
    * Mob kills, counts how many of each mob was killed
    * Loot from mobs and quests
    * Herbalism, skinning and mining yield
    * Money loot, displays total gold collected
    * Shows loot vendor value in gold
    * Reputation gain per faction
    * XP gained
    * Skill levels
    * Honor gain (not tested yet, will be available in phase 2)
* Allows reporting farm results
* Display farm yield in a window with all looted items
* Allows filtering item poor and common items
* Save multiple farm sessions, you can switch to a different session and continue from where you left off. Read more about Sessions below.

### How to install
* Download, extract (if zipped)
* Make sure folder doesn't have `-master` surffix
* Copy `FarmLog` folder to your `WoW\Interface\AddOns` folder

### How to use
* `/fl` - toggle logging on/off
* `/fl r` - reset log
* `/fl s` - shows log
* `/fl set <ITEMLINK> <GOLDVALUE>` - sets AH value of an item, in gold

### Sessions 
Many times you pause your farming to do something else in game, like doing an instance and afterwards continue to farm herbs. So you want to know how much herb farming yields and how much the instance run has yielded, but these are two different sessions! That's why you can name sessions and switch between them according to what you're doing. 

Another thing is that the more time & data you have per session, the more accurate gold/hour metric you're going to see. For example, you can `/fl switch Herbing` when collecting herbs and `/fl switch Fishing` whenever you fish, do that for a week and you'll get a reasonably accurate gold/hour metric.

![Preview 1](https://github.com/E1ila/FarmLog/blob/master/Preview2.png)
![Preview 2](https://github.com/E1ila/FarmLog/blob/master/Preview.png)
![Preview 3](https://github.com/E1ila/FarmLog/blob/master/Preview3.png)

### Changes 
* 1.8 
    * Added Tooltip on minimap icon, showing current session
    * Main window won't close when hitting ESC
    * Allow ignoring certain items for GPH, write `/fl i [Item Link]` to add/remove from ignore list
* 1.7.3
    * Fixed bug causing to sometimes not track gray items
* 1.7.2
    * Fixed window positioning bug, causing position to load incorrectly
* 1.7.1
    * Fixed exception when parsing +rep message
* 1.6
    * REVAMPED USER INTERFACE!
    * Added delete session warning
    * Choosing a session from the UI won't resume it
    * Added reset window position `/fl rmw` and reset minimap icon `/fl rmi`
    * Fixed exception for new sessions GPH calculation
    * Pauses session when leaving instance, if Auto Switch Instances is enabled
* 1.4
    * New saved variables database format
* 1.3 
    * Allowing to rename sessions
* 1.2
    * Auto start session when entering an instance, with current instance name for session name.
* 1.1 
    * Sessions! You can now keep multiple session, read about it and how to use it above.
    * Removed "Reset Data" offer when entering an instance or after `/reload`.
* 1.0 
    * Initial release.

### To do
* Count instance IDs (total & last hour)
* Track traded gold (for enchanting, etc)
* Support Chest / Container opening
* Track deaths
* Show repair bill
* Allow listing loot without mob names
* Allow custom attribution loot to certain mob
* Support multiboxing GPH
* Add button to add a new session / rename
* Show menu when clicking items on list - delete/ignore/set AH price/reassign
