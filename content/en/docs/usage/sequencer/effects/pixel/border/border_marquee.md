---
title: Marquee Mode
description: Creates an effect that outlines a display element with a marquee border.
---

---

### Overview

Creates an effect that outlines a display element with a marquee border.

---

### String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Border Mode** - Selects between _Simple_, _Advanced_, or _Marquee_ borders.  Refer to the links below for more information on each of the Border Modes.

* **Render Level** - Controls how the marquee is rendered (_Level 0_, _Level 1_, or _Level 2_).  
    * _Level 0_ - (default) renders the effect as a normal matrix outlining it with a border.
    * _Level 1_ - Converts the matrix into a single strand of pixels.  The single strand is created by looping back and forth.
    * _Level 2_ - Converts the maxrix into a single stand of pixels.  The single strand is created by always starting on the left side of the matrix.

    Render Levels 1 and 2 provide visually interesting patterns when this effect is placed on a mega-tree and other props.

* **Use Percentage** - Controls whether the _Band Length_, _Skip Length_, _Thickness_ and _Stagger_ settings are measured in pixels or are a percentage of the display element size.

* **Thickness** - Controls the width of the marquee border.

* **Stagger** - Controls the offset between each band of pixels in the marquee border.  The _Thickness_ needs to greater than 1 pixel for this control to be visible.

* **Band Length** - Controls the size of the marquee color bands.

* **Skip Length** - Controls the size of the blank area between marquee color bands.

* **Reverse** - Toggles the direction of the marquee movement.

* **X-Size** - Determines the size of the marquee along the x-axis.

* **Y-Size** - Determines the size of the marquee along the y-axis.

---

### Movement

* **X Offset** - Adjusts the position of the effect along the X axis.

* **Y Offset** - Adjusts the position of the effect along the Y axis.

* ** Wrap X Axis ** - Allows the marquee to wrap around the display element on the x-axis.

* ** Wrap Y Axis ** - Allows the marquee to wrap around the display element on the y-axis.

---

### Color

* **Color Gradient** - Controls the color of the bands that make up the marquee.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

