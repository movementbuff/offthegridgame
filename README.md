# Movementbuff's Competitive Config for Off The Grid 


> > >  Follow along here with Video Guide https:// Unreleased  < < < 
       


# Downloading the Config:
First, on the right side of this page, right-click "Movementbuff's Competitive Config" underneath "Releases" and select 'Open in New Tab'

In that tab, left-click "DeviceProfiles.ini", "Engine.ini", "GameUserSettings.ini" and "GzGameUserSettings.json". This will download the config files.
Once you have downloaded each file, close the "Releases" tab.

> > > YOU MAY NEED TO GOTO YOUR DOWNLOADS TOP RIGHT OF YOUR BROWSER AND SELECT "UNBLOCK/DOWNLOAD UNVERIFIED FILE" FOR EACH FILE. < < <

# Pre-Installation of Config:
Press Windows Key + R and type %localappdata%\G01\Saved\Config\WindowsClient then press enter.

Copy and Backup the file "GameUserSettings" to somewhere memorable.

Press Windows Key + R again and type C:\Users then press enter.

Open the folder that is the name of your Windows User. You should have 2 or 3 folders. Public, Default, and a third folder. (Default may be hidden)

Scroll down and open the folder "Saved Games" then open "OTG"

Copy and Backup the file "GzGameUserSettings" to somewhere memorable.

> > > Leave your backups alone unless you seek to restore your previous settings. < < < 

# Installation of Config files:

Inside "WindowsClient" folder ( Windows Key + R  %localappdata%\G01\Saved\Config\WindowsClient Press Enter ) copy and paste "Engine.ini" , "DeviceProfiles.ini" and "GameUserSettings.ini" from the location your downloaded them. ( Typically this is the Downloads folder, quickly navigate there by Pressing Windows Key + R and typing Downloads. Press Enter. )

After Pasting each file, Right click each file and Select "Properties". Tick the box "Unblock" if visible and ensure that "Read Only" is ticked/enabled.

Return to the G01 folder ( Windows Key + R Saved Games\OTG   Press Enter ) and replace "GzGameUserSettings.json" with the version you downloaded.

Perform the same check as you did before to verify that Read Only is enabled on both files and they are Unblocked.

# Changing Settings ingame such as Sensitivity or Preferences

DLSS is Enabled in this config and set to "Performance". If you wish to change this to another Quality level, or use FSR/TSR, you will need to open the game, minimise it once you have loaded to the Menu, right-click the GzGameUserSettings.json file and untick read only. Then return to the game, make your changes in the menu and apply them, before minimising the game again and setting "GzGameUserSettings.json" back to read-only.  

IF YOU WANT TO CHANGE YOUR GUN SENSITIVITY, VOLUME, OR ANY OTHER SETTINGS, YOU WILL ALSO NEED TO DO THIS BY REMOVING READ-ONLY FROM THE FILES PROPERTIES AND RE-APPLYING ONCE CHANGED.
-

Edit this commands from your Engine.ini underneath " [SystemSettings] " if you wish to increase or decrease the level of Sharpening. (higher values sharper, lower more blurry)

r.Tonemapper.Sharpen=1.1


# Troubleshooting:
Map loading incorrectly, weird graphical glitches, character stuck inside the road? Your CPU is likely too weak for the aggressive level streaming commands. 
Slightly increase these values until the issue is resolved:

s.AsyncLoadingTimeLimit=0.2

s.PriorityAsyncLoadingExtraTime=0.3

s.LevelStreamingActorsUpdateTimeLimit=0.2

s.PriorityLevelStreamingActorsUpdateExtraTime=0.8

s.UnregisterComponentsTimeLimit=0.2
Do this by values of 0.1 or 0.2.

Twitch. https://www.twitch.tv/movementbuff

YouTube. https://www.youtube.com/@movementbuff

Join the Discord. https://discord.gg/a47PEhE8WE
