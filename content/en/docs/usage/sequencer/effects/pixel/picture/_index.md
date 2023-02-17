---
title: Picture
author: Vixen Team
description: Creates an effect that imports a picture file to be displayed on a grid type prop.
aliases: [/vixen-3-documentation/sequencer/effects/picture/]
---

---

### Overview

Creates an effect that imports a picture file to be displayed on a grid type prop. May also be used to apply a texture to an element of any configuration.

A great place to download seamless tiles is: <http://www.patterncooler.com/>. They have a great system setup that allows you to customize the background to get almost anything you could want.

---

### String Setup
  
  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Movement

* **Type** - Controls tye type of movement (_None_, _Tiles_, _Left_, _Right_, _Up_, _Down_, _Up & Left_, _Down & Left_, _Up & Right_, _Down & Right_, _Peekaboo 0_, _Peekaboo 90_, _Peekaboo 180_,
             _Peekaboo 270_, _Wiggle).

* **Center Stop** - When selected, causes the image to stop at the center of the grid and then disappear.  This setting is only applicable to Movement types _Up_, _Down_, _Left_ and _Right_.

* **Iterations** - The number of times the pattern repeats over the duration of the effect.

* **X Offset** - Shifts the image horizontally.  This setting and the Y Offset can be used to animate the image with a  user defined motion path.

* **Y Offset** - Shifts the image vertically.  This setting and the X Offset can be used to animate the image with a user defined motion path.

---

### Configuration

* **Picture Source** - Selects between an embedded built-in image or selecting a file.

* **Embedded Pictures** - Select from a collection of included pattern images.  
*note, you may choose a eithe rcustom file, or embedded image, but not both.

* **Stretch to Grid** - Adjusts image diminesions to fit the grid size.

* **Scale to Grid** - Enable to scale the image to fit your grid.

---

### Effect Color

* **Color Effect** - Selects the type of color/gradient applied to the picture (_None_, _Custom Color_, _Gray Scale_).

* **Color Gradient** - Selects the color of the effect.  Applicable when the Color Effect selection is _Custom Color_.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

* **Increase Brightness** - Increases the brightness of the image.

---

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/picture/Picture.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
