---
title: "Atmos Mix"
---

You will use Logic Pro X to create a Dolby Atmos mix. You have the option to choose between two projects:

1. **[Aiguille Rouge's Bebe Grand](https://cambridge-mt.com/ms/mtk/#BabeGrand)**
2. **[The Film Lambs](https://dakotastateuniversity-my.sharepoint.com/:u:/g/personal/tate_carson_dsu_edu/EcGU4cdZ10ZNiSfQi1nFA9MBwZY9WMR_pZnY7I5Nv0VkFg?e=NOo8Rt)**

For either project, start by converting it into an Atmos mix format. Ensure that the settings are **24 bit / 48 kHz / 24 fps**.

## Initial Setup

1. **Set Project Audio Format**:

   - Open Logic Pro X and go to `Preferences -> Audio`.
   - Set the input/output settings to **24-bit, 48 kHz, 24 fps**.

2. **Configure Spatial Audio Settings**:

   - Navigate to `Project Settings -> Audio -> General`.
   - Under "Spatial Audio," select **Dolby Atmos**.
   - Set "Surround Format" to **7.1.2**.

## Mixing Guidelines

### Using Bed and Object Tracks

All tracks should be panned using either the `Surround Panner` or the `3D Object Panner`.

1. **Bed Tracks**:

   - Use for ambient or foundational audio, creating a consistent sonic environment. Ideal for elements that will remain static in the mix.
   - Set to **Surround Panner**.

2. **Object Tracks**:

   - Use for sound elements that move within the 3D space, or for elements that need a distinct point source with a strong locative quality.
   - Set to **3D Object Panner** and add panning automation for dynamic movement.

> **Tip**: Avoid stereo panning modes for an authentic Atmos mix.

### Monitoring in 7.1.4

Ensure that you are monitoring in **7.1**.4 Adjust this setting in the **Dolby Atmos Renderer plugin**.

### Adding Panning Automation

Add panning automation to at least two tracks to create spatial movement and enhance immersion.

### Checking Loudness Levels

1. **Master Track Analysis**:

   - On your Master track, use level and loudness meters to ensure that your mix matches the Dolby Atmos loudness standards of **-18 LUFS-I** and **-1 dbTP**.

2. **Meter Placement**: Position the meters **after the Dolby Atmos Render plugin** to accurately capture the levels of object tracks.

### Saving and Exporting

1. **Save Project File**: Save your project file in the "DAD 422 - Dolby Atmos Aiguille Rouge Turn-in Folder" if mixing *Bebe Grand*, or in the designated *Lambs* folder.

2. **Export ADM BWF File**: Export and save an **ADM BWF file** for distribution or submission. This file is essential for uploading your mix to a distributor for consumer playback.

