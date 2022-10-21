---
title: "Atmos Music mix - Ocean Eyes"
---

You will use Logic Pro X to create an Atmos mix of Billy Eilish's _Ocean Eyes_. You can find the stereo mix on the studio b computer in the demo folder. You will need to convert it into an Atmos mix to start. Make sure it is 24 bit / 48 kHz / 24 fps.

In Project Settings -> Audio -> General, set _Spatial Audio_ to _Dolby Atmos_, then set the _Surround Format_ to _7.1.2_. Use a combination of bed and object tracks to create a convincing atmos mix. Don't use any stereo panning modes.

> Make sure you are monitoring in 7.1. You can change this in the Dolby Atmos Renderer plugin.

To convert from a stereo panner, change the output routing to _Surround_. This will now give you a Logic _Surround Panner_. Right click and select _3D Object Panner_ if you want pan this track with an object channel.

Add panning automation to at least two tracks.

On your Master track use level and loudness meters to check that your mix matches the Dolby Atmos music standard loudness of -18 LUFS-I and -1 dbTP. Make sure these are placed **after** the Dolby Atmos Render plugin so that they are metering the object tracks.

Save your **project file** into the folder in studio b called _DAD 422 - Dolby Atmos Ocean Eyes Turn-in Folder_. Also save an **exported ADM BWF file**. This is the file that you would upload to a distributor if you were distributing your mix for consumers.
