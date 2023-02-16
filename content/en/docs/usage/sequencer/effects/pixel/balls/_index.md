---
title: Balls
description: Creates an effect that animates Ball looking shapes.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/balls/]
---

---

### Overview

Creates an effect that animates Ball looking shapes. 

---

### String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Type** - Configures how balls behave when reaching the edge of the display element between _Bounce_ or _Wrap_.

* **Fill** - Selects the type of fill for the balls between _Fade_, _Empty_, _Solid_, _Gradient_, and _Inverse_.

* **Speed** - Configures the speed of the moving balls.

* **Speed Variation** - Randomly adjusts the speed of the moving balls around the **Speed** level by the amount of variation.

* **Size** - Size of the balls.

* **Ball Count** - Controls the number of balls displayed.

* **Random Time** - Configures the maximum time used to detrmine when the ball direction changes.  This setting only applies when **Random Movement** is selected.

* **Random Movement** - Randomly changes the ball direction at random times.

* **Random Radius** - Creates random size balls up to the **Size** value.

* **Collide** - Change the ball direction when balls collide.

* **Collide Color** - Change the ball color when balls collide.

---

###  Color

* **Gradients** - Controls the colors of the balls.

---


### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/balls/Balls.m4v" height="150" width="150" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}

