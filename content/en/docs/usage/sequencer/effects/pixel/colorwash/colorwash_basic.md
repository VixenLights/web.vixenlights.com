---
title: Basics
author: Vixen Team
date: 2023-01-26T10:03:42+00:00

---

## Overview

Creates an effect that washes colors over the display element.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

* **Type**  - Selects between pattern variations.
    * _Center_ 
    * _Outer_ 
    * _Invert_ 

* **Motion** - Controls how the effect progresses across time between **Speed** and **Iterations**.
    * _Iterations_ - Displays the **Iterations** slider to specify the number of times the pattern repeats over the duration of the effect.
    * _Speed_ - Displays a **Speed** Curve for configuring the speed of the pattern over the duration of the effect.

* **Iterations** - The number of times the pattern repeats over the timespan of the effect.

* **Speed** - Controls the speed of the colors washing over the prop.
    
* **Horizontal Fade** - Adds a horizontal fade to the color wash pattern.

* **Vertical Fade** - Adds a vertical fade across the color wash pattern.

* **Shimmer** - Adds a flashing/strobing effect as the color fades.


---

### Color

* **Color Gradient** - Controls the color of the wash for the duration of the effect.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

#### Video 

{{< video src="/images/docs/usage/sequencer/effects/pixel/colorwash/Colorwash.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}

