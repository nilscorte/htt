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

## Install

In order to playback hubs avatars via the querystring parameter ?bot=true we first need to install some tools (github, nodejs, hubs-master, some node libraries)

1. Open a terminal and find out if you have already installed git (to get git goto https://git-scm.com/downloads)
> git --version

2. Find out if you have already installed nodejs
> node -v (to get nodejs goto https://nodejs.org/en/download/)

3. npm is distributed with Node.js- which means that when you download Node.js, you automatically get npm installed on your computer. To be on the safe side lets check if npm is installed by typing
> npm -v

4. To get the latest version of npm
> npm install npm@latest -g

5. 

