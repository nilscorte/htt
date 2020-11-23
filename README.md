# htt
## Hubs Theater Tools

Hubs Theater Tools are currently developed by Nils Corte (Coding) and Roman Senkl at the [Academy for Theatre and Digitality](https://theater.digital/) in Dortmund.
Their purpose is to expand [Mozilla Hubs](https://hubs.mozilla.com) with an easy to use motion capturing and playback tool for hubs avatars.
Furthermore our long time goals are support for Inverse Kinematics and full body tracking / eye tracking / facial tracking as these are vital parts to bring the performers expressions to life.

Why Hubs? Because we love HUBS!!! It's build on [THREE.js](https://threejs.org/) using [AFRAME](https://aframe.io) and works with all webvr compatible browsers.

If you want to visit us (or our virtual selves): Visit our [virtual lab](https://hubs.mozilla.com/3S5crQY).

## Considerations

Want to know which VR-Systems are supported by which browser: https://webvr.rocks/

> Controllers with 6 degrees of freedom (6DoF) have both rotational and positional tracking. Unlike controllers with 3DoF which are constrained to orientation, controllers with 6DoF are able to move freely in 3D space. 6DoF allows us to reach forward, behind our backs, move our hands across our body or close to our face. Having 6DoF is like reality where we have both hands and arms. 6DoF also applies to the headset and additional trackers (e.g., feet, props). Having 6DoF is a minimum for providing a truly immersive VR experience.
(https://aframe.io/docs/1.0.0/introduction/interactions-and-controllers.html#adding-6dof-controllers-vive-controls-oculus-touch-controls)

This beeing said we decided to use 6DoF (six degrees of freedom) Controller components to record and playback the movement of our performers.
HTC Vive and Oculus Rift with Touch provide 6DoF and controllers for both hands. 
HTC Vive also provides trackers for tracking additional objects in the real world into VR.

## Clone Hubs Repository 

In order to playback hubs avatars via the querystring parameter ?bot=true we first need to install some tools (github, nodejs, hubs-master, some node libraries)

1. Open a terminal and find out if you have already installed git (to get git goto https://git-scm.com/downloads)
> git --version

2. Find out if you have already installed nodejs (version 12 or above is recommanded)
> node -v (to get nodejs goto https://nodejs.org/en/download/)

3. npm is distributed with Node.js- which means that when you download Node.js, you automatically get npm installed on your computer. To be on the safe side lets check if npm is installed by typing
> npm -v

4. To get the latest version of npm
> npm install npm@latest -g

5. Next clone mozilla hubs repository to your computer
> git clone https://github.com/mozilla/hubs/

6. Change directory to [your repo directory]/scripts/bot

7. Run Puppeteer script  
> node run-bot.js --url=hubs.mozilla.com/[your room] --audio=[your].mp3 --data=[your].json

## Peppers Holosuite - Hubs Avatar Recorder

[Requirements] Windows 10 [for 3D Motion Capturing] VR capable 3D graphics card, HTC Vive System, SteamVR

Features: Motion Capturing, Audio Recording (experimental), Import/Export to Mozilla Hubs Replay compatible .json (converting left handed -> right handed coordinate system)
coming soon: Export Filter (Formations, Slow Motion, Time Lapse)

![Preferences](/images/preferences.png)

Install: 
1. Download [Hubs Avatar Recorder](https://phsuite.de/downloads/har.zip) and unpack the content into a folder of your choice
2. Download and install [SteamVR](https://store.steampowered.com/app/250820/SteamVR/)
3. Turn on your HTC Vive Hardware and launch har.exe

Configuration:
1. Choose any HTC Vive Devices (HMD, Controller, Tracker) and assign them to Avatars Head and Hands. (Hint: Before you start Motion Capturing make sure the controllers/trackers are in the correct hand!)
2. Choose Audio Capture Device
3. Set Length of Audio Recording (if you record beyond the limit the beginning will be overwritten)
4. Hit start

Warranty:
Peppers Holosuite - Hubs Avatar Recorder is currently developed at the Akademie für Theater und Digitalität Dortmund. We do not warrant that this pre-release software will meet your requirements, the operation or output of the pre-release software will be error-free, accurate, reliable, complete or uninterrupted. Peppers Holosuite is not obligated to support, update or upgrade the Pre-Release Software.
