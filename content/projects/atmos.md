---
title: "Atmos Music mix"
---

You will use Logic Pro X to create an Atmos mix of [Aiguille Rouge](https://cambridge-mt.com/ms/mtk/#BabeGrand)'s Bebe Grand. You will need to convert it into an Atmos mix to start. Make sure it is 24 bit / 48 kHz / 24 fps.

In Project Settings -> Audio -> General, set _Spatial Audio_ to _Dolby Atmos_, then set the _Surround Format_ to _7.1.2_. Use a combination of **bed** and **object** tracks to create a convincing atmos mix. Don't use any stereo panning modes. 

> Make sure you are monitoring in 7.1. You can change this in the Dolby Atmos Renderer plugin.

To convert from a stereo panner, change the output routing to _Surround_. This will now give you a Logic _Surround Panner_. Right click and select _3D Object Panner_ if you want pan this track with an object channel.

Add panning automation to at least two tracks.

On your Master track use level and loudness meters to check that your mix matches the Dolby Atmos music standard loudness of -18 LUFS-I and -1 dbTP. Make sure these are placed **after** the Dolby Atmos Render plugin so that they are metering the object tracks.

Save your **project file** into the folder in studio b called _DAD 422 - Dolby Atmos Aiguille Rouge Turn-in Folder_. Also save an **exported ADM BWF file**. This is the file that you would upload to a distributor if you were distributing your mix for consumers.


## Guide to Creating an Atmos Mix in Logic Pro X

In this step-by-step guide, we'll walk through the process of creating an Atmos mix of "Aiguille Rouge's Bebe Grand" using Logic Pro X. Follow these instructions to ensure a successful Atmos mix:

### Step 1: Configure Logic Pro X Audio Settings

1.1. **Open Logic Pro X**: Launch Logic Pro X and open your project.

1.2. **Set Audio Format**:
   - In the Logic Pro X menu, go to Logic Pro X -> Preferences -> Audio.
   - Set the **Audio Input/Output**: 24-bit, 48 kHz, and 24 fps.

### Step 2: Configure Project Settings

2.1. **Spatial Audio Settings**: 
    * Navigate to Project Settings -> Audio -> General.
    * Under "Spatial Audio," select "Dolby Atmos."
    * In the same settings window, set the "Surround Format" to "7.1.2."

### Step 3: Use Bed and Object Tracks

All tracks should be panned with either the `Surround Panner` or the `3D Object Panner`

3.1. **Bed Tracks**:
   - These are foundational tracks with static or non-moving audio elements, providing a consistent sonic environment.
   - Use bed tracks for ambient or static elements in the mix. 
   - Bed tracks use the `Surround Panner`. 

3.2. **Object Tracks**:
   - These contain dynamic sound objects that can move independently within the three-dimensional sound space.
   - Employ object tracks for dynamic elements that you wish to have a more precise location in space.
   - Object tracks use the `3D Object Panner`

### Step 4: Monitor in 7.1

4.1. **Adjust Monitoring**: Ensure that you are monitoring in 7.1. You can change this setting in the Dolby Atmos Renderer plugin.

### Step 7: Add Panning Automation

6.1. **Create Automation**: Add panning automation to at least two tracks to control the spatial movement of sound elements within the Atmos mix.

### Step 8: Check Loudness Levels

7.1. **Master Track Analysis**: On your Master track, use level and loudness meters to check that your mix matches the Dolby Atmos music standard loudness of -18 LUFS-I and -1 dbTP.

7.2. **Placement of Meters**: Ensure that the meters are placed **after** the Dolby Atmos Render plugin in your signal chain. This will accurately meter the object tracks.

### Step 9: Save and Export

8.1. **Save Your Project**: Save your project file into the designated folder called "DAD 422 - Dolby Atmos Aiguille Rouge Turn-in Folder" within your studio workspace.

8.2. **Export ADM BWF File**: Additionally, save an **exported ADM BWF file**. This file is essential if you plan to distribute your Atmos mix to consumers or other platforms.

Following these renumbered step-by-step instructions will help you create a high-quality Dolby Atmos mix of "Aiguille Rouge's Bebe Grand" using Logic Pro X, incorporating both bed and object tracks to achieve an immersive audio experience. Ensure that your audio settings in Logic Pro X are correctly configured to match the specified format before starting your project. Remember to pay close attention to audio quality, routing, and loudness standards to achieve the best results.