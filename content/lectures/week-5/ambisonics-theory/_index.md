+++
title = "Ambisonics Introduction"
outputs = ["Reveal"]
[reveal_hugo]
theme = "moon"
margin = 0.2
+++

# Ambisonics

{{% note %}}

- **1970s:** Ambisonics was developed in the 1970s as a surround sound technology by British engineer Michael Gerzon and later refined by Peter Fellgett and others.

- **Spherical Sound:** Ambisonics aims to capture and reproduce audio in a spherical or three-dimensional manner, including both horizontal and vertical sound information.

- **B-Format:** The core of Ambisonics is the B-Format, which represents audio as a combination of spherical harmonic components (W, X, Y, Z). This format allows for flexible manipulation of sound directionality.

- **Encoding and Decoding:** Ambisonics involves encoding audio using B-Format during recording or synthesis and decoding it for playback through speaker arrays or virtual systems.

- **Immersion and Realism:** Ambisonics has been used in various applications, including music production, gaming, and virtual reality, to create immersive and realistic audio experiences.

- **Challenges and Adoption:** While Ambisonics offers a high degree of flexibility, its adoption has faced challenges due to the complexity of encoding and decoding, as well as the need for specialized equipment.

- **Modern Resurgence:** In recent years, Ambisonics has seen a resurgence in interest, driven by advancements in VR and 360-degree video, as well as software-based solutions for encoding and decoding.

- **Open Standards:** Efforts have been made to standardize Ambisonics, making it more accessible and compatible across different platforms and software.

- **Future Applications:** Ambisonics continues to be explored for applications like 3D audio for headphones, spatial audio for augmented reality, and improved audio experiences in various multimedia content.

- **Ongoing Research:** Research and development in Ambisonics continue to push the boundaries of spatial audio, aiming to provide more realistic and immersive soundscapes for listeners.
{{%/ note %}}

---

<iframe width="560" height="315" src="https://www.youtube.com/embed/X23hZNoSkUs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


---

### BBC R&D Ambisonics Intro

[Ambisonics and Periphony](https://www.bbc.co.uk/rd/blog/2010-03-ambisonics-periphony-audio-sound)

{{% note %}}
- Ambisonics is a system that can represent a sound-field at a single point in space.
- It has the potential to solve many of the problems with current surround sound systems, such as the need to create separate mixes for different speaker configurations.
- The BBC has conducted a number of experiments with Ambisonics, including recording The Last Night of the Proms.
- The results of these experiments are currently being analyzed.
{{%/ note %}}

---

## Principles

- Gerzon, Barton, Fellgett - main theoretical basis
- hierarchical approach to directional sound recording
- formats
  - A-format: microphone recording
  - B-format: studio equipment and processing
  - C-format: transmission
  - D-format: decoding and reproduction
  - UHJ - good for mono/stereo compatibility

{{% note %}}

- Ambisonics is a hierarchical approach to sound pickup, storage, transmission, and reproduction. This means that it can be used to create audio for any number of channels, from mono to stereo to surround sound with height information.
- The more channels used, the greater number of dimensions can be reproduced during playback.
- Ambisonics can be used to create surround sound recordings, which can then be played back on any speaker configuration, including 7.1, quad, or 5.1.

{{%/ note %}}

---

### Differences from stereo/quad

- Quad
  - is fixed to four speakers
  - Uses phantom images between two speakers
  - worse with off center listening
  - common "hole in the middle" problem
- Ambisonics
  - encodes from all directions, decodes to your loudspeaker setup

{{% note %}}

- Ambisonics encodes sounds from all directions in terms of pressure and velocity components.
- Ambisonics decodes these signals to a number of loudspeakers.
- Ambisonics uses psychoacoustically optimized shelf filtering above 700 Hz to correct for the shadowing effects of the head.
- Ambisonics uses an amplitude matrix to determine the correct levels for each speaker for the layout chosen.

{{%/ note %}}

---

- Ambisonic microphone:
    - Sennheiser AMBEO VR Microphone
    - RØDE NT-SF1
    - NEVATON VR
    - Zoom VRH-8 Ambisonic Microphone Capsule for H8 Recorder
    - Zoom H3-VR Handy Audio Recorder with Built-In Ambisonics Mic Array
    - Soundfield SPS200
    - Schoeps Double-MS
    - Josephson Engineering C700S

- Virtual source

{{% note %}}

- Ambisonic signals can be captured using an ambisonic microphone, such as the Calrec Soundfield.
- Ambisonic signals can also be created by artificially panning a mono signal and adjusting the ratios between the signals to place the sound in a specific position around the listener.
- For more information on mixing ambisonics, please see Daubney (1982) and Elen (1983).

{{%/ note %}}

---

### Signal formats - A format

![](a-format.png)

{{% note %}}
Remember there are four basic signal formats for ambisonics, **a, b, c and d.**

The A-format consists of the four signals from a microphone with four sub-cardioid capsules orientated as shown in Figure 4.14 (or the panpot equivalent of such signals).

The capsules are mounted on the four faces of a tetrahedron and match to left-front (LF), right-front (RF), left-back (LB) and right-back (RB), although two of the capsules point upwards and two point downwards.
{{%/ note %}}

---

### B format

![](b-format.png)

{{% note %}}
**B-format Ambisonics**

* Consists of four signals: W, X, Y, and Z
* W (omnidirectional) represents the pressure component of the sound field
* X, Y, and Z (figure-eight) represent the velocity components of the sound field in the forward, sideways, and upward directions, respectively
* Similar to the sum and difference format of two-channel stereo, where the B-format is made up of three orthogonal figure-eight components and an omni component

**Picking out the figure-eight and omni polar patterns**

* W: omni
* X: forward-facing figure-eight
* Y: sideways-facing figure-eight
* Z: upward-facing figure-eight

**Horizontal and vertical spatial information**

* W, X, and Y provide the horizontal spatial information
* Z provides the vertical spatial information

**Comparison to MS stereo**

* X: equivalent to M (mid) in MS stereo
* Y: equivalent to S (side) in MS stereo

**Recording options in the Zoom recorder**

* Can record directly to B-format with either FuMa or AmbiX encoding
* Can record in A-format

**Additional information**

* FuMa encoding is a more efficient way to store and transmit B-format audio signals than AmbiX encoding
* Encoding is not necessary if recording in FuMa

I hope this is helpful!
{{%/ note %}}

---


| Feature    | A-format                                    | B-format                                                |
| ---------- | ------------------------------------------- | ------------------------------------------------------- |
| channels   | 4                                           | 4                                                       |
| Signal rep | Raw output of ambisonic microphone capsules | Derived from A-format using mathematical transformation |
| Efficiency | Less efficient                              | More efficient                                          |
| Ease?      | More difficult to work with                 | Easier to work with                                     |


{{% note %}}
A-format and B-format are two ways of representing ambisonic audio signals.

A-format is the raw output of an ambisonic microphone. It is a set of four channels, each of which contains the signal from one of the microphone capsules.

B-format is a derived format that is more efficient and easier to work with than A-format. It is a set of four channels, but the signals in these channels are not the same as the signals in the A-format channels. The B-format channels are derived from the A-format channels using a mathematical transformation.

B-format is the preferred format for storing, transmitting, and processing ambisonic audio signals. It is also the format that is used by most ambisonic software and hardware.

Here is a table that summarizes the key differences between A-format and B-format ambisonics:

{{%/ note %}}

---

### A to B Conversion

- X = 0.5((LF – LB) + (RF – RB))
- Y = 0.5((LF – RB) – (RF – LB))
- Z = 0.5((LF – LB) + (RB – RF))
- W = 0.5(LF + LB + RF + RB)

{{% note %}}
The A-to-B ambisonic conversion is the process of converting the raw output of an ambisonic microphone (A-format) into a more efficient and easier-to-work-with format (B-format).

The conversion is performed using a mathematical transformation that combines the four A-format signals into four B-format signals. The B-format signals are derived as follows:

* **W (omnidirectional)**: The sum of all four A-format signals
* **X (forward-facing figure-eight)**: The difference between the left and right A-format signals
* **Y (sideways-facing figure-eight)**: The difference between the front and back A-format signals
* **Z (upward-facing figure-eight)**: The difference between the top and bottom A-format signals

The A-to-B conversion is typically performed in software, but it can also be implemented in hardware.

Here are some of the benefits of using B-format over A-format:

* B-format is more efficient to store and transmit, as it uses less data.
* B-format is easier to work with, as it is based on a more intuitive representation of the sound field.
* B-format is compatible with most ambisonic software and hardware.

{{%/ note %}}

---

### C format - aka UHJ

![](c-format.png)

{{% note %}}
**C-format Ambisonics**

* Consists of four signals: 
  * L: Left channel
  * R: Right channel
  * T: Top channel
  * Q: Quad channel

* Conforms to the UHJ (Universal HJ) hierarchy, which is a system for encoding multichannel ambisonic information into two or three channels while retaining good mono and stereo compatibility
* Used for mono or stereo-compatible transmission or recording
* A useful consumer matrix format

**UHJ**

* Allows us to listen to ambisonics on stereo loudspeakers
* Can be decoded using the UHJ decoder in the ATK

**Summary**

C-format ambisonics is a useful format for transmission or recording ambisonics in a mono or stereo compatible way. It is based on the UHJ hierarchy, which allows us to listen to ambisonics on stereo loudspeakers.

{{%/ note %}}

---

### D format - reproduction

- Speaker numbers
  - Four speakers give adequate surround sound
  - six provide better immunity against the drawing of transient and sibilant signals towards a particular speaker
  - eight may be used for full periphony with height.

{{% note %}}
**D-format Ambisonics**

* A format for decoding ambisonic audio signals for a specific speaker configuration.
* Not a separate ambisonics format, but rather a way of representing ambisonic audio in a way that is optimized for playback on a particular set of speakers.
* Example: Using a D-format decoder to decode an ambisonic recording into seven channels for a 7.1 surround sound system.
* Less commonly used than other ambisonics formats, such as B-format, but useful for applications where you need to decode ambisonic audio for a specific speaker configuration.
* Used in some virtual reality and augmented reality headsets, as well as in some home theater systems.
 

**Benefits:**
* Allows you to decode ambisonic audio for a specific speaker configuration, which can improve the immersive sound experience.
* Relatively efficient, so it can be used to transmit and store ambisonic audio without using too much bandwidth or storage space.

**Conclusion:**
D-format ambisonics is a practical and efficient format that can allow you to enjoy the full immersive sound experience of your ambisonic recording, especially if you need to decode it for a specific speaker configuration.
{{%/ note %}}

---

### Higher order Ambisonics

![](Spherical_Harmonics_deg3.png)

{{% note %}}
Here is a summary of higher order ambisonics in bullet points:

* Higher order ambisonics is a format for representing sound fields with a higher degree of accuracy than traditional ambisonics formats.
* It is based on the use of higher order spherical harmonics, which can be used to represent more complex sound fields.

Here are some of the challenges of using higher order ambisonics:

* Increased computational complexity
* Increased storage requirements
* Limited playback support

Visual representation of the Ambisonic B-format components up to third order. Dark portions represent regions where the polarity is inverted. Note how the first two rows correspond to omnidirectional and figure-of-eight microphone polar patterns.
{{%/ note %}}

---

## Current Developments

- Open Source Output format - [Opus 1.3](https://jmvalin.ca/opus/opus-1.3/)
- Corporate interest
  - Google - [Spatial Audio RPC](https://github.com/google/spatial-media/blob/master/docs/spatial-audio-rfc.md)
  - Youtube - [180 or 360 degree videos](https://support.google.com/youtube/answer/6178631?hl=en-GB) with [spatial audio](https://support.google.com/youtube/answer/6395969)
  - [Occulus audio](https://developer.oculus.com/documentation/native/audio-intro/)
  - Microphones - [Sennheiser Ambeo VR Mic](https://en-us.sennheiser.com/microphone-3d-audio-ambeo-vr-mic), [Zoom H3-VR](https://zoomcorp.com/en/us/handheld-recorders/handheld-recorders/h3-vr-360-audio-recorder/)
  - BBC Research on [ambisonics](https://www.bbc.co.uk/rd/search?query=Ambisonics&Type=All&=2020)

---

### Gaming

- [Unity](https://docs.unity3d.com/Manual/AmbisonicAudio.html), [Unreal](https://docs.unrealengine.com/5.0/en-US/native-soundfield-ambisonics-rendering-in-unreal-engine/)
- [Resonance Audio](https://resonance-audio.github.io/resonance-audio/discover/overview.html)
- [Steam Audio](https://valvesoftware.github.io/steam-audio/#learn-more)
- Battlefield 1 & Battlefield V - [Dev Talks video](https://www.youtube.com/watch?v=84EDwVHY2BY)
