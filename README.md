# Movementbuff's Competitive Config for Off The Grid with Video Tutorial
Follow along here with the Video Tutorial!

>  Don't forget to follow me on Twitch <3
https://www.twitch.tv/movementbuff
       
This config will raise your AVG FPS but more importantly will reduce the severity of stutters and how low your FPS drops. 
Some users may notice similar AVG FPS to their previous settings, however you WILL see a great improvement to performance during fights and "stutter prone" instances throughout your encounters on Teardrop Island.

# Downloading the Config:
- First, on the right side of this page, right-click "Movementbuff's Competitive Config" underneath "Releases" and select 'Open in New Tab'
  Alternatively, open this link in a new tab:  https://github.com/movementbuff/offthegridgame/releases

- In that tab, Right-Click and select "Open in new tab" for the two files "GzGameUserSettings.json" and "Help.txt".  To download the remaining config files, you will 
  need to open each one in a new tab, then goto the top right of your browser and select Downloads where you should see three instances of 
  "Unverified Download Blocked". You will need to left-click each one and select "Download Unverified File". Ensure you do this for **"Engine.ini"** , **"DeviceProfiles.ini"** and **"GameUserSettings.ini"** .
  
  Once you have downloaded each file, close the "Releases" tab.





# Pre-Installation of Config:
- Press Windows Key + R and type **%localappdata%\G01\Saved\Config\WindowsClient** then press enter.

- Copy and Backup the file **"GameUserSettings"** to somewhere memorable.

- Press Windows Key + R again and type **Saved Games\OTG** then press enter.

- Copy and Backup the file **"GzGameUserSettings"** to somewhere memorable.

**Leave your backups alone unless you seek to restore your previous settings.**

# Installation of Config files:

- Inside "WindowsClient" folder ( **Windows Key + R  %localappdata%\G01\Saved\Config\WindowsClient** ) copy and paste **"Engine.ini"** , **"DeviceProfiles.ini"**,
 **"GameUserSettings.ini"** and a copy of **"Help.txt"** from the location you downloaded them to.
  
( Typically this is the Downloads folder, quickly navigate there by **Pressing Windows Key + R and typing 
 Downloads**.  )


- After Pasting the files into the folder, Right click each file ( except for Help.txt ) and Select "Properties". Tick the box **"Unblock"** if visible and ensure that **"Read Only" is ticked/enabled.**

- Return to the G01 folder ( **Windows Key + R Saved Games\OTG**   Press Enter ) and replace **"GzGameUserSettings.json"** with the version you downloaded aswell as placing *another* copy of **"Help.txt"**.

- Ensure that the file **"GzGameuserSettings.json"** is ***not*** set to Read Only. This is important as it will allow you to change your sensitivity, volume, resolution and scaling methods inside the game menu without having to edit this file!

# Changing Settings ingame 

***Do NOT change any graphic settings ingame except for "Resolution Scaling Method","DLSS/FSR Mode", "Resolution", "Monitor/Display" or "Fullscreen/Borderless".***
-
DLSS is Enabled in this config and set to "Performance". Raise this to Balanced if you want to have greater image clarity at range. 
From my testing; the image quality DLSS provides ( on my system ) is superior in clarity to FSR3 whilst achieving the same or better performance. I recommend using DLSS, but you're free to try other options or completely disable upscaling if you wish. You may want to lower the Sharpening as per the following instructions in "Troubleshooting and User Preferences" if you choose to use FSR.




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

Your character appears too pixellated now and you want Ninja to look high quality again?
-

Remove the file "DeviceProfiles.ini"
The game appears to not utilise it fully anyway and from what I can see, DeviceProfiles.ini is only affecting character, UI, and maybe some occasional Effects in the distance. Feel free to remove it but I can't promise FPS stutter won't worsen as a result.

When changing settings inside the config, be mindful of making changes that result in a broken appearance of the game. 
For example; if you could change a setting and as a result are able to see through walls, do not use that command. Your account *will* receive a suspension, and eventually *the Developers will prevent the entire community from being able to utilise custom configs by restricting the ability for the game to read them.*
We all want and deserve to play this game with consistent and high end framerates so ensure you conduct yourself and changes you make responsibly.
-
Twitch. https://www.twitch.tv/movementbuff

YouTube. https://www.youtube.com/@movementbuff

Join the Discord. https://discord.gg/a47PEhE8WE
