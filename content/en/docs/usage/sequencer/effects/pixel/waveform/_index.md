---
title: Waveform
author: Vixen Team
description: Creates an effect that fills a display element with color based on the audio.
aliases: [/vixen-3-documentation/sequencer/effects/waveform/]
---

---

### Overview

Creates an effect that fills a display element with color based on the audio.

---

### Audio Sensitivity Range

* **Gain** - This adjusts the sensitivity of the effect to the audio volume.

* **High Pass Filter** - Applies a high pass filter to the audio before processing. 
                         A high pass filter allows frequencies above the defined threshold to pass while blocking everything below it. 
                         This represents the low end cutoff of the audio.

* **High Pass Frequency** - The frequency (in Hz) to use for the High Pass Filter. This value should be lower than that of the Low Pass Filter if it is being used.

* **Low Pass Filter** - Applies a low pass filter to the audio before processing. 
                        A Low Pass filter allows frequencies below the defined threshold to pass while blocking everything above it. 
                        This represents the high end cutoff of the audio.  

* **Low Pass Frequency** - The frequency (in Hz) to use for the Low Pass Filter. This value should be greater than that of the High Pass Filter if it is being used.

* **Normalize** - Applies an audio normalizing filter to the audio before it is analyzed for use in the effect. This should be enabled for most uses.

* **Zoom** - Scales the visual response to the audio.
            

---

### Response Speed

* **Scroll Speed** - How fast the color scrolls across the display element.

* **Attack Time** - How fast the effect responds to the audio. This adjusts the slope of the leading edge of the wave.

* **Decay Time** - How long the effect lingers on the audio before dropping back down. This is the slope of the trailing edge of the wave.


---

### Color

* **Color Handling** - Controls how the color is handled.
    * _Linear_ - Applies a standard Green-Yellow-Red gradient to the string. When this option is selected, The Green and Red position sliders will be available to adjust the threshold where the color transitions. 
    * _Discrete_ - Applies a standard Green-Yellow-Red gradient to the string using discrete colors. When this option is selected, the Green and Red position sliders will be available to adjust the threshold where the color transitions. 
    * _Custom_ - Uses a custom gradient to define the color range. Set up the custom gradient in the Color box below.

* **Custom Gradient** - Controls the color of the effect.

* **Green Gradient Position** - Controls the stop point for the green color in the gradient.

* **Red Gradient Position** - Controls the stop point for the red color in the gradient.

* **Reverse** - Reverses the direction of the meter.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

### Depth

* **Levels Deep** - Determines at which element grouping level to apply the effect.

---

