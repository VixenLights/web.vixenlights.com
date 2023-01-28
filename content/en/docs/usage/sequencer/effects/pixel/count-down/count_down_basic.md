---
title: Basics
author: Vixen Team
date: 2023-01-26T10:03:42+00:00

---

## Overview

Creates an effect that displays a count down on a display element.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

* **Count Type** - Controls how the effect counts (_To end of effect_, _Down from time_, _Up from time_).

* **Time Format** - Controls the units of the count down (_Minutes_ or _Seconds_). 

* **Fade** - Controls how the count down numbers appear (_None_, _In_, _Out_, _In/Out_)

* **Size Mode** - Controls whether the text shrinks or grows as the numbers are displayed (_None_, _Shrink_, _Grow_).

* **Start Time** - Field is only available when the **Count Type** is set to **Down from time** or **Up from time**. This initializes where the effect will count from.

* **Font** - Specifies the font, style and size to be used. You may use any font installed on the PC. Note that the fonts used must be installed on any PC where you will transfer this sequence. 

* **Film Spinner** - Adds a film spinner around the number. This feature works best on a medium to high resolution matrix.

---

## Movement

* **Direction** - Controls the direction of the effect (_Left_, _Right_, _Up_, _Down_, _Rotate_, _None_, _Random_).

* **Angle** - When enabled, controls the angle of the count down over the duration of the effect. This field is only available when the **Direction** is set to **Rotate.**

* **Horizontal Offset** - This is used to offset the center of the count down horizontally on the grid. Since this is a curve it can be used to move the center over the duration of the effect.

* **Vertical Offset** - The vertical offset. This is used to offset the center of the count down vertically on the grid. Since this is a curve it can be used to move the center over the duration of the effect.

* **Center Stop** - When enabled, causes the count down number to stop at the center of the grid. This field is only available when the **Direction** is set to **Left, Right, Up,** or **Down**.

* **Movement per number** - When enabled, the count down number moves as specified by the **Direction** over the grid for each number. This field is only available when the **Direction** is set to **Left, Right, Up,** or **Down**. 

* **Iterations** - When enabled, controls how fast the count down moves.  
This field is only available when the **Direction** is set to **Left, Right, Up,** or **Down**. This field is not applicable when **Movement per number** is selected. 


---

### Color

* **Text Color Gradients** - One or more gradients used to color the count down number and when enabled the film spinner. 

* **Gradient Mode** - Specifies how gradients will be applied to the text. There are 8 combinations of direction and how it’s applied. The gradient can be applied across the letters of the text, or across the whole element group. If it’s across the letters, the gradient will stay with the text. If it is across the element, it will appear that the text travels through the colors of the gradient. 

* **Film Spinner Gradients** - One or more gradients used to color the film spinner background swipe. 

* **Film Spinner Gradient Mode** - Specifies how gradients will be applied to the film spinner background swipe (_Across Text_, _Vertical Across Text_, _Vertical Across Element_, _Diagonal Across Text_, _Diagonal Across Element_, _Reverse Diagonal Across Element_, _Reverse Diagonal Across Text_) 


---

### Brightness

* **Intensity** - This is an overall brightness intensity curve for the count down over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

                  
---

#### Video Tutorial

{{< youtube RR2egpih9Fw>}}

