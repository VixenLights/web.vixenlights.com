---
title: Curtain
description: Creates an effect that imitates a curtain opening or closing across your display element.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/curtain/]
---

---

## Overview

Creates an effect that imitates a curtain opening or closing across your display element.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

* **Direction** - Selects the direction of the movement (_Open_, _Close_, _Open-Close_, _Close-Open_).

* **Motion** - Controls how the effect progresses across time between _Position_ or _Iterations.

* **Iterations** - The number of times the pattern repeats over the duration of the effect.

* **Edge** - Selects the position where the curtain opens from (_Left_, _Center_, _Right_, _Bottom_, _Middle_, _Top_).

* **Swag** - Controls the amount of swag on the moving curtain edge. (simulating the inertial curving movement of drapery in motion).


---

## Color

* **Color Gradient** - The color of the curtain.

---

## Brightness

* **Intensity** - This is an overall brightness intensity curve for over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

* **Intensity Per Iteration** - Adjust the intensity over each iteration.

---

## Video 

{{< video src="/images/docs/usage/sequencer/effects/pixel/curtain/Curtain.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}

---