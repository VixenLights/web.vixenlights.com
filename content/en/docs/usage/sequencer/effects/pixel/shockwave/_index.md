---
title: Shockwave
author: Vixen Team
description: Creates an effect that simulates the shockwave from an explosion, or the ripples of an object thrown into water.             
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/shockwave/]
---

---

### Overview

Creates an effect that simulates the shockwave from an explosion, or the ripples of an object thrown into water.             

---

### String Setup
  
  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Center X:** - Sets the horizontal position where the pattern is centered from. This control has a range of 0-100 where 50 is the horizontal center.

* **Center Y** - Sets the vertical position where the pattern is centered from. This control has a range of 0-100 where 50 is the vertical center.

* **Radius** - Controls the radius of the shockwave over the duration of the effect.

* **Scaled Radius** - Scales the shockwave to the size of the element.

* **Width** - Controls the width of the shockwave over the duration of the effect.

* **Acceleration** - The increase in movement speed over the duration of the effect.

---

### Color

* **Color Gradient** - The color or gradient used to color the effect. If a gradient is used, it is applied to the whole effect over the duration of the effect.

* **Blend Edges** - When checked, adds smoothing to the leading and trailing edge of the ripple. When unchecked the ripple will have a hard edge.

---

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/shockwave/Shockwave.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
