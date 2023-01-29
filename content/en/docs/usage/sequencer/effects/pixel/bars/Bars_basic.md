---
title: Basics
author: Vixen Team
date: 2023-01-16T10:03:42+00:00

---

## Overview

Creates an effect that animates bars on a display element.  This effect works the best on a matrix with a large pixel count.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

## Configuration

* **Bar Type**  - Selects either a _Flat_ or an angled _Zig Zag_ styled bar.

* **Direction** - Sets the direction of bar movement.

  * _Moves Up_ - The bars move in a upward direction.
  * _Moves Down_ - The bars move in a downward direction.
  * _Compress_ - The bars move in a motion that looks like they are compressing in the middle.
  * _Expands_ - The bars move outward from the center.
  * _Moves Left_ - The bars move from right to left.
  * _Moves Right_ - The bars move from left to right.
  * _Horizontal Compress_ - The bars move in a motion that looks like they are compressing in the middle.
  * _Horizontal Expand_ - The bars move outward from the display element center.
  * _Alternate Up_ - The bars move up in an alternating fashion.
  * _Alternate Down_ - The bars move down in an alternating fashion. 
  * _Alternate Left_ - The bars move left in an alternating fashion.
  * _Alternate Right_  - The bars move right in an alternating fashion.
  
* **Rotation:** The rotation of the bars.  The bars can rotate in either direction using the following mapping to the curve:          
    
* 100 – 180 Degrees (Counter Clockwise)
* 75 – 90 Degrees (Counter Clockwise)
* 50 – No Rotation
* 25 – 90 Degrees (Clockwise)
* 0 – 180 Degrees (Clockwise)

* **Motion** - Determines the how the motion of the bars is controlled by selecting either _Iterations_ or _Speed_.

* **Iterations** The number of times the pattern repeats over the duration of the effect.

* **Speed** - Determines how fast the bars moves.

* **Repeat** - Determines how times the color bars are repeated on the display element.  This indirectly determines the thickness of the bars.

* **Highlight:** Creates a white highlighted leading edge on each bar. This may not be highly visible in some cases using locations.

* **Highlight %:** Controls the percentage of the bar that is highlighted white.  Setting only available in _Location_ mode.

* **3D:** Makes each color appear as a gradient fading to black. This is a legacy function, consider using gradients instead.


---

### Color

* **Gradients:** This is where you set the colors of the bars.  The number and order of the colors here will be how they are applied in the effect.  The list supports gradients of solid, or varying colors.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 

---

#### Zig Zag Configuration

* **Amplitude:** Controls the height of the zig zag&#8217;s crest.

* **Period:** Controls the width or wave length of the zig zag.

* **Thickness:** Controls the thickness of the zig zag.

* **Spacing:** Controls the blank area between each zig zag color.

---

#### Video Tutorial

{{< youtube puavBNDAIbw>}}
