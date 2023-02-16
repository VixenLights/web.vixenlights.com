---
title: Garlands
description: Creates an effect that simulates filling the grid by wrapping it with garland.  This effect is best suited on megatree type props.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/garlands/]
---

---

## Overview

Creates an effect that simulates filling the grid by wrapping it with garland.  This effect is best suited on megatree type props.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

* **Motion** - Controls how the effect progresses across time between _Iterations_ or _Speed_.

* **Movement Type** - Selects whether the movement is based on iterations or speed.

* **Direction** - Sets the direction of the movement (_Up_, _Down_, _Left_, _Right_).

* **Iterations** - The number of times the pattern repeats over the duration of the effect.  This is only available when movement type is set to **Iterations**.

* **Speed** - The amount of time for one iteration of the effect.  If the speed is set to a point where one iteration is less than the duration of the effect, it will repeat with one or more additional iterations.  This parameter is only available when movement type is set to **Speed**.

* **Garland Type** - Selects between different styles of garland.

* **Spacing** - Adjusts the distance between the strings of garland.

---

## Color

* **Gradients** - Specify one or more colors/gradients to be applied across the prop.  
               The colors are applied starting with the last color in the list filling 
               the side where the direction is set and follows through to the first color in the list on the other side of the prop

---

## Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.
                 
---

## Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/garlands/Garlands.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}


---