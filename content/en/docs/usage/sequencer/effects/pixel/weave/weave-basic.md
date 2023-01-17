---
title: Basics
author: Vixen Team
date: 2023-01-16T10:03:42+00:00

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
    * Moves Up – The bars move in a upward direction.
    * Moves Down – The bars move in a downward direction.
    * Vertical Expand – The bars move outward from the center.
    * Vertical Compress – The bars move in a motion that looks like they are compressing in the middle.
    * Moves Left – The bars move from right to left.
    * Moves Right – The bars move from left to right.
    * Horizontal Expand – The bars move outward from the center.
    * Horizontal Compress – The bars move in a motion that looks like they are compressing in the middle.       
    * Center Compress – The bars move in a motion that looks like they are compressing in the middle.    
    * Center Expand – The bars move outward from the center.
    

  * **Rotation** - The rotation of the weave bars.  The weave bars can rotate in either direction using the following mapping to the curve:

    * 100 – 180 Degrees (Counter Clockwise)
    * 75 – 90 Degrees (Counter Clockwise)
    * 50 – No Rotation
    * 25 – 90 Degrees (Clockwise)
    * 0 – 180 Degrees (Clockwise)

  * **Speed** - Determines how fast the weave moves.

  * **Highlight** -  Creates a white highlighted leading edge on each bar. This may not be highly visible in some cases when using location positioning.

  * **3D** - Makes each color appear as a gradient fading to black.

  * **Thickness** - Controls the thickness of the weave bar.  This value is a percentage of the display element.

  * **Spacing** - Controls the blank area between each weave bar. This value is percentage of the display element. 

---

### Color

  * **Horizontal Gradients** - The color gradients for the horizontal bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

  * **Vertical Gradients** - The color gradients for the vertical bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

---

### Brightness

  * **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 