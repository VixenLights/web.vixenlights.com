---
title: Pinwheel
author: Vixen Team
description: Creates an effect that makes a spiral that resembles a Pinwheel.
aliases: [/vixen-3-documentation/sequencer/effects/pinwheel/]
---

---

## Overview

Creates an effect that makes a spiral that resembles a Pinwheel.
You can control the number of arms that it has and the colors they will be.
There are numerous options that control how the arms behave.
This effect can be layered with other effects to produce complex effect combinations.

---

### String Setup

* **Positioning** - Determines how the target elements are treated. Either as individual strings or by their actual location in the display preview.
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

* **Offset Percentage** - Determines how the **X Offset** and **Y Offset** values below are interpreted. When enabled (the default), the offsets are a percentage of the target's width/height. When disabled, the offsets are an absolute pixel amount instead.

* **X Offset** - Shifts the center of the wheel along the X-axis.

* **Y Offset** - Shifts the center of the wheel along the Y-axis.

* **Center Hub** - Determines how big the hub or hole in the center of the wheel is.

* **Rotation** - Rotation speed and direction over the duration of the effect. 50 means no rotation, values above 50 rotate forward faster as they approach 100, and values below 50 rotate backward faster as they approach 0.

* **Blade Type** - Determines how the blade looks (*Flat*, *3D*, *Inverted 3D*, *Fan*).
  There are 4 choices from a flat look to 3D looks and a fan blade look.

---

### Color

* **Color Type** - Determines how arm colors are generated from the **Colors** list below.
* _Gradient over time_ - Each arm is given one color from the list (cycling through the list if there are more arms than colors), which shifts along that color's gradient as the effect plays.
* _Gradient Across Arms_ - Each arm's color instead varies along its length, from hub to tip, following the gradient.
* _Random_ - Each arm is assigned a random solid color when the effect starts and keeps that color for the duration. The **Colors** list is hidden and not used.
* _Rainbow_ - Each arm is assigned a new random color on every frame, producing a flickering rainbow look. The **Colors** list is hidden and not used.

* **Colors** - Can be simple colors or gradients. Each color or gradient has a level to adjust its brightness over the duration of the effect. You can have one to many colors; if there are more arms than colors, colors are reused round-robin across the arms. Hidden when **Color Type** is set to _Random_ or _Rainbow_.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
  This is a legacy parameter, consider using intensity overlay layers instead.

---

#### Video

{{< video src="Pinwheel.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
