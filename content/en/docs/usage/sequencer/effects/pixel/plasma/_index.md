---
title: Plasma
author: Vixen Team
description: Creates an effect that resembles plasma.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/plasma/]
---

---

### Overview

Creates an effect that resembles plasma.  The style and motion of the plasma can be configured by the effect settings.

---

### String Setup
  
  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Speed** - Controls the speed of the motion.

* **Line Density** - Controls the density of the pattern. The higher the setting, the smaller and tighter the plasma patterns appear.

* **Plasma Style** - Selects between different variations of the plasma pattern.

---

### Color

* **Color Type** - Selects between different methods to apply colors to the effect.  
    * _Custom_ - Uses one or more gradients to set the colors.  
    * _Red & Green_
    * _Green & Blue_
    * _Rainbow_
    * _Black & White_

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

* **Gradients** - Configure one or more colors or gradients to use when the color type is set to _Custom_.
---

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/plasma/Plasma.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
