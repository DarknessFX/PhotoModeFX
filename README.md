     .----------------.  .----------------.  .----------------. 
    | .--------------. || .--------------. || .--------------. |
    | |  ________    | || |  _________   | || |  ____  ____  | |
    | | |_   ___ `.  | || | |_   ___  |  | || | |_  _||_  _| | |
    | |   | |   `. \ | || |   | |_  \_|  | || |   \ \  / /   | |
    | |   | |    | | | || |   |  _|      | || |    > `' <    | |
    | |  _| |___.' / | || |  _| |_       | || |  _/ /'`\ \_  | |
    | | |________.'  | || | |_____|      | || | |____||____| | |
    | |              | || |              | || |              | |
    | '--------------' || '--------------' || '--------------' |
     '----------------'  '----------------'  '----------------' 

           DarknessFX @ https://dfx.lv | Twitter: @DrkFX

# PhotoModeFX for Unreal Engine 4

A complete, generic, unobtrusive, easy-to-use in game photographic system for Unreal Engine 4.23.1 (and newer).<br/>

Project info/blog at https://dfx.lv/PhotoModeFX .<br/>

<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/MenuCapture.png" width="640px" />

## Features

- Moveable camera while paused.
- Easy to use, add BP_PhotoModeFX to your level and is ready to use.
- HighResolution with Buffer Visualization screenshots (via ScreenshotTools plugin).
- Panoramic (360) and Stereoscopic (VR) with Buffer Visualization screenshots (via PanoramicCapture plugin).
- Blueprint Actor and UMG to easily package your project to any supported platform.
- No tick events.
- Following current UE4 Best Practices.

# Requirements
Unreal Engine 4.23.1 or newer.<br/>
ScreenshotTools plugin (can be disabled if HighRes Screenshots aren't necessary).<br/>
PanoramicCapture plugin (can be disabled if Panoramic/Stereoscopi Screenshots aren't necessary).<br/><br/>

<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/HowToUse_0.png" width="640px" />

# Note for compatibility with Unreal Engine 4.26

CineCameraComponent Filmback nodes changed name from **"Filmback Settings"** to **"Filmback"** after UE4.23.1, to fix this error just create new nodes Get/Set using "Filmback" and move the connectors.<br/>
You can find this nodes inside **BP_PhotoModeFX**, Functions **PMFX_UI_Filmback** and **PMFX_UI_SensorChanged**.<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/HowToUse_UE426.png" width="640px" />


# Versioning
v0.1 - Alpha released.

## TODO

- Lots of features are under construction until full release.

## Credits

Unreal Engine by Epic Games - https://www.unrealengine.com/ .<br/>

## License

@Copyleft all wrongs reserved. <br/><br/>
DarknessFX @ <a href="https://dfx.lv" target="_blank">https://dfx.lv</a> | Twitter: <a href="https://twitter.com/DrkFX" target="_blank">@DrkFX</a> <br/>https://github.com/DarknessFX/PhotoModeFX
