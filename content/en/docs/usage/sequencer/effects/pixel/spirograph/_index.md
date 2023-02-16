---
title: Spirograph
author: Vixen Team
description: Creates an effect simulating the geometric patterns created by a children''s spirograph geometric drawing toy. 
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/spirograph/]
---

---

### Overview


Creates an effect simulating the geometric patterns created by a children''s spirograph geometric drawing toy. 
This effect creates moving flower type effects. When setting the controls for this effect, it is helpful to understand the actual toy it is based upon: 
<https://en.wikipedia.org/wiki/Spirograph>

---

### String Setup
    
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Speed** - The speed at which the pattern is drawn.

* **Outer Circle Radius** - The radius of the inner circle.

* **InnerCircle Radius** - The radius of the outer circle.

* **Spirographs** - The number of circles (roulette curves) that make up the spirograph.

* **Distance** - A fixed distance between the circles

* **Color Range** - When color type is set to _Standard_, this defines what part of the range of colors is used.

* **Animate Distance** - Uses a variable distance instead of a fixed distance. Creates a sense of growth in the pattern.


---

### Color

* **Color Type** -  Controls how color is applied to the effect.
    * _Standard_ - Uses the defined colors/gradients in order from center outward.  
    * _Rainbow_ - Draws in completely random colors.  
    * _Random_ - Uses only the defined colors randomly.

* **Gradients** - One or more colors used to shade the effect.
   
---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/spirograph/Spirograph.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
