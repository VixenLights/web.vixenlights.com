---
title: Twinkle
author: Vixen Team
description: Creates a twinkling effect.
aliases: [/vixen-3-documentation/sequencer/effects/twinkle/]
---

### Overview

The **Twinkle** effect was designed to simulate the effect of twinkling lights on a Prop. 

---

### Color

* **Color Handling** This controls how the colors are applied on the effect. The simplest is a single color which will create a simple Twinkle with only that color on it. The other three options allow for a [Color Gradient][3] to be applied in different ways on the effect. See [Inline Gradient Editor][4].
  * **Single Color** This sets the color to be a simple color.
  * **Gradient Thru Effect** This will transition the colors on the Twinkle over time to match the colors in the gradient. This allows you to have  a Twinkle that goes from say red to blue over the duration.
  * **Gradient Per Pulse** Each individual pulse within the Twinkle will have the gradient applied to it. Each pulse will have the same color. So the pulse can go from red to blue.
  * **Gradient Across Items** The gradient will be applied proportionately over group of items that the Twinkle covers with each item receiving the color within the gradient that corresponds to it's percentage of the entire group.
* **Color Gradient / Color** Depending on the **Color Handling** setting this will allow the simple color, or the [Color Gradient][3] to be set. See [Inline Gradient Editor][4].

---

### Brightness

* **Max** Controls the maximum brightness of the twinkles.
* **Min** Controls the minimum brightness of the twinkles.
* **Variation** Controls the percent variation in the brightness of each twinkle.

---

### Configuration

* **Avg Pulse Time** Controls how long the average pulse time of each twinkle is in milliseconds.
* **Coverage** Controls what percentage of the Prop is covered by twinkles.
* **Variation** Controls the percent variation in the time of each twinkle.
  
---

### Depth

* **Levels Deep** When enabled it controls at what level the **Twinkle** is applied inside a group of elements. So you can have 8 items and then have 4 of them grouped to the left and 4 grouped to the right. All of these are grouped under on group. By placing the **Twinkle** at the top level group, you can **Twinkle** all 8 of the items or the left and the right group as a pair.

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
