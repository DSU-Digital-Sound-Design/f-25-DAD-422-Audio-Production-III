+++
title = "Ambisonics Recording"
outputs = ["Reveal"]
[reveal_hugo]
theme = "moon"
margin = 0.2
+++

# First-Order Ambisonics (FOA)

ref: [The Double Mid-Sides Array](https://www.soundonsound.com/techniques/double-mid-sides-array)

{{% note %}}
Essentially based on similar considerations as MS, one can define first-order Ambisonic recording. For 2D recordings, a Double-MS microphone arrangement is suitable and only requires one more microphone than MS recording: a front-back oriented figure-of-eight microphone. The scheme is extended to 3D first-order Ambisonics by a third figure-of-eight microphone of up-down aiming.

The Double Mid-Sides (DMS) microphone array is a versatile technique for recording spatial information in a sound field. It is an extension of the Mid-Sides (MS) microphone array, which uses two microphones: a cardioid microphone for the mid channel and a figure-8 microphone for the side channel. The mid microphone captures the sound pressure directly in front of it, while the side microphone captures the difference in sound pressure between the left and right sides.

The DMS array adds a third figure-8 microphone, which is oriented in an up-down direction. This allows the DMS array to capture the difference in sound pressure between the front and back, left and right, and up and down directions. This information can then be used to reproduce the sound field over a variety of speaker configurations, including stereo, surround sound, and binaural audio.

The DMS array is a good choice for recording a variety of sound sources, including music, vocals, and sound effects. It is also a good choice for recording in a variety of environments, including studios, concert halls, and outdoor locations.

**Advantages of using the DMS array:**

* It is a versatile microphone array that can be used in a variety of situations.
* It is a good choice for recording stereo sound.
* It can be used to create immersive audio experiences for a variety of applications, including music production, film and television production, and virtual reality.

**Disadvantages of using the DMS array:**

* It is more complex to set up and use than the MS microphone array.
* It requires three microphones, which can be more expensive than the two microphones required for the MS microphone array.

**Overall, the DMS microphone array is a versatile and powerful tool for recording spatial sound. It is a good choice for a wide range of applications, and it is widely supported by audio software and hardware.**
{{%/ note %}}


---

### Native 2D Ambisonic recording (Double-MS)

![](native-2d-foa.png)

{{% note %}}
To record the Ambisonic channels W, X, Y, one can use a Double-MS arrangement
{{%/ note %}}

---

### 2D Ambisonic recording with four 90◦-angled cardioids

![](2d-foa-cardiod.png)

---

### 2D Ambisonic recording with three 120◦-angled cardioids

![](2d-foa-2.png)

---

### Native 3D Ambisonic recording (Triple-MS)

![](native-3d-foa-1.png)

---

### 3D Ambisonic recording with a tetrahedral arrangement of cardioids

![](tetrahedral-array-four-cardiods.png)

---

# Higher-Order Ambisonics (HOA)

---

### Eigenmike®

![](eigenmike.png)

[Sound Demos](https://mhacoustics.com/demos) - listen with headphones, we'll listen to some in studio B later.

{{% note %}}
This microphone can create higher order ambisonics signals from its 32 microphones. able to achieve **fourth-order Ambisonics**.
{{%/ note %}}

---

[Sound Demos](https://mhacoustics.com/demos) - listen with headphones, we'll listen to some in studio B later.

---

### Octomic

[Octomic](https://www.core-sound.com/products/octomic)

{{% note %}}
In 2018 US-company Core Sound, which also produces the ‘TetraMic,’ has come up with the first commercially available ‘Second-Order Ambisonic’ (SOA) microphone: the ‘OctoMic’ is made up of 8 capsules with cardioid characteristics, which apparently allows not only for a broad range of first- and second-order microphone patterns but also delivers more accurate spatial impression and localization due to better signal separation between the capsules.
{{%/ note %}}

---

### Zylia

[ZM-1](https://www.zylia.co/zylia-zm-1-microphone.html)

{{% note %}}
Around the same time, Polish company Zylia has released their third-order Ambisonics (TOA) microphone ‘ZM-1,’ based on 19 omni-directional capsules. Accompanying software enables beamforming and the creation of useful microphone patterns for 2D and 3D Audio use, including binaural signal generation.
{{%/ note %}}
