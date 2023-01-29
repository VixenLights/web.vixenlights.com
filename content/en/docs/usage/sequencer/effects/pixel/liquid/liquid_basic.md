---
title: Basics
author: Vixen Team
date: 2023-01-16T10:03:42+00:00

---

## Overview

Creates an effect that leverages the Google Liquid Fun library to simulate fluid movement.
This effect can produce unique liquid patterns if the settings are finely tuned.  
This effect works the best on a matrix with a large pixel count.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

* **Render Scale Factor** -  Determines the factor used to scale the Liquid matrix  to the sparse matrix formed by the selected elements.  The scale factor can improve how the effect renders in a sparse location based matrix since the liquid particles are larger.

* **Top Barrier** - Creates a barrier at the top of the display area.  This barrier prevents the liquid particles from leaving the top of the display area.

* **Bottom Barrier** - Creates a barrier at the bottom of the display area.  This barrier prevents the liquid particles from falling out of the element.

* **Left Barrier** - Creates a barrier at the left side of the display area.  This barrier prevents the liquid particles from leaving the left side of the display area.

* **Right Barrier** -  Creates a barrier on the right side of the display area.  This barrier prevents the liquid particles from leaving the right side of the element.

* **Mix Colors** -  When selected liquid particles of different colors will combine colors when the particles collide or come into contact with each other.

* **Particle Size** - Defines the radius of all particles in the effect.

* **Warm Up Frames** - Runs the Liquid engine for the specified number of frames before rendering the effect.  This setting is useful if you want a large number of particles in the display area at the beginning of the effect.

* **Despeckle Threshold** - This setting helps fill in empty (speck) pixels in the effect by filling them in with the average color of the surrounding pixels if the number of surrounding empty (black) pixels is less than the threshold.

---

## Emitters

* **Emitters** - This list defines the emitters in the effect.  Emitters can be added or removed via buttons at the bottom of the list.

* **Particle Type** - Determines the type of particle created by the emitter.  The differences between the types is very subtle.  **Powder** is the one type that produces a different behavior that is visually discernible.

* **Use Color List** - When selected this option controls the color of the particles created by the emitter.  The particles will cycle through the colors in the list for configurable number of frames.

* **Frames Per Color** - Determines how many frames of particles are created for each color in the list.

* **Particle Color** - Determines the color of the emitter&#8217;s liquid particles

* **Particle Intensity** - Determines the brightness of the emitter&#8217;s liquid particles.

* **Particle Lifetime** - Determines how long the emitter&#8217;s particles exist.

* **Particle Velocity** - Determines the speed of the particles emitting from the emitter.

* **Animate** - This option animates the position of the emitter within the element.

* **Random Start** - Controls whether the animated emitter&#8217;s start position is random.  When selected the initial start position of the emitter is randomized to a position on the display element.

* **X Start Position** - Controls the X starting position of the emitter.  Zero is the far left of the display element.  100 is the far right of the display element.

* **Y Start Position** - Controls the Y starting position of the emitter.  Zero is the bottom of the display element.  100 is the top of the display element.

* **Edge Handling** - This option controls how the emitters behave when they reach the edge of the display area.  **Bounce** setting causes the emitter to bounce off the edge of the display area.  **Wrap** setting causes the emitter to wrap around from the other side of the display area.

* **Velocity X** - Controls the speed of the emitter in the X axis when animated.

* **Velocity Y** - Controls the speed of the emitter in the Y axis when animated.

* **X Position** - Controls the position of the emitter on the display area in the X axis.

* **Y Position** - Controls the position of the emitter on the display area in the Y axis.

* **Nozzle Size** - Controls the size of the area the particles are released from the emitter.  The smaller the nozzle the more the particles go in different directions.   The larger the nozzle the more the particles go in a straight line.

* **Nozzle Movement** - Controls how the position of the emitter&#8217;s nozzle is determined.

  * _Fixed Angle_ - Angle determine by a curve
  * _Oscillate_ - Oscillates back and forth between two angular stops.
  * _Spin Clockwise_ - Spins clockwise for the duration of the effect
  * _Spin Counter Clockwise_ - Spins clockwise for the duration of the effect

* **Nozzle Angle** - Controls the angle of the emitter&#8217;s nozzle.
  * 0 - Points Right (0 Degrees)
  * 25 - Points Up (90 Degrees)
  * 50 - Points Left (180 Degrees)
  * 75 - Points Down (270 Degrees)
  * 100 - Points Right (360 Degrees)

* **Oscillate Start Angle** - Defines the starting angle of the oscillation.

* **Oscillate End Angle** - Defines the end angle of the oscillation. This is the point where the nozzle will reverse the direction of rotation.

* **Nozzle Speed** - Determines the emitter&#8217;s nozzle rotation speed.

* **Flow Control** - This drop down determines the continuity of the liquid flow.
  * _Continuous_ - Solid flow of liquid.
  * _Pulsating_ - Solid flow for a number of seconds followed by a period where the emitter if off for a number of seconds.
  * _Use Marks_ - Uses a mark collection to determine when the emitter is On.  The emitter will be Off when not covered by a mark.
  * _Musical_ - Uses the volume of the music associated with the sequence to determine the flow rate.  As the volume in the music gets louder the flow of the emitter increases.

* **Flow** - Controls the rate of particles emitted by the emitter.

* **Mark Collection** - Selects the Mark Collection to use to determine when the emitter is emitting (On).

* **On Time (ms)** - Controls the number of milliseconds the emitter is emitting in 50 ms increments.

* **Off Time (ms)** - Controls the number of milliseconds the emitter is off in 50ms increments.

---

