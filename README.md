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

A complete, generic, unobtrusive, easy-to-use in game photographic system (PhotoMode) for Unreal Engine 4.23.1 (and newer).<br/>

Project info/blog at https://dfx.lv/PhotoModeFX .<br/><br/>

## Features

- Easy to use, add BP_PhotoModeFX to your level and is ready to use.
- Moveable camera with free movement while game is paused.
- 21 Filters with customizable settings, compatible with Deferred and Forward renderer.
- Pre and Post events to notify the game when PhotoModeFX is starting/exiting.
- HighResolution with Buffer Visualization screenshots (via ScreenshotTools plugin).
- Panoramic (360) and Stereoscopic (VR) with Buffer Visualization screenshots (via PanoramicCapture plugin).
- Capture and export Cubemaps.
- Generate 3DPhotos (for Facebook).
- Blueprint only, to easily package your project to any supported platform.
- No tick events.
- Following current UE4 Best Practices.

# Requirements
Unreal Engine 4.23.1 or newer.<br/>
ScreenshotTools plugin (can be disabled if HighRes Screenshots aren't necessary).<br/>
PanoramicCapture plugin (can be disabled if Panoramic/Stereoscopic Screenshots aren't necessary).<br/><br/>

<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/HowToUse_0.png" width="640px" />

## Note for compatibility with Unreal Engine 4.26

CineCameraComponent Filmback nodes changed name from **"Filmback Settings"** to **"Filmback"** after UE4.23.1, to fix this error just create new nodes Get/Set using "Filmback" and move the connectors.<br/><br/>
You can find this nodes inside **BP_PhotoModeFX**, Functions **PMFX_UI_Filmback** and **PMFX_UI_SensorChanged**.<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/HowToUse_UE426.png" width="640px" /><br/><br/>

Video Instructions:<br/>
<a href="https://www.youtube.com/watch?v=bHuNqfk4248" target="_blank"><img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_HowToUse_UE426_YTInstrucs.jpg" /></a><br/>

# How to Use

Download the Zip file.<br/>
Extract the files to any folder.<br/>
Delete the .git_img* folder (if you download/clone from main instead of <a href="https://github.com/DarknessFX/PhotoModeFX/releases/download/v0.7/PhotoModeFX.zip">release package</a>).<br/>
Open PhotoModeFX.uproject in Unreal Engine. (double+click the PhotoModeFX.uproject file)<br/>
Open Content/PhotoModeFX/BP_PhotoModeFX and compile the blueprint (ignore warnings, fix the error mentioned above).<br/>
Open the included Content/PhotoModeFX/PMFX_SampleMap and play the level.<br/>
Press keyboard P key to start PhotoModeFX (you can change the default key and other settings on BP_PhotoModeFX Details panel).<br>
If you like the features, you can migrate BP_PhotoModeFX to other projects (UE4 will migrate any dependencies too), add BP_PhotoModeFX to your main level and test on your project.<br/><br/>--<br/>
. PhotoModeFX project files are light weight with 5,659Kb (zipped) but ReadMe screenshots at .git_img folder raises it to 48,356Kb (zipped) .<br/>

# Samples

## Usage

GIF:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_Feature.gif" width="640px" /></a><br/>

Video:<br/>
<a href="https://www.youtube.com/watch?v=IyxmRHzYy-Q" target="_blank"><img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PhotoModeFX_YoutubePreview.png" width="640px" /></a><br/>

## Capture Modes

Screenshot:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_SS.png" width="640px" /><br/>

HighResolution Screenshot (scaled from 8K to 1K, displayed as 640p):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_HRSS.png" width="640px" /><br/>

HighResolution Buffer Visualization Screenshots (scaled from 8K to 1K, to 216p 5x gallery, displayed as 640p):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_BufVis.png" width="640px" />

HighResolution Buffer Visualization HDR Screenshot:<br/>
It's like the sample before but brighter and with .EXR file extension...<br/>

Panoramic 360 Screenshot (scaled from 2K to 1K, displayed as 640p):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_Pano.png" width="640px" /><br/>

Stereoscopic VR Screenshot (scaled from 2K to 1K, displayed as 640p):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_VR.png" width="640px" /><br/>

Cubemap (scaled from 4096x2048 to 1280x640, displayed as 640p):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_Cubemap.jpg" width="640px" /><br/>

3DPhoto For Facebook (sample from 2k x 2 images [FinalColor 29.1Mb + SceneDepth 745KB], captured as 560p MP4, converted to 100MB GIF, optimized to 1/4 frames, compressed to 24MB GIF, displayed as 640p):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_3DPhoto.gif" width="640px" /><br/>

## Filters

Blur:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FBlur.png" width="640px" /><br/>

Blur Fast:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FBlurFast.png" width="640px" /><br/>

Black & White:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FBW.png" width="640px" /><br/>

ColorBlind:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FColorBlind.png" width="640px" /><br/>

Contrast:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FContrast.png" width="640px" /><br/>

CRT:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FCRT.png" width="640px" /><br/>

Curve:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FCurve.png" width="640px" /><br/>

Fade Distance:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FFadeDistance.png" width="640px" /><br/>

Fade Sphere:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FFadeSphere.png" width="640px" /><br/>

Flat Colors:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FFlatColors.png" width="640px" /><br/>

Gaussian Blur:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FGaussianBlur.png" width="640px" /><br/>

Greyscale:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FGreyscale.png" width="640px" /><br/>

Greyscale Back:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FGreyscaleBack.png" width="640px" /><br/>

Greyscale Front:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FGreyscaleFront.png" width="640px" /><br/>

Hue Shift:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FHurShift.png" width="640px" /><br/>

Impress:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FImpress.png" width="640px" /><br/>

Isolate Color:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FIsolateColor.png" width="640px" /><br/>

Kuwahara (Oil Painting):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FKuwahara.png" width="640px" /><br/>

Outline (Cartoon or Comics):<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FOutline.png" width="640px" /><br/>

Pixelated:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FPixelated.png" width="640px" /><br/>

Retro:<br/>
<img src="https://raw.githubusercontent.com/DarknessFX/PhotoModeFX/main/.git_img/PMFX_FRetro.png" width="640px" /><br/>

# Versioning
v1.0 - Full Filters Tab with 21 filters, hided Sticker and Pose tab (feature creep, maybe in future). Full release.<br/>
v0.7.1 - Added HDRHistogram to Dev Tab, Fixed UI bugs, fine tune in some default values.<br/>
v0.7 - Included Filters Tab settings and controls. Moved UI Events to a Component to reduze PMFX blueprint file size.<br/>
v0.6 - Fixed "Cannot destroy CineCameraComponent" on exit. Better camera UI and positioning.<br/>
v0.5.2 - Fixed the License "Copyleft" on ReadMe to "Unlicense - Public Domain - Free for everyone and any use".<br/>
v0.5.1 - Small improvements on Panoramic+Stereoscopic default settings in Dev Tab.<br/>
v0.5 - Included RayTracing Tab settings and controls.<br/>
v0.4 - Included Effect Tab settings and controls.<br/>
v0.3 - 3DPhoto Material prefix. Screenshots samples to ReadMe.<br/>
v0.2 - New 3DPhoto (for Facebook) capture and settings. Fix on camera detection for pawns without camera component.<br/>
v0.1 - Alpha released.

## TODO

- Files and instructions to install as an Engine Template / "Add Feature or Content Pack" to easily add to any project.

## Credits

Unreal Engine by Epic Games - https://www.unrealengine.com/ .<br/>
Video trailer uses UE4 Hour Of Code by Steve Isaacs, Brian Dickman and Ian Southwell - https://www.unrealengine.com/en-US/blog/learn-how-to-code-with-unreal-engine .<br/>
Screenshot samples uses UE4 Detective Office by Justin Mohlman - https://www.unrealengine.com/en-US/onlinelearning-courses/build-a-detectives-office-game-environment .<br/>
GIF video by 3dnchu <a href="https://twitter.com/ymt3d" target="_blank">@ymt3d</a> - https://3dnchu.com/archives/photomodefx-for-ue4/ .<br/>
Filter BlurFast (adapted) from TouchKey9691 - https://forums.unrealengine.com/community/community-content-tools-and-tutorials/28458-radial-blur-postprocess-material?p=1541025#post1541025 <br/>
Filter CRT (adapted) from - https://babylonjs.medium.com/retro-crt-shader-a-post-processing-effect-study-1cb3f783afbc and https://www.shadertoy.com/view/XtlSD7 <br/>
Filter GaussianBlur (adapted) from https://www.raywenderlich.com/57-unreal-engine-4-custom-shaders-tutorial <br/>
Filter Kuwahara (adapted) from https://www.raywenderlich.com/100-unreal-engine-4-paint-filter-tutorial <br/>
Filter Pixelated (adapted) from 8 Bit Pixellize in Unreal Engine 4 - https://www.youtube.com/watch?v=GLJC1qG3oK4 <br/>
Filter Retro (adapted) from @AlanNoon - https://twitter.com/AlanNoon/status/1297774377547845632 <br/>

## License

@Unlicense - Public Domain - Free for everyone and any use. <br/><br/>
DarknessFX @ <a href="https://dfx.lv" target="_blank">https://dfx.lv</a> | Twitter: <a href="https://twitter.com/DrkFX" target="_blank">@DrkFX</a> <br/>https://github.com/DarknessFX/PhotoModeFX
