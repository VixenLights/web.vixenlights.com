---
title: Pattern
description: Creates an effect that draw a pattern and animates it.
---

---

## Overview

Creates an effect that draws a pattern and animates it.  The pattern is either a basket weave or bricks.  This effect works the best on a matrix with a large pixel count.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

  * **Pattern Type** - Selects the pattern (_Weave_ or _Brick_) to animate.

  * **Direction** - Configures the direction of pattern movement.
    * _Moves Up_ - The pattern moves in a upward direction.
    * _Moves Down_ - The pattern moves in a downward direction.
    * _Vertical Expand_ - The pattern moves outward from the vertical center.
    * _Vertical Compress_ - The pattern moves in a motion that looks like they are compressing in the vertical middle.
    * _Moves Left_ - The pattern moves from right to left.
    * _Moves Right_ - The pattern moves from left to right.
    * _Horizontal Expand_ - The pattern moves outward from the horizontal center.
    * _Horizontal Compress_ - The pattern moves in a motion that looks like they are compressing in the horizontal middle.       
    * _Center Compress_ - The pattern moves in a motion that looks like they are compressing in the middle.    
    * _Center Expand_ - The pattern moves outward from the center.
    

  * **Rotation** - The rotation of the pattern.  The pattern can rotate in either direction using the following mapping to the curve:

    * 100 - 180 Degrees (Counter Clockwise)
    * 75 - 90 Degrees (Counter Clockwise)
    * 50 - No Rotation
    * 25 - 90 Degrees (Clockwise)
    * 0 - 180 Degrees (Clockwise)

  * **Speed** - Determines how fast the pattern moves.

  * **Highlight** -  Creates a white highlighted leading edge on each weave bar or brick. This may not be highly visible in some cases when using location positioning.

  * **Highlight %** - Controls the percentage of the bar / brick that is highlighted.  This control is only applicable when the effect is in _Locations_ mode.

  * **3D** - Makes each color appear as a gradient fading to black.
  
  

---

## Weave Configuration

  * **Thickness** - Controls the thickness of the weave bar.  This value is a percentage of the display element.  

  * **Spacing** - Controls the blank area between each weave bar. This value is percentage of the display element. 

  * **Advanced Sizing** - Enables curves for controling the weave bar thickness and spacing.  The horizontal and vertical weave bar thickness and spacing can be configured independently
                          when in advanced sizing mode.

  * **Horizontal Thickness** - Controls the thickness of the horizontal weave bars.  This value is a percentage of the display element.

  * **Horizontal Spacing** - Controls the blank area between each horizontal weave bar. This value is percentage of the display element. 

  * **Vertical Thickness** - Controls the thickness of the vertical weave bars.  This value is a percentage of the display element.

  * **Vertical Spacing** - Controls the blank area between each vertical weave bar. This value is percentage of the display element. 

---

## Brick Configuration

* **Brick Height** - Controls the height of the bricks.

* **Brick Width** - Controls the width of the bricks.

* **Mortar Height** - Controls the height and width or mortar between bricks.

* **Rotate Brick** - Rotates the bricks by 90 degrees.

---

### Color (Weave)

  * **Horizontal Gradients** - The color gradients for the horizontal bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

  * **Vertical Gradients** - The color gradients for the vertical bars that make up the weave.  The list supports gradients of solid, or varying colors.  Gradients are applied over the width of the bar.

---

### Color (Brick)

* **Brick Colors** - Controls the color of the bricks.  The list supports gradients of solid, or varying colors.  Gradients are applied across the bricks.

* **Mortar Color** - Controls the color of the brick mortar.  Gradients is sampled and applied over the duration of the effect.

### Brightness

  * **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                    This is a legacy parameter, consider using intensity overlay layers instead.

---

#### Video Tutorial

{{< youtube pmC0ZrT3ceE>}}