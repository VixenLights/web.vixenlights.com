---
title: Pinwheel
author: Vixen Team
description: Creates an effect that makes a spiral that resembles a Pinwheel.             
aliases: [/vixen-3-documentation/sequencer/effects/pinwheel/]
---

---

### Overview

Creates an effect that makes a spiral that resembles a Pinwheel.
You can control the number of arms that it has and the colors they will be. 
There are numerous options that control how the arms behave. 
This effect can be layered with other effects to produce complex effect combinations.

---

### String Setup
  
  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Motion** - Controls how the effect progresses across time between **Speed** and **Iterations**.

* **Movement** - Controls variance of the motion over time.

* **Arms** - Controls how many arms the wheel has.

* **Thickness** - Determines how thick the arms are.

* **Size** - Determines how big around the wheel is.

* **Twist** - Determines how much the arms curve.

* **X Offset** - Shifts the center of the wheel along the X-axis.

* **Y Offset** - Shifts the center of the wheel along the Y-axis.

* **Center Hub** - Determines how big the hub or hole in the center of the wheel is.

* **Rotation** - Determines which direction the wheel spins (_Forward_, _Backward_).

* **Blade Type** - Determines how the blade looks (_Flat_, _3D_, _Inverted 3D_, _Fan_).
                   There are 4 choices from a flat look to 3D looks and a fan blade look.

---

### Color

* **Color Type** - Determines how the colors are applied to a blade. The gradient can traverse over time, over the length of the blade. There are options for random colors or a rainbow of colors.

* **Colors** - Can be simple colors or gradients. Each color or gradient has a level to adjust it's brightness over the duration of the effect. You can have one to many colors. 
The blades will rotate across the selected colors.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/pinwheel/Pinwheel.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
