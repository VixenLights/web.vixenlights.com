---
title: Snowflakes
author: Vixen Team
description: Creates an effect that simulates falling snowflakes.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/snowflakes/]
---

---

### Overview

Creates an effect that simulates falling snowflakes.

---

### String Setup
    
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Snowflake Type** - The number of tips on the snowflakes, or a random, mixed collection.  

* **Include 45pt** - When _Random_ is selected, this option determines whether the large and complex 45pt flakes are included.

* **Motion** - Controls the motion of the snowflakes between _Falling_, _Random_, _Explode_, _Grid_, and _Grid Offset_.

* **Fade** - Controls the type of fade applied to each snowflake (_None_, _In_, _Out_, _In/Out_).

* **Snow Build-up** - Allows the snowflakes to build up at the bottom of the display element.

* **Build-up Speed** - Adjusts how fast the build up of snow is over the duration of the effect.

* **Initial Build-up** - Sets the height level of the initial snow build-up at the bottom of the display element.

* **Min Angle** - Minimum angle the snowflake moves.  Applicable when the **Motion** is set to _Random_.

* **Max Angle** - Maximum angle the snowflake moves.  Applicable when the **Motion** is set to _Random_.

* **Speed** - Controls the base speed of the snowflake motion.

* **Speed Variation** - The amount of variation from the base speed for the snowflakes over the duration of the effect.
                        This allows you to add some dynamic variation to the falling speed of the snowflakes. 
                        The speed will only deviate from the base speed by the rate set here.

* **Horizontal Flake Count** - Controls the number of horizontal snowflakes.

* **Verical Flake Count** - Controls the number of vertical snowflakes.

* **Flake Count** - The number of snowflakes in the pattern over the duration of the effect.

* **Movement** - Adjusts the type of movement.

* **Random Intensity** - Uses a random Brightness/Intensity for each snowflake.

### Movement

This category is visible when the **Movement** is set to _Speed_, _Wobble_, or _Wobble Both Directions_.

* **Horizontal Center Speed** - Horizontal center speed.

* **Horizontal Speed Variation** - Randomly adjust the speed around the **Horizontal Center Speed** by the amount of variation.

* **Vertical Center Speed** - Vertical center speed.

* **Vertical Speed Variation** - Randomly adjust the speed around the **Vertical Center Speed** by the amount of variation.

* **Wobble** - Controls the wobble of the snowflakes.  This setting is only applicable when the **Movement** is set to _Wobble_ or _Wobble Both Directions_.

* **Wobble Variation** - Randomly adjust the wobble around the **Wobble** level by the variance over the duration of the effect.

---

### Color

* **Color Type** - Controls the Type of color.
    * _Range_ - Requires multiple colors/gradients. Flakes will appear in a range of colors bounded by the colors defined in the color/gradient lists.  
    * _Palett_ - Snowflakes will appear in the specific color(s) defined in the color/gradient lists.  
    * _Rainbow_ - Applies a cycling rainbow of color to each snowflake
    * _Alternate_ 

* **Center Color** - The color of the center point of each snowflake. When a gradient is used, each snowflake uses a fixed color centerpoint, but the centerpoint of each snowflake will be the color of the point in the gradient in time when that snowflake appears.

* **Outer Color** - The color for the arms and tips of the snowflake. When a gradient is used, each snowflake uses a fixed color for the arms and tips, but the color of each snowflake will be the color of the point in the gradient in time when that snowflake appears.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.



#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/snowflakes/Snowflakes.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
