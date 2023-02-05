---
title: VU Meter
author: Vixen Team
description: Create an effect that simulates a VU meter indicator light.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/vu-meter/]
---

---

### Overview

Create an effect that simulates a VU meter indicator light.
This is designed as a single element effect. The whole element group will be the same color at any point in time.
This effect, along with Vertical Meter and Waveform are all audio based effects. 
They use the actual audio associated with the sequence as the input for the effect. 
Because these effects must preprocess the audio before creating the effect, it may take a few extra moments to render the effect on the timeline whenever it moves or changes.

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
             Hint: To get the meter to properly fit the element group, you should Start with the **Zoom** at max and then adjust the **Gain** starting at the low end working upward so that the loudest parts of the music have minimial visible effect. 
             Then adjust the **Zoom** downward so that the softer parts of the music make the element light up most of the time.
   


---

### Response Speed

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

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---



