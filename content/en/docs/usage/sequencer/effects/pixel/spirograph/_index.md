---
title: Spirograph
author: Vixen Team
description: Creates an effect simulating the geometric patterns created by a children''s spirograph geometric drawing toy. 
aliases: [/vixen-3-documentation/sequencer/effects/spirograph/]
---

---

## Overview

Creates an effect simulating the geometric patterns created by a children''s spirograph geometric drawing toy. 
This effect creates moving flower type effects. When setting the controls for this effect, it is helpful to understand the actual toy it is based upon: 
<https://en.wikipedia.org/wiki/Spirograph>

---

### String Setup

* **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Speed** - Controls how quickly the spirograph pattern rotates and advances over the effect duration.
Inner Circle Radius: Sets the inner circle radius used to draw the spirograph shape. Smaller values create tighter, more intricate loops.

* **Outer Circle Radius** - Sets the outer circle radius used to draw the spirograph shape. Larger values expand the pattern outward across the display.

* **InnerCircle Radius** - Sets the inner circle radius used to draw the spirograph shape. Smaller values create tighter, more intricate loops.

* **Spirographs** - Controls how much of the spirograph path is drawn. Higher values create longer, denser patterns of the roulette curves.

* **Distance** - Sets how far the drawing point is from the center of the inner circle, changing the size and shape of the loops.

* **Color Range** - Controls how colors are spread from the center of the pattern outward. Higher values stretch the color bands over a larger area.

* **Animate Distance** - When enabled, the drawing distance changes as the effect plays, making the spirograph shape morph over time. Creates a sense of growth in the pattern.

---

### Color

* **Color Type** -  Chooses how colors are applied.
  * _Standard_ - Standard uses the selected colors by distance from center.  
  * _Rainbow_ - Rainbow generates random rainbow colors.  
  * _Random_ - Random picks randomly from the selected colors.
* **Gradients** - One or more colors used to shade the effect.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/spirograph/Spirograph.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
