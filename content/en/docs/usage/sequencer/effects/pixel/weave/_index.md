---
title: Weave
description: Creates an effect that draw a basket weave pattern and animates it.
---

---

## Overview

Creates an effect that draws a weave pattern and animates it.  This effect works the best on a matrix with a large pixel count.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

  * **Direction** - Configures the direction of bar movement.
    * _Moves Up_ - The bars move in a upward direction.
    * _Moves Down_ - The bars move in a downward direction.
    * _Vertical Expand_ - The bars move outward from the center.
    * _Vertical Compress_ - The bars move in a motion that looks like they are compressing in the middle.
    * _Moves Left_ - The bars move from right to left.
    * _Moves Right_ - The bars move from left to right.
    * _Horizontal Expand_ - The bars move outward from the center.
    * _Horizontal Compress_ - The bars move in a motion that looks like they are compressing in the middle.       
    * _Center Compress_ - The bars move in a motion that looks like they are compressing in the middle.    
    * _Center Expand_ - The bars move outward from the center.
    

  * **Rotation** - The rotation of the weave bars.  The weave bars can rotate in either direction using the following mapping to the curve:

    * 100 - 180 Degrees (Counter Clockwise)
    * 75 - 90 Degrees (Counter Clockwise)
    * 50 - No Rotation
    * 25 - 90 Degrees (Clockwise)
    * 0 - 180 Degrees (Clockwise)

  * **Speed** - Determines how fast the weave moves.

  * **Highlight** -  Creates a white highlighted leading edge on each bar. This may not be highly visible in some cases when using location positioning.

  * **3D** - Makes each color appear as a gradient fading to black.
  
  * **Thickness** - Controls the thickness of the weave bar.  This value is a percentage of the display element.

  * **Spacing** - Controls the blank area between each weave bar. This value is percentage of the display element. 

  * **Advanced Sizing** - Enables curves for controling the weave bar thickness and spacing.  The horizontal and vertical weave bar thickness and spacing can be configured independently
                          when in advanced sizing mode.

  * **Horizontal Thickness** - Controls the thickness of the horizontal weave bars.  This value is a percentage of the display element.

  * **Horizontal Spacing** - Controls the blank area between each horizontal weave bar. This value is percentage of the display element. 

  * **Vertical Thickness** - Controls the thickness of the vertical weave bars.  This value is a percentage of the display element.

  * **Vertical Spacing** - Controls the blank area between each vertical weave bar. This value is percentage of the display element. 

---

### Color

  * **Horizontal Gradients** - The color gradients for the horizontal bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

  * **Vertical Gradients** - The color gradients for the vertical bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

---

### Brightness

  * **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                    This is a legacy parameter, consider using intensity overlay layers instead.