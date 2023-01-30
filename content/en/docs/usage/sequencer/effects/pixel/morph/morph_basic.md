---
title: Basics
author: Vixen Team
date: 2023-01-16T10:03:42+00:00

---

### Overview

Create an effect morphs shapes (polygons/ellipses/lines) on the display element(s). 
This effect works the best on a matrix or mega-tree with a large pixel count.  
This effect can be used as a standalone effect but also can be used as a layering mask along with other effects.

---

### String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Polygon Configuration

* **Polygon Type** - Determines the mode of the morph effect.

  * [_Pattern_](../morph_pattern) - This mode was inspired by other sequencers.  This mode is restricted to using four point polygons, ellipses or lines.  This mode includes settings that allow the user to repeat a shape (polygon/ellipse/line) several times across the display element.  Repeating the shape establishes a repeating pattern.
_ 
  * [_Free Form_](../morph_freeform) - This mode allows the user to draw an unlimited number of shapes (polygons/ellipses/lines) on the display element.  There is no limit to the number of polygon points used.
_ 
  * [_Time Based_](../morph_time_based) - This mode allows the user to draw a shape (polyon/ellipse/line) and then morph it over the duration of the effect.  The only restriction on the number of polygon points is that all polygon frames must have the same number of points.  In this mode the user creates frames and positions them within the time scale of the effect.  The user is in control of how the shape moves or changes shape by creating the frame snapshots. 

  Both the _Free Form_ and _Time Based_ modes are candidates to be used with layering and other effects to create unique composite effects.

  Each mode of the morph effect has a dedicated help page:

  * [Pattern Mode](../morph_pattern)
  * [Free Form Mode](../morph_freeform)
  * [Time Based Mode](../morph_time_based)

* **Fill Type** - Determines how the shape (polygon/ellipse/line) is filled (_Wipe_, _Solid_, _Outline_).

* **Margin** - By default the polygon editor associated with the Morph effect only allows the user to draw on the display element.  
The Margin defaults to zero (percent).  
By increasing the Margin a larger virtual display element is created for the purposes of drawing shapes.   
When a margin is in use the actual display element is outlined in red.   When the effect is rendered only the portion of shapes that overlap the red outline will be displayed.   
The margin setting is especially useful for Time Based Mode.  It can be used to animate a shape that enter and exits the display element smoothly.
The margin is a percentage of the display element width and height (0 - 100%).

---

### Video Tutorial

{{< youtube phoCw_kFld4>}}

---

 
