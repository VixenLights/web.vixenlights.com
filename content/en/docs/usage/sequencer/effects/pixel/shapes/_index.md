---
title: Shapes
description: Creates an effect that animates shapes on the display element.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/shapes/]
---

---

### Overview

Creates an effect that animates shapes on the display element.

---

### String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Shape Source** - Selects option for determining how shapes are added or removed.  Options include _None_, _Create Shapes from Mark Collection_, _Remove shapes from Mark Collection_.

* **Mark Collection** - Selects the mark collection for determining when to add or remove shapes as determined by the **Shape Source** setting.

* **Type** - Selects the type of shape to display.  There are built-in shapes organized by the following categories _Geometric_, _Christmas_, _Halloween_.  There is also a _File_ option to
             import a shape from an svg file.

* **File** - Display a file selection dialog to select an svg file to use for the shape.  This setting is only available when _File_ **Type** is selected.

* **Geometric Shapes** - Selects one of the built-in geometric shapes to animate.

* **Christmas Shapes** - Selects one of the built-in Christmas themed shapes to animate.

* **Halloween Shapes** - Selects one of the built-in Halloween themed shapes to animate.

* **Movement** - Configures how shapes behave when reaching the edge of the display element between _None_, _Bounce_ or _Wrap_.

* **Fade Type** - Selects the type of shape fade type from _None_, _In_, _Out_ or _Random_.

* **Size Mode** - Selects how the shape changes size between _Shrink_, _Grow_, and _Random_.

* **Size** - Determines the size of the shapes.

* **Size Variation** - Randomly adjusts the shape size around the **Size** level by the amount of variation.

* **Count** - Controls the number of shapes to be displayed.

* **Size Change** - Enable increase/decrease of shape size based on size variation.

* **Scale To Grid** - Sizes the shape to fill the display element.  Shape motion is disabled with this option.

* **Random Angle** - Randomly configures the rotation of the shape.

* **Random Size** - Randomly adjusts the shape size.

* **Fill Color** - Fills the shape with the **Fill Color**.


---

### Shape Settings

* **Outline Dash Length** -  Controls the outline dash length of the shape, used with the **Outline Space Length** to draw the shape.

* **Outline Space Length** - Controls the outline space length of the shape, used with the **Outline Dash Length** setting to draw the shape.

* **Outline Thickness** - Controls the thickness of the shape outline.

* **Rounded Corners** - Add rounded corners to the Geometric shapes.


---

### Speed Settings

* **Speed** - Controls the speed of the shape moving on the display element.

* **Speed Variation** - Randomly adjusts the speed around the **Speed** level by the amount of the variation.

* **Size Speed** - Controls how fast the shape grows or shrinks.

* **Size Speed Variation** - Randomly adjusts the size speed around the **Size Speed** level by the amount of the variation.

* **Angle Speed** - Controls the rotation speed of the shape.

* **Angle Speed Variation** - Randomly adjusts the rotation speed around the **Angle Speed** level by the amount of the variation.

---

### Color

* **Fill Colors 1** - Controls the fill color of the shapes.

* **Outline Colors** - Controls the outline color of the shapes.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

### Video Tutorial

{{< youtube Wsouti49lWs>}}

