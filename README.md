# Movementbuff's Competitive Config for Off The Grid 


>  Follow along here with Video Guide https:// Unreleased  
       


# Downloading the Config:
- First, on the right side of this page, right-click "Movementbuff's Competitive Config" underneath "Releases" and select 'Open in New Tab'
  Alternatively, open this link in a new tab:  https://github.com/movementbuff/offthegridgame/releases

- In that tab, left-click "DeviceProfiles.ini", "Engine.ini", "GameUserSettings.ini" and "GzGameUserSettings.json". This will download the config files.
  Once you have downloaded each file, close the "Releases" tab.

- **You will need to goto the top right of your browser and select Downloads then Left-Click each file and select "Unblock/Download unverified file"**
  



# Pre-Installation of Config:
- Press Windows Key + R and type **%localappdata%\G01\Saved\Config\WindowsClient** then press enter.

- Copy and Backup the file **"GameUserSettings"** to somewhere memorable.

- Press Windows Key + R again and type **Saved Games\OTG** then press enter.

- Copy and Backup the file **"GzGameUserSettings"** to somewhere memorable.

**Leave your backups alone unless you seek to restore your previous settings.**

# Installation of Config files:

- Inside "WindowsClient" folder ( **Windows Key + R  %localappdata%\G01\Saved\Config\WindowsClient** ) copy and paste **"Engine.ini"** , **"DeviceProfiles.ini"** and 
 **"GameUserSettings.ini"** from the location your downloaded them.
  
( Typically this is the Downloads folder, quickly navigate there by **Pressing Windows Key + R and typing 
 Downloads**.  )


- After Pasting the files into the folder, Right click each file and Select "Properties". Tick the box **"Unblock"** if visible and ensure that **"Read Only" is ticked/enabled.**

- Return to the G01 folder ( **Windows Key + R Saved Games\OTG**   Press Enter ) and replace **"GzGameUserSettings.json"** with the version you downloaded.

- Perform the same check as you did before to verify that Read Only is enabled on both files and they are Unblocked.

# Changing Settings ingame 

***Do NOT change any graphic settings ingame except for "Resolution Scaling Method","DLSS/FSR Mode", "Resolution", "Monitor/Display" or "Fullscreen/Borderless".***
-
DLSS is Enabled in this config and set to "Performance". Raise this to Balanced if you want to have greater image clarity at range. 
From my testing; the image quality DLSS provides ( on my system ) is superior in clarity to FSR3 whilst achieving the same or better performance. I recommend using DLSS, but you're free to try other options or completely disable upscaling if you wish. You may want to lower the Sharpening as per the following instructions in "# Troubleshooting" if you choose to use FSR.




# Troubleshooting and User Preferences:


Want to increase or decrease the Sharpness of the image?
-
Edit this command from your Engine.ini underneath " [SystemSettings] " if you wish to increase or decrease the level of Sharpening. (higher values sharper, lower more blurry)

r.Tonemapper.Sharpen=1.1

Map loading incorrectly, weird graphical glitches, character stuck inside the road? Your CPU is likely too weak for the aggressive level streaming commands. 
Slightly increase these values in increments of 0.1 or 0.2 until the issue is resolved:
-
s.AsyncLoadingTimeLimit=0.2

s.PriorityAsyncLoadingExtraTime=0.3

s.LevelStreamingActorsUpdateTimeLimit=0.2

s.PriorityLevelStreamingActorsUpdateExtraTime=0.8

s.UnregisterComponentsTimeLimit=0.2


Have an older GPU like a GTX 1660,  GTX 1080, RTX 2060 or Radeon RX 590, Rx 5600xt etc?
-
Try lowering the value of this command in increments of 1024.

r.Streaming.PoolSize=3072
For most users the current value of 3072 should be fine.
Do not set it to 0.


View Distance too low?
-
Increase the value of this command. Do not set it lower than 0.4, and do not set it higher than 2.

"r.ViewDistanceScale="

When changing settings inside the config, be mindful of making changes that result in a broken appearance of the game. 
For example; if you change a setting and suddenly can see through walls, do not use that command. Your account will receive a suspension, and eventually the Developers will prevent the entire community from being able to utilise custom configs by restricting the ability for the game to read them.
We all want and deserve to play this game with consistent and high end framerates so ensure you conduct yourself and changes you make responsibly.
-
Twitch. https://www.twitch.tv/movementbuff

YouTube. https://www.youtube.com/@movementbuff

Join the Discord. https://discord.gg/a47PEhE8WE
