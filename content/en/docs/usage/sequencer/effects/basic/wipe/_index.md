---
title: Wipe
author: Vixen Team
description: Creates a wiping effect.
aliases: [/vixen-3-documentation/sequencer/effects/basic-lighting-effects/wipe/]
---

### Overview

The Wipe was one of the first location aware effects in Vixen. The goal of this effect is somewhat similar to the [Chase][5], however it is aware of the position of the elements as defined in the Preview. It uses this location awareness to simulate a chase across all of its elements in a Wiping fashion.

![Wipe Settings Screen](/images/docs/usage/sequencer/effects/basic/wipe/Wipe_Properties-216x300.jpg)

### Type

* **Movement**
  * **Count** This sets the number of wipe passes in the timespan of the effect.
    * **Wipe Count** The number of wipes.
    * **Wipe On** When enabled, the wipe will maintiain the elements in the on state as the wipe moves across.
    * **Wipe Off** When enabled, the wipe will start out on and wipe off across the prop.
  * **Pulse Length** This controls the wipe by a measure of the pulse length.
  * **Movement** This controls the wipe by the movement curve.

The Wipe on/off options are similar to the [Chase][5] extend to start/end options. These are most useful for wiping the stage on or off. The pulses have the same rules as the [Chase][5] and need to have a > zero end value for wiping on and a > zero start value for wiping off. The default pulse curve has a zero start and end value, so to use this you would need to adjust to a ramp on  for the wipe on case or ramp off for wipe off as an example.

---

### Direction

* **Direction** It can move in a number of directions, horizontal, vertical, diagonal up, diagonal down, burst, circle burst and diamond burst.
* **Reverse Direction** When enabled, the direction will be reversed.

---

### Color

* **Color Handling** This controls how the colors are applied on the effect. The simplest is a single color which will create a simple Twinkle with only that color on it. The other three options allow for a [Color Gradient][3] to be applied in different ways on the effect. See [Inline Gradient Editor][4].
  * **Gradient Thru Effect** This will transition the colors on the **Wipe** over time to match the colors in the gradient. This allows you to have a **Wipe** that goes from say red to blue over the duration.
  * **Gradient Across Items** The gradient will be applied proportionately over group of items that the **Wipe** covers with each item receiving the color within the gradient that corresponds to it's percentage of the entire group.
* **Color Gradient** Sets the [Color Gradient][3] to be used. See [Inline Gradient Editor][4].

---

### Brightness

* **Intensity** This sets the [Curve][1] that controls the intensity of the color over the effect. See [Inline Curve Editor][2].

### Pulse

* **Pulse Length** The pulse length is also similar to the pulse overlap feature of the [Chase][5] and allows for the pulses to be adjusted to smooth out the Wipe or lengthen the amount of visible time any part of the lights are lit.

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
[5]: {{< ref "chase">}}
