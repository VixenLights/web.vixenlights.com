---
title: Basics
author: Geoff Armstrong
date: 2018-02-01T10:03:42+00:00

---

## Overview

Creates an effect that draws a basket weave pattern and animates it.  This effect works the best on a matrix with a large pixel count.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

  * **Direction** -  Configures the direction of bar movement.
    * Up – The bars move in a upward direction.
    * Down – The bars move in a downward direction.
    * Left – The bars move from right to left.
    * Right – The bars move from left to right.
    * Compress – The bars move in a motion that looks like they are compressing in the middle.
    * Expands – The bars move outward from the center.
    * Horizontal Compress / Expand – This is the same as Compress / Expand only in the opposite plane.

  * **Rotation** - The rotation of the weave bars.  The weave bars can rotate in either direction using the following mapping to the curve:

    * 100 – 180 Degrees (Counter Clockwise)
    * 75 – 90 Degrees (Counter Clockwise)
    * 50 – No Rotation
    * 25 – 90 Degrees (Clockwise)
    * 0 – 180 Degrees (Clockwise)


  * **Speed** - Determines how fast the weave moves.

  * **Highlight** -  Creates a white highlighted leading edge on each bar. This may not be highly visible in some cases when using location positioning.

  * **3D** - Makes each color appear as a gradient fading to black.

  * **Weave Thickness** - Controls the thickness of the weave bar.  This value is a percentage of the display element.

  * **Weave Spacing** - Controls the blank area between each weave bar. This value is percentage of the display element. 

---

### Color

  * **Horizontal Colors** - The color gradients for the horizontal bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

  * **Vertical Colors** - The color gradients for the vertical bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

---

### Brightness

  * **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 