+++
title = "Distance Perception in Mono"
outputs = ["Reveal"]
[reveal_hugo]
theme = "moon"
margin = 0.2
+++

## Acoustical and Psychoacoustic Properties for Mono Sound Walk

- Understand acoustical properties affecting distance perception.
- Learn psychoacoustic cues to simulate depth and movement.
- Apply sound design techniques in the Mono Sound Walk project.
- Explore practical strategies for spatial simulation in mono sound.

{{% note %}}

- Introduce the concept of using sound to simulate distance and spatial awareness, focusing on a mono format.
- Highlight the importance of understanding both acoustical and psychoacoustic principles to create depth and movement.
- Mention that these concepts will directly apply to the Mono Sound Walk project.
- Emphasize that today's session will cover practical techniques for simulating spatial depth in mono soundscapes.

{{%/ note %}}

---

[Automation Review](https://www.reapertips.com/post/10-automation-shortcuts-in-reaper)

---

# Let's find a walking tour video to use for these examples. 

---

## Acoustical Properties of Distance Perception

- Sound level (intensity) decreases with distance.
- High frequencies attenuate faster over distance.
- Reverberation increases in enclosed spaces.
- Direct-to-reverberant ratio affects distance perception.

{{% note %}}

- Explain how sound intensity diminishes as the distance between the listener and the source increases, affecting perception.
- High-frequency sounds lose energy more quickly than low frequencies, creating a muffled effect as sound travels.
- Reverberation plays a key role in simulating distance, especially in indoor spaces.
- The direct-to-reverberant ratio is a critical cue, where more reverb and less direct sound imply greater distance.

{{%/ note %}}

---

## Sound Level (Intensity)

- Sound intensity decreases by 6 dB per doubling of distance.
- Quieter sounds suggest greater distance.
- Use volume automation to simulate sound proximity.

{{% note %}}

- Sound intensity follows the inverse-square law: it decreases by approximately 6 dB for every doubling of distance, helping to simulate how far away a sound is.
- In sound design, reducing the volume of sounds can effectively create a sense of distance.
- Students should apply volume automation in the Mono Sound Walk to make sounds appear closer or farther away, mimicking real-world acoustics.

{{%/ note %}}

---

## REAPER Automation Envelope Shapes

- Linear → Corresponds to Linear
- Square → No direct counterpart (instant step)
- Slow Start/End → Corresponds to S-Curve
- Fast Start → Corresponds to Exponential Growth

{{% note %}}

- The linear envelope in REAPER creates a straight, constant-rate change, ideal for smooth, predictable volume transitions.
- Square shapes lead to abrupt, instant changes, often used for sudden sound events.
- Slow Start/End shapes resemble S-curves, creating gradual, natural transitions at the beginning and end.
- Fast Start mimics exponential decay, where volume drops rapidly at first and slows down later, useful for fast fades.

{{%/ note %}}

---

## REAPER’s Fast End and Bezier Envelopes

- Fast End → Corresponds to Exponential Decay (Similar to Logarithmic)
- Bezier → Customizable (Linear, Logarithmic, Exponential, or S-Curve)
  - Bezier allows full control over transitions
  - Great for detailed audio shaping

{{% note %}}

- The fast end shape mimics exponential growth, with sound gradually increasing and then rapidly intensifying.
- Bezier curves offer flexibility, letting you tailor the shape to any transition, from smooth fades to sharp changes.
- Bezier curves are ideal for complex, dynamic movements.
- Use this flexibility for precise audio transitions in any scenario.

{{%/ note %}}


---

# Volunteer to try volume automation?

---

## Frequency Response (High-Frequency Roll-off)

- High frequencies attenuate faster than low frequencies.
- Distant sounds lose high frequencies, creating a "muffled" effect.
- Use low-pass filtering to replicate distant sounds.

{{% note %}}

- High frequencies diminish more rapidly over distance due to atmospheric absorption, making distant sounds softer and less defined.
- Low-pass filters in a DAW can simulate this effect, helping to create realistic distant sounds in the Mono Sound Walk.
- Encourage students to think about how reducing high frequencies alters the perception of distance in their soundscapes.

{{%/ note %}}

---

# Volunteer to try low-pass filtering?

---

## Reverberation and Echoes

- Reverberation increases with distance in enclosed spaces.
- A higher reverb level implies greater distance from the sound source.
- Adjust reverb to reflect environmental conditions.

{{% note %}}

- Reverberation is a vital acoustical cue for distance, especially in indoor or enclosed spaces, where sound reflects off walls and surfaces.
- In sound design, increasing the reverb as a sound source moves away from the listener creates the perception of a larger space.
- Students should experiment with different reverb settings to simulate various environments in their Mono Sound Walk.

{{%/ note %}}

---

## Simulating Distance with Reverb

- Near sounds: minimal reverb, dry sound.
- Far sounds: higher reverb, muffled sound.
- Adjust wet/dry ratio to simulate depth.
- EQ changes for high and low frequencies.

{{% note %}}

- Close sounds are typically more direct, while far sounds feel distant due to more reverb and reduced clarity.
- By altering the wet/dry mix, you can create a sense of proximity or distance, making the sound feel near or far.
- Increasing reverb makes a sound feel more distant as it simulates bouncing off surfaces.
- EQ adjustments help simulate distance by mimicking how sound loses clarity over space.

{{%/ note %}}

---

## Starting Reverb Settings for Distance

- Close proximity: Short reverb time, low wet/dry mix.
- Medium distance: Moderate reverb, slight high-frequency damping.
- Far distance: Long reverb, heavy high-frequency roll-off.
- Adjust pre-delay for spatial reflection.

{{% note %}}

- For close proximity, use minimal reverb and pre-delay to maintain the dry sound with clear mids and highs.
- In medium-distance settings, more reverb and slight EQ changes simulate a natural room tone.
- To create far distances, use long reverb and reduced clarity by dampening high frequencies.
- Pre-delay settings affect how the sound reflections are perceived, adding a sense of depth.

{{%/ note %}}


---

## Advanced Automation: Tail and Pre-delay

- Tail length: Adjust reverb tail for room size.
- Pre-delay: Automate for proximity changes.
- Combine wet/dry and pre-delay for complex depth.
- Simulate large spaces with longer reverb tails.

{{% note %}}

- Reverb tail length directly influences the perceived room size—long tails suggest large, open spaces.
- Pre-delay automation helps control the initial perception of sound distance.
- Blending changes in pre-delay with wet/dry ratio creates intricate space and depth effects.
- By manipulating the reverb tail, you can simulate a shift from a small room to a vast outdoor environment.

{{%/ note %}}

---


# Volunteer to try reverb?

---

## Practice Tips for Simulating Distance with Echo or Delay Automation

- Use echo/delay to create a sense of distance
- Adjust delay time for close or distant effects
- Modify feedback to simulate multiple reflections
- Combine delay with reverb for natural depth

{{% note %}}

- Echo/delay replicates real-world sound reflections, where greater delay suggests a farther sound.
- Shorter delays (few milliseconds) for closer sounds, longer delays (50 ms to several hundred milliseconds) for distant ones.
- Higher feedback values create multiple reflections, mimicking large spaces.
- Reverb adds realism by simulating how sound reflects off surfaces in natural environments.

{{%/ note %}}

---

## Suggested Starting Settings for Delay Automation

- For close proximity (1-3 meters): 10-50 ms delay, 10-20% feedback
- For medium distance (3-10 meters): 50-150 ms delay, 30-40% feedback
- For long distance (10+ meters): 200-500 ms delay, 50-80% feedback
- Automation curves: adjust for linear or fast changes

{{% note %}}

- Close proximity: Use a delay time of 10-50 ms, with 10-20% feedback and a dry/wet mix of 20-30%. Keep reverb subtle or minimal.
- Medium distance: Set delay to 50-150 ms, 30-40% feedback, and dry/wet mix at 30-50%, with moderate reverb.
- Long distance: Increase delay to 200-500 ms, feedback to 50-80%, and dry/wet mix to 50-80%. Use larger reverb spaces for a more immersive effect.
- Automation curves adjust how quickly delay changes with sound movement.

{{%/ note %}}

---

# Volunteer to try delay?

---

## Motion and Dynamic Cues

- Changing sound level or frequency suggests movement.
- The Doppler effect simulates pitch changes as sound moves.
- Adjust sound properties dynamically to reflect movement.

{{% note %}}

- Dynamic cues, such as changes in volume or pitch, help convey movement in sound design.
- The Doppler effect, where pitch increases as a sound approaches and decreases as it moves away, is a powerful tool for simulating motion.
- Students can use these dynamic cues to create realistic movement and depth in their Mono Sound Walk projects, even without stereo sound.

{{%/ note %}}

---

# Volunteer to try Doppler effect?