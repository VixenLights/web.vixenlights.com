---
title: Whirlpool
description: Creates an effect that draws a whirlpool.
---

---

## Overview

Creates an effect that draws a whirlpool.  This effect works the best on a matrix with a large pixel count.

---

## String Setup

  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
  * **Orientation** - Controls the orientation of the display area (matrix).
  * **Render Scale Factor** -  Determines the factor used to scale the Whirlpool matrix to the sparse matrix formed by the selected elements.  
                               A value of 1 will provide the highest quality whirlpool.
                               A larger scale factor can improve rendering speed with a potential tradeoff in image quality.  This setting is only applicable when
                               the **Positioning** is set to *Locations*.
---

## Grid Panels

  * **Columns** - Controls the number of columns of whirlpools on the display element.
  * **Rows** - Controls the number of rows of whirlpools on the display element.
  * **Panel Spacing** - Controls the spacing between the whirlpool panels on the display element as a percentage of the display element.
  * **Individual Configuration** - Enables each individual whirlpool to be configured separately by displaying each whirlpool in the **Whirls** collection.
  If the top level **Whirl Configuration** settings are modified, those changes are applied to all whirl panels.
---
    
## Whirl Configuration

  * **Whirl Mode** - Determines if the whirls are drawn as continous rings, concentric rings, or as a meteor travelling the whirlpool path.
    * _Continuous Whirls_ - Draw a continuous whirl.
    * _Concentric Whirls_ - Draws concentrics rings to form the whirlpool.
    * _Meteor_ - Draws a meteor following the whirlpool path.
    
  * **Tail Length** - Determines the length of the meteor as a percentage of the display element.  Only applies when the **Whirl Mode** is set to *Meteor*.

  * **Rotation** - Configure the direction of rotation (Clockwise vs Counter-Clockwise) that the whirls are drawn.
    * _Clockwise_ - Whirls are drawn moving clockwise.
    * _Counter-Clockwise_ - Whirls are drawn moving clockwise.

  * **Start Location** - Controls the corner of the matrix where the whirls start from.
    * _Top Left_ - Whirls start in the upper left corner.
    * _Bottom Left_ - Whirls start in the bottom left corner.
    * _Top Right_ - Whirls start in the top right corner.
    * _Bottom Right_ - Whirls start in the bottom right corner.

  * **Direction** -  Determines if the whirls are drawn moving *In*, moving *Out*, or *In and Out*.
    * _In_ - Draws the whirls moving in.
    * _Out_ - Draws the whirls moving out.
    * _In And Out_ - Draws the whirls moving in and then erases the whirls moving out.

  * **Reverse Draw** - Reverses the drawing of the whirl.  The whirl is drawn complete and then is erased.
  
  * **Spacing** - Controls the amount blank area between each whirl as a percentage of the display element.

  * **Thickness** - Controls the thickness of the whirl as a percentage of the display element.

  * **3D** - Adds 3D shading to the whirls.
---

## Whirls

The whirl collection is only visible when **Individual Configuration** setting is selected.  With the exception of **Enabled** all the settings
of the whirls are documented in the section above. 

* **Enabled** - Determines whether a particular whirl is visible.  This settings helps determine which whirl is being modified.

Note if any of the top level **Whirl Configuration** settings are changed those settings will override any previous individual configuration of those specific settings.

---

### Configuration

* **Iterations** - Determines how many times the whirls are drawn during the effect duration.

* **Pause At End** - Determines the percentage of the effect's duration that the completed whirls will be displayed.

---

### Movement

* **X-Scale** - Determines the size of the effect's drawing area along the x-axis.

* **Y-Scale** - Determines the size of the effect's drawing area along the y-axis.

* **Vertical Offset** - Controls the position of the effect's drawing area on the display element in the y-axis.

* **Horizontal Offset** - Controls the position of the effect's drawing area on the display element in the x-axis.

---

### Color

* **Color Mode** - Controls how color is applied to the whirlpool.
    * _Single Color_ - Applies a single color gradient to the whirlpool over the duration of the effect.
    * _Side Colors_ - Applies a unique color gradient to each side over the duration of the effect of the whirlpool.
    * _Color Rings_ - Iterates over a collection of color gradients and draws each ring with a separate color gradient over the duration of the effect.
    * _Color Bands_ - Applies a collection of colors to the whirlpool by drawing a small band of the whirlpool in each color.


* **Color** - Color gradient applied to the whirlpool when in *Single Color* color mode.

* **Bottom Color** - Color gradient applied to the bottom sides of each whirlpool when the **Color Mode** is *Side Colors*.

* **Left Color** - Color gradient applied to the left sides of each whirlpool when the **Color Mode** is *Side Colors*.

* **Right Color** - Color gradient applied to the right sides of each whirlpool when the **Color Mode** is *Side Colors*.

* **Top Color** - Color gradient applied to the top sides of each whirlpool when the **Color Mode** is *Side Colors*.

* **Band Length** - The length of each color band as a percentage of the display element when the **Color Mode** is *Color Bands*.

* **Colors** - The collection of color gradients when the **Color Mode** is *Color Rings* or *Color Bands*.

---

### Brightness

  * **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                    This is a legacy parameter, consider using intensity overlay layers instead.

---

#### Video Tutorial
