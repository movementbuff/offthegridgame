**Updated 22 March 2025:
Improved Stability (Stutter/Lag), removed entries that may conflict with future updates, re-enabled logging for Gunzilla dev team support. <3
Users must update "Engine.ini" by downloading the newest version with link below: https://github.com/movementbuff/offthegridgame/releases/download/Config/Engine.ini**
-


**Updated 12 Dec 2024:
Fixed "Red Scope" issue caused by texture quality settings in the config being incompatible with new scope system in today's update. Users must update to the newest version of "DeviceProfiles.ini" to resolve the issue. Alternatively you can simply delete the file "DeviceProfiles.ini" if preferred.**

**Updated 16 Nov 2024: Updated Engine.ini and DeviceProfiles.ini - Improved Compatibility for all systems especially laptops by raising Level Streaming CVARS under [ConsoleVariables], + minor optimizations regarding lumen as well as broader VRAM budget inclusivity.**

**Updated 2nd Nov 2024: Removed parameters for Preoptimsation of Shaders from DeviceProfiles.ini as it caused longer initial launch times.**

**Updated 1st Nov 2024: Clearly explained how AMD GPU users can use FSR instead of being confused about DLSS, added info regarding Shadows and improving the appearance of the game.**

**Updated 17th Oct 2024: Changed DLSS Mode value to "6" as the recent patch has changed the definition of the values.** 

**Updated 16th Oct 2024: Fixed broken UI on compass and potentially paralyser effect** Redownload "DeviceProfiles.ini" to update

# Movementbuff's Competitive Config for Off The Grid with Video Tutorial
Follow along here with the Video Tutorial!
https://youtu.be/OZDg6I79BQc

>  Don't forget to follow me on Twitch <3
https://www.twitch.tv/movementbuff
       
This config will raise your AVG FPS but more importantly will reduce the severity of stutters and how low your FPS drops. 
Some users may notice similar AVG FPS to their previous settings, however you WILL see a great improvement to performance during fights and "stutter prone" instances throughout your encounters on Teardrop Island.

***The config is constantly receiving changes. It may not be as pretty as you wish it were, but it significantly increases overall performance on the majority of systems and massively reduces input lag. Over time changes are being made to improve visibility, reduce unappealing aspects and eliminate non-functioning or improperly functioning commands. Please take into consideration that I am not a software engineer, game developer, or anything similar.***

# Downloading the Config:
- First, on the right side of this page, right-click "Movementbuff's Competitive Config" underneath "Releases" and select 'Open in New Tab'
  Alternatively, open this link in a new tab:  https://github.com/movementbuff/offthegridgame/releases

- In that tab, Right-Click and select "Open in new tab" for the file "Help.txt".  To download the remaining config files, you will 
  need to open "DeviceProfiles.ini", "Engine.ini" , and "GameUserSettings.ini" in a new tab, then goto the top right of your browser and select Downloads where you should see three instances of 
  "Unverified Download Blocked". You will need to left-click each one and select "Download Unverified File". Ensure you do this for **"Engine.ini"** , **"DeviceProfiles.ini"** and **"GameUserSettings.ini"** .
  
  Once you have downloaded each file, close the "Releases" tab.





# Pre-Installation of Config:
- Press Windows Key + R and type **%localappdata%\G01\Saved\Config\WindowsClient** then press enter.

- Copy and Backup the file **"GameUserSettings"** to somewhere memorable.

- Press Windows Key + R again and type **Saved Games\OTG** then press enter.

- Copy and Backup the file **"GzGameUserSettings"** to somewhere memorable.

**You *WILL* need your backups so you can maintain your sensitivity and volume settings if you accidentally make a mistake! Make sure to do this step!**

# Installation of Config files:
- Press Windows Key + R and type Downloads then press enter.

- Inside "WindowsClient" folder ( **Windows Key + R  %localappdata%\G01\Saved\Config\WindowsClient** ) copy and paste **"Engine.ini"** , **"DeviceProfiles.ini"**,
 **"GameUserSettings.ini"** and a copy of **"Help.txt"** from your Downloads folder.

- After Pasting the files into the folder, Right click each file ( except for Help.txt ) and Select "Properties". Tick the box **"Unblock"** if visible and ensure that **"Read Only" is ticked/enabled.**

- Inside the G01 folder ( **Windows Key + R Saved Games\OTG**   Press Enter ) and place another copy of **"Help.txt"** inside the folder, 
  then Right-Click **"GzGameUserSettings.json"**, select Properties and ensure Read Only is ***NOT*** ticked.

-  Open the file **"GzGameUserSettings.json"** with Notepad.

-  You should see a large list of settings and their current values. Look for these entries and set the values to match the ones shown:


       "viewDistanceQuality": 0,
       "antiAliasingQuality": 0,
        "textureQuality": 0,
        "shadowQuality": 0,
        "effectsQuality": 0,
        "globalIlluminationQuality": 0,
        "reflectionQuality": 0,
        "postProcessQuality": 0,
        "foliageQuality": 0,
        "shadingQuality": 0,
        "displayGamma": 1.7000000476837158,
        "bUseVSync": false,
        "resolutionScalingMethod": "DLSSResolutionScaling",
        "resolutionScaleValue": 0,
        "antiAliasingMethod": 0,
        "dLSSMode": 6,
   As of the most recent update, Global Illumination will likely force to a setting of "1" when you launch the game. This is fine and doesn't appear to be affecting the performance of the config.

- ***dLSSMode should now be set to 6,*** not 5 as mentioned in the installation guide on youtube as an optimization patch has just released which has changed this.     
 Set it to 6 rather than 5

***FOR AMD GPU USERS*** please use these settings!

         "resolutionScalingMethod": "FSRResolutionScaling",
         "resolutionScaleValue": 0,
         "antiAliasingMethod": 0,
         "dLSSMode": 6,
         "fSRQualityMode": 3,
	  "metalFxQualityMode": "Quality",
  
- Next, scroll down towards the bottom of the file and set these entries to match the values shown.

       "hideoutMeshMinLODQuality": 0,
       "gameMeshMinLODQuality": 0,
       "bMotionBlurActive": false,
       "bIsPerformanceMode": true,
       "bHardwareRayTracingEnabled": false,

 

- Save and exit the file. Do ***NOT*** set the file to Read Only. This is important as doing so would not allow you to change your sensitivity, volume, resolution and scaling methods inside the game menu!
  

- ***If you wish to improve the appearance of the game***, you can re-enable shadows. This greatly improves the quality of the image and can help with spotting players *at the cost of some performance* ( 10-30% depending on system )
To do this,

- Right click Engine.ini located in **%localappdata%\G01\Saved\Config\WindowsClient** and select properties then disable 
             Read Only and press Ok.


- Open Engine.ini in Notepad and **remove** these entries. You will find them under [SystemSettings]
 	
		r.ShadowQuality=0
		r.Shadow.CSM.MaxCascades=0
		r.Shadow.DistanceScale=-1
		r.Shadow.CSM.TransitionScale=0
		r.DistanceFieldShadowing=0
		r.Shadows.SpotLightTransitionScale=1
		r.Shadow.MaxResolution=0
		r.Shadow.MaxCSMResolution=0
		r.MaxCSMRadiusToAllowPerObjectShadows=0.01
		r.Shadow.RadiusThresholdRSM=0
		r.Shadow.SpotLightDepthBias=0
		r.Shadow.TexelsPerPixel=0
		r.Shadow.PerObject=0
		r.AllowLandscapeShadows=0
		r.DFShadowScatterTileCulling=0
		r.ParallelShadows=0
		r.Shadow.FadeExponent=1
		r.Shadow.PreshadowExpand=-1


	- Close and Save Engine.ini then Right click > Properties > Enable Read Only > Press OK


# Changing Settings ingame 

***Do NOT change any graphic settings ingame except for "Resolution Scaling Method","DLSS/FSR Mode", "Resolution", "Monitor/Display" or "Fullscreen/Borderless".***
-
DLSS is Enabled in this config and set to "Performance". Raise this to Balanced if you want to have greater image clarity at range. 
From my testing; the image quality DLSS provides ( on my system ) is superior in clarity to FSR3 whilst achieving the same or better performance. I recommend using DLSS, but you're free to try other options or completely disable upscaling if you wish. You may want to lower the Sharpening as per the following instructions in "Troubleshooting and User Preferences" if you choose to use FSR.




# Troubleshooting and User Preferences:


GzGameUserSettings.json file is missing some commands?
-
After one of the more recent updates, it appears some users json file is not correctly generating the commands for game options. Click this link and follow this extra guide if this applies to you. https://github.com/movementbuff/otgjson

Want to increase or decrease the Sharpness of the image?
-
Edit this command from your Engine.ini underneath " [SystemSettings] " if you wish to increase or decrease the level of Sharpening. (higher values sharper, lower more blurry)

r.Tonemapper.Sharpen=1.1

Map loading incorrectly, weird graphical glitches, character stuck inside the road? Your CPU is likely too weak for the aggressive level streaming commands. 
Slightly increase these values in increments of 0.2 - 0.5 until the issue is resolved:
-
s.AsyncLoadingTimeLimit=

s.PriorityAsyncLoadingExtraTime=

s.LevelStreamingActorsUpdateTimeLimit=

s.PriorityLevelStreamingActorsUpdateExtraTime=

s.UnregisterComponentsTimeLimit=



View Distance too low? *Changing this value is not recommended. It will not affect the render distance of other players.
-
 Increase the value of this command. Do not set it lower than 0.4, and do not set it higher than 1.

"r.ViewDistanceScale="

Character or other textures like Smoke appear too blocky and pixellated?
-

Remove the file "DeviceProfiles.ini"
FPS and stutter will likely worsen without this file but the appearance of the game will improve. Alternatively, if the smoke appearance is the only concern, try removing the Effects and EffectsNotFiltered entries in the file. 

When changing settings inside the config, be mindful of making changes that result in a broken appearance of the game. 
For example; if you could change a setting and as a result are able to see through walls, do not use that command. Your account *will* receive a suspension, and eventually *the Developers will prevent the entire community from being able to utilise custom configs by restricting the ability for the game to read them.*
We all want and deserve to play this game with consistent and high end framerates so ensure you conduct yourself and changes you make responsibly.
-
Twitch. https://www.twitch.tv/movementbuff

YouTube. https://www.youtube.com/@movementbuff

Join the Discord. https://discord.gg/a47PEhE8WE
