---
title: Snowstorm
author: Vixen Team
description: Creates an effect that mimics an intense snowstorm with snow falling sideways.
aliases: [/vixen-3-documentation/sequencer/effects/snowstorm/]
---

---

### Overview

Creates an effect that mimics an intense snowstorm with snow falling sideways.

---

### String Setup
    
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Speed** - How fast the snowflakes move.

* **Count** - How many snowflakes are in the effect at any given time.

* **Length** - The length of the tail on each snowflake.

* **Reverse Direction** - When checked, snowflakes move from left to right. When unchecked, snowflakes move from right to left.

---

### Color

    
* **Color Type**  - Controls the type of color for the snowstorm.
    * _Rainbow_ - Cycles through a rainbow of colors.
    * _Range_ - Each snowflake will be a single color selected from a range between the defined colors.  
    * _Palette_ - Each snowflake will be one of the specific colors/gradients defined in the color list.  
    * _Gradient_ - Uses gradients in the color list for each individual snowflake. 

* **Color** - Selects the color gradients used by **Color Types** _Range_, _Pallette_, and _Gradient_.

---

### Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/snowstorm/Snowstorm.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
