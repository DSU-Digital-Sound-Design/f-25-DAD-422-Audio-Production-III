+++
title = "What is Dolby Atmos?"
outputs = ["Reveal"]
[reveal_hugo]
theme = "serif"
margin = 0.2
+++

<!-- Source: MixingInDolbyAtmos-#1HowItWorks(2021-0928) -->

# What is Dolby Atmos?

{{% note %}}
What was the point of this new standard? What problems did it try to solve?

We'll review some of the history we have already learned through the semester to answer this question, then delve deeply into the technical workings of atmos.
{{%/ note %}}

---

<!-- Mono -> Stereo -> Surround -> Immersive -->


<p style="font-size:50px;">
Mono &rarr; Stereo &rarr; Surround &rarr; Immersive
</p>

{{% note %}}
**Evolution of Audio Reproduction Technologies**

*Introduction*
Sound design has come a long way since its early beginnings, with innovations in audio reproduction technologies transforming the way we experience sound. This journey from mono to immersive audio has reshaped the field of sound design and enriched the auditory experiences we encounter in various media. In this overview, we will explore the key milestones in audio reproduction, from mono to immersive 3D audio.

**Mono - 1D Spot**

- *Historical Context*: In 1876, Alexander Graham Bell made significant strides in audio reproduction with the introduction of mono sound. At this early stage, audio, music, and sound were reproduced using a single speaker, which essentially consisted of a cone without electrical amplification.
- *Audio Channel*: Mono playback was characterized by its ability to convey only a single audio source through a single audio channel. This meant that the listener experienced sound from a singular point, lacking the spatial dimension that would later revolutionize audio.

**Stereo - 1D Line**

- *Innovation by Alan Blumlein*: The breakthrough into stereo sound, credited to Alan Blumlein in 1930, marked a significant advancement. It introduced the concept of a 1-dimensional sound field where sound could be perceived along a line rather than from a single point.
- *Phantom Source Phenomenon*: Stereo sound utilized two amplified speakers, allowing listeners to perceive sound sources between and outside the two speakers. This phenomenon, known as the Phantom Source, enriched the immersive quality of audio.

**Surround - 2D**

- *Early Implementations*: While Ray Dolby is often associated with the development of surround sound in the 1970s, earlier implementations can be traced back to the 1940s, exemplified by Disney's "Fantasia." The core idea was to extend sound beyond the front of the listener, incorporating side and back speakers.
- *2-Dimensional Sound Field*: Despite the term "surround," this technology primarily created a 2-dimensional sound field, enhancing the listener's experience by enveloping them with sound from multiple directions.

**Immersive - 3D**

- *Introduction of the Third Dimension*: Immersive sound, a significant leap forward, introduces a third dimension to the sound field. In addition to surround speakers at ear level, speakers above the listener contribute to the 3-dimensional soundscape.
- *Immersive Audio or 3D Audio*: This technology, often referred to as Immersive Audio, truly immerses the listener in a 3D sound environment. The listener is surrounded not only horizontally but also vertically, enhancing the realism and depth of the auditory experience.

**Conclusion**

The evolution of audio reproduction technologies, from mono to immersive 3D audio, showcases the remarkable progress in sound design. Each stage has added new dimensions to our perception of sound, providing sound designers with increasingly sophisticated tools to craft immersive auditory experiences in various media forms. Understanding this progression is essential for sound design professionals and students, as it informs the creative possibilities and technical aspects of contemporary sound design practices.
{{%/ note %}}

---

## Gray Area

- Mono vs. Stereo
- Speaker vs. Channel
- Surround vs. Immersive
- Immersive Audio
- Ambisonics

{{% note %}}
**Understanding Audio Terminology: Mono, Stereo, Surround, and Immersive**

*Introduction*
The world of audio is filled with terminology that can sometimes be confusing or misinterpreted. To gain clarity, it's important to understand the distinctions between various terms like mono, stereo, surround, and immersive audio. Let's break down these concepts with bullet points and provide context for each.

**Mono vs. Stereo**

- *Mono vs. Stereo Basics*: Mono typically refers to a single speaker, while stereo implies two speakers. However, the distinction is not solely based on the number of speakers.
- *Correlation Matters*: Stereo playback can be considered mono if both channels are fully correlated, meaning they play the same signal. In such cases, even though there are two speakers, the audio experience remains mono, lacking spatial separation.

**Speaker vs. Channel**

- *Surround Sound Misconception*: The presence of multiple speakers around the listener does not necessarily mean you are experiencing "Surround Sound." It merely indicates that you are surrounded by speakers.
- *Super-Mono Scenario*: If numerous speakers around you all reproduce the same signal, it technically results in a mono signal (1 audio channel) emanating from multiple speakers. This is sometimes referred to as "Super-Mono." To achieve genuine surround sound, individual speakers must handle different audio channels.

**Surround vs. Immersive**

- *Clarity in Terminology*: The terms "Surround" and "Immersive" audio can lead to confusion due to differing interpretations. In a technical sense, Immersive Audio surrounds the listener with sound, but it is not the same as "Surround Sound."
- *Surround Sound Configuration*: Surround Sound typically refers to configurations where all speakers are at ear level, often in setups like 5.1 or 7.1. This creates a 2-dimensional sound field with speakers around the listener.

**Immersive Audio**

- *Diverse Terminology*: The term "Immersive Audio" itself can be perplexing because it encompasses various technologies and meanings. Commonly used terms include Immersive Audio, 3D Audio, 360 Audio, Spatial Audio, and marketing-driven names invented by companies.
- *Sloppy Terminology*: Some individuals may even use the term "Surround Sound" to describe Immersive Sound, which is imprecise and can lead to misunderstandings.

**Ambisonics**

- *Specialized Recording Format*: Ambisonics is a term often associated with Immersive Audio. It specifically refers to a specialized recording format for full-sphere immersive sound capture. It's a technique used to capture audio in all directions, contributing to the immersive experience.

*Conclusion*
Understanding the nuances of audio terminology is crucial, especially in the context of teaching sound design to undergraduate students. The distinctions between mono, stereo, surround, and immersive audio not only enrich students' technical knowledge but also enhance their ability to communicate effectively in the field of digital sound design. Clarifying these concepts ensures that students are well-equipped to navigate the ever-evolving landscape of audio technologies.
{{%/ note %}}

---

![](timeline-1.png)

---

![](timeline-2.png)

---

## Key aspects of Dolby Atmos

- Workflow
- Immersive Sound
- Object-based Format
- Speaker Rendering
- Speaker Virtualization
- Binaural Rendering
- Sing Format Serves It All
- Dolby Atmos Everywhere

---

**Workflow**

<!-- ![](daw.png) ->  ![](renderer.png) ->  ![](panner.png) -> ![](pan-transmission.png) -->

<div style="display: flex; align-items: center; justify-content: center; font-size: 24px;">
    <img src="daw.png" alt="DAW" style="max-width: 250px;">
    <span>&#8594;</span>
    <img src="renderer.png" alt="Renderer" style="max-width: 250px;">
    <span>&#8594;</span>
    <img src="panner.png" alt="Panner" style="max-width: 250px;">
    <span>&#8594;</span>
    <img src="pan-transmission.png" alt="Pan Transmission" style="max-width: 250px;">
</div>



{{% note %}}
**Creating Atmos Mix with Your DAW:**

- **DAW Compatibility**: The good news is that you can utilize your favorite Digital Audio Workstation (DAW) for creating your Dolby Atmos Mix. This means you can continue to use the same editing and signal processing tools you're already familiar with.

**Utilizing the Dolby Atmos Renderer:**

- **Output Routing**: Instead of directing your audio to a traditional 2-channel or multichannel output bus within your DAW, you will route up to 128 audio Dolby Atmos channels to a specialized software application known as the Dolby Atmos Renderer. This step is essential for creating a truly immersive audio experience.

**3D Panning for Positioning:**

- **3D Panner**: On each track within your DAW, you'll utilize either the built-in 3D Panner (if available in your DAW) or the Dolby Atmos Music Panner Plugin. These tools are crucial for precisely positioning each track within the three-dimensional space of the Dolby Atmos soundscape.

**Transmission of Pan Data:**

- **Metadata Transmission**: The positioning information generated by the 3D Panner is not directly embedded into the audio signal itself. Instead, it is transmitted as separate metadata, similar to GPS coordinates, accompanying the audio signal that is routed to the Dolby Atmos Renderer. This metadata ensures that each audio element is correctly placed within the immersive audio environment, allowing for a dynamic and enveloping listening experience.

{{%/ note %}}

---

<div style="display: flex; justify-content: center; align-items: center;">
    <div style="text-align: center;">
        <img src="object-audio-r.png" alt="Object Audio Renderer (OAR)" style="max-width: 300px;">
        <p>Object Audio Renderer (OAR)</p>
    </div>
    <div style="text-align: center;">
        <img src="master-file.png" alt="Dolby Atmos Master File" style="max-width: 300px;">
        <p>Dolby Atmos Master File</p>
    </div>
</div>

{{% note %}}
**Dolby Atmos Object Audio Renderer (OAR):**

- *Speaker Configuration*: When working with Dolby Atmos, your studio speakers, including height speakers for a more immersive experience, are connected to the output of the Dolby Atmos Renderer.
- *Real-time Processing*: The key innovation lies in the Dolby Atmos Renderer software. It processes the 128 audio signals along with their individual pan information in real-time. This processing creates a true 3D sound field, ensuring that audio objects are accurately positioned in space. This 3D audio can be experienced either through the studio's speakers or as a 2-channel headphone mix using Binaural Rendering, which mimics the spatial perception of speakers even when using headphones.

**Dolby Atmos Master File:**

- *Recording the Atmos Mix*: In the context of Dolby Atmos, rather than the traditional practice of "bouncing" the mix to a standard WAV file, you "record" the Atmos Mix to a specialized Dolby Atmos Master File.
- *Preserving Separation*: The Dolby Atmos Master File retains the crucial separation of the 128 audio signals and their associated panning information. This separation is essential for maintaining the flexibility to make adjustments or record additional content "over" specific sections of the file. Essentially, it allows for ongoing editing and enhancements while preserving the integrity of the original audio signals and spatial data.

{{%/ note %}}

---

- Open Master File: ![](open-master.png)
- Delivery files

{{% note %}}
**Dolby Atmos Master Files: Unleashing the Full Potential of Immersive Audio**

Dolby Atmos Master Files play a pivotal role in delivering immersive audio experiences that captivate audiences in various media forms, from cinema to home entertainment. These master files represent a significant advancement in audio technology, allowing sound professionals to harness the full potential of spatial audio. Let's delve into the world of Dolby Atmos Master Files, exploring their significance, characteristics, and applications.

**Defining Dolby Atmos Master Files**

- *Spatial Audio Mastery*: Dolby Atmos Master Files are specialized audio files meticulously crafted to preserve the intricacies of immersive audio experiences. They encapsulate the spatial dimension, allowing sound objects to move dynamically through a three-dimensional sound field.

**Key Features and Components**

- *Audio Objects*: These master files encapsulate not only audio channels but also individual audio objects. Audio objects are discrete sound elements that can be dynamically positioned and moved within the 3D audio environment. Each object has its own metadata describing its spatial location and motion.

- *Panning Information*: Crucially, Dolby Atmos Master Files retain the panning information for audio objects. This information defines precisely where each sound element should be located within the three-dimensional space.

- *Flexibility and Post-Production*: One of the defining characteristics of Dolby Atmos Master Files is their flexibility. Sound professionals can make adjustments, add new audio objects, or modify the spatial placement of existing ones without compromising audio quality. This flexibility is especially valuable in post-production, where fine-tuning audio for different playback systems and environments is essential.

**Applications**

- *Cinema Soundtracks*: In the realm of cinema, Dolby Atmos Master Files are used to create captivating and immersive soundtracks. The ability to precisely position audio objects in a 3D space enhances the movie-watching experience, immersing viewers in the action and storytelling.

- *Home Entertainment*: Dolby Atmos Master Files have also made their way into home entertainment systems, enabling consumers to enjoy cinematic audio experiences in the comfort of their homes. High-end soundbars, AV receivers, and compatible streaming services support Dolby Atmos playback, bringing the magic of immersive audio to living rooms.

- *Gaming and Virtual Reality*: The gaming industry has embraced Dolby Atmos to provide players with heightened spatial awareness and immersive gameplay experiences. In virtual reality (VR) environments, the use of Dolby Atmos Master Files contributes to a more realistic and engaging audio landscape.

**Conclusion**

Dolby Atmos Master Files represent a paradigm shift in audio production and playback. They empower sound professionals to create immersive and dynamic audio experiences that transcend traditional stereo or multichannel formats. As technology continues to evolve, the role of Dolby Atmos Master Files in shaping the future of audio entertainment remains pivotal, offering audiences an unparalleled auditory journey through the realms of storytelling, gaming, and beyond.{{%/ note %}}

---

- Encoded Bitstream Files
- Consumer Playback
  ![](consumer-playback.png)

{{% note %}}
Dolby Atmos Master Files and Dolby Atmos Bitstream Files are distinct components of the Dolby Atmos audio ecosystem, serving different purposes and stages of the audio production and distribution process. Let's explore the key differences between the two:

**Dolby Atmos Bitstream Files:**

1. **Distribution Stage**: Dolby Atmos Bitstream Files are the encoded audio files that are distributed to consumers for playback. They are derived from Dolby Atmos Master Files but are optimized for specific playback systems.

2. **Encoded Format**: Bitstream files are encoded representations of the audio objects and metadata found in Dolby Atmos Master Files. They are compressed to reduce file size and are compatible with various delivery formats, including Blu-ray discs, streaming services, and gaming platforms.

3. **Metadata Preservation**: While bitstream files retain essential metadata for audio object positioning, they may not provide the same level of flexibility as Dolby Atmos Master Files in terms of real-time adjustment and dynamic mixing.

4. **Playback Compatibility**: Bitstream files require a compatible Dolby Atmos playback system for proper decoding and rendering. This includes Dolby Atmos-enabled AV receivers, soundbars, headphones, or dedicated home theater setups.

5. **Consumer Experience**: Consumers can enjoy immersive audio experiences using Dolby Atmos Bitstream Files, as the encoded audio objects are rendered in real-time to match the capabilities of their playback equipment.

In summary, Dolby Atmos Master Files are the source files used during audio production and offer maximum flexibility for sound professionals, while Dolby Atmos Bitstream Files are encoded versions optimized for distribution and playback on compatible systems, providing consumers with immersive and dynamic audio experiences.
{{%/ note %}}

---

## Three tasks of the Dolby Atmos Renderer

- Mixing
- Recording
- Exporting

---

![](mixing.png)

{{% note %}}
The Dolby Atmos Renderer plays a crucial role in the production and distribution of immersive audio experiences. It performs three key tasks: mixing, recording, and exporting. Let's delve into each of these tasks to understand their significance:

1. **Mixing**:
   - **Positioning Audio Objects**: One of the primary functions of the Dolby Atmos Renderer is to mix audio objects within a three-dimensional sound field. These audio objects can represent individual sound elements, such as dialogue, music instruments, or environmental sounds.
   - **Spatial Placement**: The Renderer allows sound engineers to precisely position audio objects in a 3D space. This spatial placement is achieved by leveraging metadata associated with each object, specifying its location and movement within the sound field.
   - **Immersive Sound**: By mixing audio objects in this way, the Renderer creates a truly immersive audio experience. Sound can come from all directions, including above and below the listener, resulting in a lifelike and engaging auditory environment.
   - **Real-time Adjustment**: Sound professionals can make real-time adjustments to audio object positions and movements during the mixing process, providing fine control over the spatial aspects of the audio.


{{%/ note %}}

---

![](recording.png)

{{% note %}}
2. **Recording**:

   - **Dolby Atmos Master Files**: Rather than traditional audio "bouncing" or rendering to a standard audio format like WAV, the Dolby Atmos Renderer is used to "record" the audio mix into a specialized format known as a Dolby Atmos Master File.

   - **Preserving Separation**: Dolby Atmos Master Files retain the individual audio objects and their associated metadata. This preservation of separation is crucial for post-production flexibility and ensuring that the 3D audio experience remains intact.

   - **Section Recording**: Sound engineers can record specific sections of the audio mix or extend the master file to accommodate additional content. This flexibility allows for future adjustments and enhancements without the need to recreate the entire mix.
   - 

{{%/ note %}}

---

![](exporting.png)

{{% note %}}

1. **Exporting**:

   - **Delivery Formats**: After the mixing and recording processes, the Dolby Atmos Renderer can export the audio content into various delivery formats suitable for distribution. These formats may include Dolby Atmos bitstream files for Blu-ray discs, streaming platforms, or gaming consoles.

   - **Compatibility**: The exported files are optimized for specific playback systems and are encoded to ensure compatibility with Dolby Atmos-enabled devices. This encoding ensures that the audio objects are rendered correctly in real-time during playback.

   - **Consistency**: Exporting audio content in Dolby Atmos formats maintains consistency with the original immersive audio experience created during mixing. It ensures that consumers can enjoy the same level of immersion and spatial accuracy when playing back the content on compatible systems.

In conclusion, the Dolby Atmos Renderer is a vital tool in the production and distribution of immersive audio content. It handles mixing to create immersive soundscapes, recording to preserve separation and flexibility, and exporting to deliver the content in formats suitable for various playback systems, ultimately enhancing the audio experience for audiences in cinema, home entertainment, gaming, and more.

{{%/ note %}}

---

## Immersive Sound

- *Immersive Sound Format*
- *Beyond 2-Dimensional Sound*
- *Sound Emanating from Above*
- *Surrounded and Immersed*

{{% note %}}
**Dolby Atmos: Revolutionizing Immersive Sound**

- *Immersive Sound Format*: Dolby Atmos represents a groundbreaking advancement in audio technology, offering an immersive sound format that transcends traditional audio setups.

- *Beyond 2-Dimensional Sound*: What sets Dolby Atmos apart is its ability to extend sound beyond the confines of a 2-dimensional space. Unlike conventional 5.1 or 7.1 audio configurations that primarily surround the listener with speakers at ear level, Dolby Atmos takes it a step further.

- *Sound Emanating from Above*: In Dolby Atmos setups, sound is not limited to speakers at ear level; it can also emanate from speakers positioned above the listener. This addition of overhead sound sources introduces a third dimension to the auditory experience.

- *Surrounded and Immersed*: This distinctive feature means that listeners are not merely surrounded by sound; they are truly immersed in it. It creates a sensory experience where audio elements can originate from all around and even above, offering a heightened level of realism and immersion.
{{%/ note %}}

---

## Height Speakers

![](2d-vs-3d.png)

---

## How many speakers?

![](speakers.png)

{{% note %}}
**Dolby Atmos Speaker Configurations: Options for Immersive Sound**

- *Immersive Sound Requires Speaker Immersion*: Achieving an immersive sound experience necessitates being immersed in speakers, where audio surrounds the listener, creating a captivating sensory experience.

- *Traditional Surround Formats*: Conventional surround sound formats typically utilize approximately six to ten speakers, providing a basic level of immersion by positioning speakers in front, on the sides, and in the back of the listener.

- *Dolby Atmos Extends Possibilities*: Dolby Atmos takes immersive audio to the next level by supporting up to 64 separate speaker channels. These speakers can be strategically mounted not only in the typical front, sides, and back locations but also on the ceiling, introducing the crucial overhead dimension.

- *Adaptability with Other Configurations*: Recognizing that not everyone can accommodate 64 speakers, Dolby Atmos offers adaptable configurations and innovative technological solutions. These configurations and "technological tricks" ensure that immersive audio experiences can be enjoyed even with more manageable speaker setups, making the technology accessible to a broader audience.
{{%/ note %}}

---

# Object-based Format

---

## Channel-based mixing

![](channel-based-mixing.png)

{{% note %}}
What we used in the previous month:

**Challenges of Traditional Speaker Representation in Stereo and Surround Formats**

- *Single Channel per Speaker*: In stereo and traditional surround sound formats, each individual speaker is represented by a dedicated channel, which is managed through your output busses.

- *Routing and Mixing Specific to Speakers*: This approach requires routing, panning, and mixing your audio tracks to specific speakers, making it necessary to precisely control the audio distribution across these channels.

- *Lack of Scalability*: Using a single channel per speaker is not scalable, meaning it becomes impractical when dealing with a large number of speakers. Adding more speakers for increased surround resolution adds complexity without making the system easily adaptable to other formats.

- *Limited Flexibility*: Traditional speaker representation lacks flexibility since it does not readily adjust to varying speaker configurations or adapt to different audio formats. This rigidity can be a limitation in optimizing audio experiences.
{{%/ note %}}

---

## Object-based mixing

- *Object-Based Track Assignment*
- *3D Positioning*
- *Metadata for Position*
- *Rendering with Object Audio Renderer*
- *Mixing to Location, Not Speaker*

{{% note %}}
**Dolby Atmos: Object-Based Audio Mixing and Playback**

- *Object-Based Track Assignment*: In a Digital Audio Workstation (DAW), audio tracks are assigned to "Objects." This shift from traditional channels to objects is a fundamental aspect of Dolby Atmos audio production.

- *3D Positioning*: The essence of Dolby Atmos lies in the ability to position audio signals precisely within a 3D space. Instead of thinking about directing sound to a specific speaker, audio professionals focus on placing the audio at a specific location in this three-dimensional soundscape.

- *Metadata for Position*: This positional data is crucial and is stored as metadata known as "Object Audio Metadata" within the audio file. It includes information about the object's position and movement in the 3D space.

- *Rendering with Object Audio Renderer*: During playback, the audio rendering process uses this metadata, often referred to as XYZ information, to reproduce the mix on a particular set of speakers. This process, known as "Rendering," is carried out by the "Object Audio Renderer," ensuring that audio objects are placed accurately within the listener's space.

- *Mixing to Location, Not Speaker*: In Dolby Atmos, the fundamental shift is that audio professionals mix to a specific location in the 3D space rather than targeting a particular speaker. This approach allows for a more dynamic and immersive audio experience, as sound objects can move freely throughout the 3D environment, creating a lifelike auditory landscape.
{{%/ note %}}

---

![](object-based-mixing.png)

---

### **Dolby Atmos Speaker Rendering: Expanding Compatibility**

- *Incompatibility of Existing Surround Formats*
- *Challenge of Adding More Speakers*
- *Magic of Dolby Atmos: Speaker Rendering*

{{% note %}}
**Dolby Atmos Speaker Rendering: Expanding Compatibility**

- *Incompatibility of Existing Surround Formats*: Traditional surround formats like 5.1 and 7.1 have a significant limitation – they only deliver their intended experience when played back on a speaker setup that matches the exact configuration in which they were mixed. This constraint restricts their usage to specialized movie theaters and dedicated home theater setups with the necessary space and financial resources.

- *Challenge of Adding More Speakers*: Simply adding more speakers to an immersive sound format would exacerbate the problem. It would still confine the format to movie theaters and make it even less practical for typical home theaters.

- *Magic of Dolby Atmos: Speaker Rendering*: Dolby Atmos introduces a groundbreaking solution known as "Speaker Rendering." This innovation is one of the key ingredients that sets Dolby Atmos apart. It addresses the compatibility issue by dynamically adapting the audio playback to the specific speaker configuration available, whether it's a state-of-the-art movie theater or a modest home theater system. This adaptability ensures that the Dolby Atmos experience remains accessible and enjoyable across a wide range of playback setups.
{{%/ note %}}

---

<img src="speaker-rendering.png" alt="Speaker Rendering Image" style="max-width: 300px; float: left; margin-right: 20px;"></img>

- *Adaptive Speaker Rendering*
- *Versatile Playback*
- *Optimizing Smaller Setups*
- *Accessible in Home Devices*
- *Intelligent Adaptation*

{{% note %}}

- *Adaptive Speaker Rendering*: Let's assume a movie is mixed on a big dubbing stage with a substantial Dolby Atmos configuration featuring up to 64 speaker channels.

- *Versatile Playback*: When this mix is played back in a big theater equipped with the same 64-speaker setup, it reproduces the audio faithfully. However, when the same mix is played in a smaller multiplex theater with only 20 speakers, Dolby Atmos employs its "rendering" capabilities. This process adapts the audio from 64 speakers to the available 20, ensuring that the immersive experience is maintained. For instance, a signal initially intended for both front and back height speakers is intelligently reconfigured for a single height speaker if necessary.

- *Optimizing Smaller Setups*: Dolby Atmos extends its adaptability further. If the mix is played on an even smaller speaker setup, the system dynamically adjusts to replicate the immersive sound experience as closely as possible on the available speakers.

- *Accessible in Home Devices*: The remarkable "Speaker Rendering" capability is not limited to large theaters. It's seamlessly integrated into any home Dolby Atmos playback device. Whether you have an expensive home theater system, an Audio Video Receiver (AVR) in your living room, or even a computer, tablet, or smartphone, you can enjoy the benefits of this technology.

**Not a Downmix!**

- *Intelligent Adaptation*: The Speaker Rendering process may seem akin to a traditional downmix procedure, but it's far more intelligent and capable. This is because Dolby Atmos operates on an Object-based model, as opposed to the Channel-based approach used in conventional surround formats.

{{%/ note %}}

---

## Speaker Virtualization

- Speaker Rendering: Using the panning data to route the audio signal to the speaker layout of the given room.
- Speaker Virtualization: Alternative to multi-speaker setups
  - Soundbars - [Samsung HW-Q90R](https://www.dolby.com/experience/sound-bars/hw-q90r/)
  - Smart Speakers - [Amazon Echo Studio](https://www.amazon.com/Echo-Studio/dp/B07G9Y3ZMC)
  - Computers
  - Tablets and smart phones
  - Binaural Rendering

{{% note %}}
**Speaker Rendering and Speaker Virtualization**

- *Speaker Rendering*: In Dolby Atmos, speaker rendering involves using panning data to precisely route the audio signal to the speaker layout of the specific room or playback system. This process ensures that audio objects are accurately reproduced and positioned, creating an immersive listening experience tailored to the environment.

- *Speaker Virtualization*: Speaker virtualization is an alternative approach to traditional multi-speaker setups, allowing immersive audio experiences in various playback devices, including:
  - Soundbars, such as the [Samsung HW-Q90R](https://www.dolby.com/experience/sound-bars/hw-q90r/)
  - Smart speakers, like the [Amazon Echo Studio](https://www.amazon.com/Echo-Studio/dp/B07G9Y3ZMC)
  - Computers
  - Tablets and smartphones
  - Binaural Rendering

- *Expanding Accessibility*: Speaker virtualization expands the accessibility of Dolby Atmos, making it available on a wide range of consumer devices, from compact soundbars and smart speakers to personal computing devices. It enables users to enjoy immersive audio without the need for elaborate multi-speaker configurations.
{{%/ note %}}

---

#### Single format

![](single-format.png)

{{% note %}}
The mix is done in Atmos a native immersive format. Surround formats are created during playback by the Dolby Atmos playback device.

You can even bring a mix back into a protools session.
{{%/ note %}}

---

### Atmos Everywhere?

- Cinema
- Home Theater
- Broadcast - sports events etc.
- Games - binaural rendering, could use head-tracking. competes with Ambisonics
- Cars - [Lucid Air](https://www.lucidmotors.com/air/connectivity)
- Music
- [Live Events](https://www.dolby.com/dolby-live-mgm/)

---

## DAW support

- Pro tools - the standard, tightest integration with the Dolby Atmos Renderer app.
- Nuendo - the first DAW with Dolby Atmos Renderer built-into the DAW.
- Logic Pro - limited support see Next Week
- DaVinci, Pyramix
- Other DAWs - can mix in Dolby Atmos using the Dolby Atmos Music Panner together with the Dolby Atmos Production Suite.

---

![](purchase.png)

{{% note %}}
Immersive Audio: This is the latest battleground that started in 2019 when the streaming service Tidal and Amazon Music offered music mixed in Dolby Atmos on their streaming service. In June 2021, Apple Music raised the bar when they entered the Immersive Audio game with "Spatial Audio with support for Dolby Atmos". Unlike the other services that charge for a premium for Dolby Atmos, Apple made it available to all their 72 million subscribers at no extra cost.
{{%/ note %}}

---

## Choices for streaming Atmos music

- Streaming services offering Dolby Atmos music:
  - Apple Music
  - Amazon Music HD
  - Tidal 
  - Spotify
  - YouTube Music
  - Netflix
- [More](https://youtube.com/playlist?list=PLC4e6_QLepbQEtBut4QBo4n7f0CiLsLUP&si=xAMBktrewp1GqitQ)

{{% note %}}
Here are some of the major music streaming services that currently offer Dolby Atmos music streaming:

- Apple Music - Apple Music has offered Dolby Atmos music streaming since June 2021. The Atmos catalog contains thousands of songs encoded in Dolby Atmos. It requires a compatible device.

- Amazon Music HD - Amazon Music HD provides access to songs available in Dolby Atmos through their 3D audio catalog. An Amazon Music HD subscription is required.

- Tidal HiFi - Tidal has a growing library of tracks in Dolby Atmos through its Tidal Masters catalog. It's available to Tidal HiFi subscribers.

- Spotify - Spotify launched Spotify Premium users access to a selection of Dolby Atmos music content in June 2022. The Atmos experience is limited to certain content and devices. 

- YouTube Music - YouTube Music provides a limited collection of songs available in Dolby Atmos for premium subscribers. Atmos playback requires compatible devices.

- Netflix - The Netflix app allows streaming select Dolby Atmos content like films and live performances for users with Dolby Atmos enabled devices.

- Windows Media Player - The Windows 11 Media Player app can play Dolby Atmos music files on compatible PCs through the Dolby Access app.

So in summary, Apple Music, Amazon Music HD, Tidal, Spotify, YouTube Music and Netflix are the major streaming services expanding their libraries with Dolby Atmos music content. Device and subscription compatibility is required.
{{%/ note %}}