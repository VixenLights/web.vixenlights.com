---
title: Advanced Mode
description: Creates an effect that outlines a display element with a border with advanced configuration controls.

---

### Overview

Creates an effect that outlines a display element with a border with advanced configuration controls.

---

### String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Border Mode** - Selects between _Simple_, _Advanced_, or _Marquee_ borders.

* **Border Type** - Selects between _Single_ or _Independent_ border width control.  
                    _Single_ border type makes all the sides of the display element a uniform thickness.

---

### Border

* **Thickness** - Adjusts the thickness of the border.  Applies when _Single_ **Border Type** is selected.

* **Top Width** - Adjusts the top border thickness. Applies when _Border Type_ is set to _Independent_.

* **Bottom Width** - Adjusts the bottom border thickness. Applies when _Border Type_ is set to _Independent_.

* **Left Width** - Adjusts the left border thickness. Applies when _Border Type_ is set to _Independent_.

* **Right Width** - Adjusts the right border thickness. Applies when _Border Type_ is set to _Independent_.

* **Width** - Configures the width of the border. 

* **Height** - Configures the height of the border.

---

### Movement

* **X Offset** - Adjusts the position of the effect along the X axis.

* **Y Offset** - Adjusts the position of the effect along the Y axis.

---

### Color

* **Gradient Mode** - Configures how the **Color Gradient** is applied to the border
                      (_Over Time_, _Across Element_, _Vertically Across Element_, _Diagonal Bottom-Top Element_, _Diagonal Top-Bottom Element_).

* **Color Gradient** - Controls the colors of the border.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

