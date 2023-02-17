---
title: Spiral
author: Vixen Team
description: Creates a spiraled effect when applied to a mega-tree.
aliases: [/vixen-3-documentation/sequencer/effects/spiral/]
---

---

### Overview


This effect is best used on a megatree. When used on a megatree, it appears as a spiraled effect around the tree. 
When used on a flat matrix, it appears similar to the bars effect but with diagonal bars and space between the bars.

---

### String Setup
    
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Direction** - The direction of movement of the bands in the spiral pattern. Forward, Reverse or None.

* **Motion** - Controls how the effect progresses across time between _Speed_ and _Iterations_.

* **Iterations** - The number of times the pattern repeats over the duration of the effect.

* **Speed** - Determines how fast the swirls move.

* **Repeat** - The number of times the color pattern repeats per iteration.

* **Thickness** - The thickness of each band. This value is a percentage range of 0-100%

* **Rotation** - The angle of rotation of the bands. 0 is in the center and is vertical. The outer limits are -50 and 50 and represent a tilt of 50 degrees to the left or right.

* **3D** - Applies a horizontal fade to each band.

* **Grow** - Causes each band to start at the thickness specified above and grow to the maximum width.

* **Shrink** causes each band to start at the maximum thickness and shrink to the thickness defined above.

Grow and shrink can be combined and used together. When used this way, it will first start at the specified thickness and 
grow to the maximum followed by shrinking from the maximum to the specified thickness.


---

### Color

* **Gradients** - One or more gradients used to color the spiral bands.

* **Vertical Blend** - When selected, gradients are applied vertically to the bands. When not selected, gradients are applied horizontally.

   
---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/spiral/Spiral.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
