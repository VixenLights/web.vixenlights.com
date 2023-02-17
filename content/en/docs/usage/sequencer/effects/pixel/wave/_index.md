---
title: Wave
author: Vixen Team
description: Creates an effect that produces waves on the display element.  
aliases: [/vixen-3-documentation/sequencer/effects/Wave/]
---

---

### Overview


Creates an effect that produces waves on the display element.  This effect works the best on a matrix with a large pixel count.


---

### String Setup
    
  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Waves** - This list defines the waves in the effect.
            Waves can be added or removed via the **Add** and **Remove** buttons at the bottom of the list.
            The waves are ordered by number and layered on top of each other.
            The last wave will draw on top of all the other waves.

* **Wave Type** - Determines the type of of waveform.

  * _Sine_ - Sinusoidal waveform.
  * _Triangle_ - Non-sinusoidal waveform named for its triangular shape.
  * _Square_ - Non-sinusoidal periodic waveform in which the amplitude alternates at a steady frequency between fixed minimum and maximum values, with the same duration at minimum and maximum.
  * _Decaying Sine_ - Sinusoidal waveform where the amplitude is decreasing over time.
  * _Fractal Ivey_ - Random growing ivey vine like growing pattern.
  * _Sawtooth_ - Non-sinusoidal waveform. It is named based on its resemblance to the teeth of a plain-toothed saw with a zero rake angle.


* **Use Marks** - Enables the Mark Collection Name drop down to select a mark collection to determine when the Decaying Sine will bounce back to the normal amplitude.

* **Mark Collection Name** - This optional setting determines when the Decaying Sine wave type rebounds back to the normal amplitude.  If this setting is left empty the Decaying Sine will bounce back to the normal amplitude once the amplitude reaches zero.

* **Movement Type** - Determines the movement of the waveform.

  * _Continuous_ - Continuous waveform that grows.
  * _Snake_ - Only portion of the waveform is shown which for sine wave type appears snake like.  Once the waveform reaches the edge of the display element it wraps around to the other side.
  * _Grow and Shrink_ - The waveform grows to the edge of the display and then shrinks back to the opposite edge of the display.

* **Snake Length** - Determines the length of the snake.  This setting is only applicable when the Movement Type is Snake.

* **Prime Wave** - By default the wave grows across the display element.  This setting primes the waveform such that it fills the entire display element at the start of the effect.


* **Direction** - Determines the direction of the waveform.  This setting allows for multiple waveforms to move in opposing directions.

  * _Left To Right_
  * _Right To Left_ 
  * _Top To Bottom_ 
  * _Bottom To Top_ 

* **Mirror** - Mirrors the waveform across an imaginary y-axis.

* **Frequency** - Determines how many times the waveform repeats on the display element.

* **Phase Shift** - Determines how far the waveform is shifted horizontally from the usual position.  The phase shift is adjustable from zero to 180 degrees.  This setting is useful to control the relative position of waveforms relative to each other.

* **Thickness** - Determines the vertical thickness of the waveform.

* **Amplitude** - Determines the height of the waveform.

* **Y Offset** - Moves the waveform up or down in the display element.

* **Speed** - Determines how fast the waveform moves.  The speed determines how many columns of the waveform are rendered each frame.   This setting is in columns (or pixels) where each 10 units in the curve editor equals 1 column.

* **Color** - Determines the color of the wave over the duration of the effect.

* **Color Handling** - Controls how the color gradient is applied to the wave.  Selecting _Along Wave_ colors each column of the wave by sampling the gradient for the duration of the effect.  Selecting _Across Wave_ uses the gradient to color each pixel that makes up the thickness of the wave.


---


