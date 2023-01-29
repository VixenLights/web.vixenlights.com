---
title: Chase
author: Vixen Team
description: Creates a chasing effect.
aliases: [/vixen-3-documentation/sequencer/effects/basic-lighting-effects/chase/]
---

### Overview

The **Chase** Effect allows you to have a series of **Pulse** effects spaced out across the duration of the effect. Instead of having to place and distribute individual pulses over time, this effect will do the math to distribute them evenly for you.

---

### Behavior

Since Version 3.6u1

* **Across Elements/Groups** is the default behavior and is equivalent to how the effect acted prior. When the effect is applied on an element that has multiple levels deep, then the Behavior section will appear.

* **Each Element/Group** This is a new behavior that changes how the effect looks at the elements and targets them. Previously you could use the levels and chase across a group of Arches or similar props, but if you wanted to apply the same chase to each Arch in the group, you would need to put a Chase on each Arch specifically. Now you can choose the Each Element/Group behavior and the proper level to get an identical Chase on each arch. This also allows the possibility to Chase up/down a Pixel tree instead of just around it. Many combinations are possible using variations of the Behavior and Level options.

---

### Color

* **Color Handling** This controls how the colors are applied on the effect. The simplest is a single color which will create a simple chase with only that color on it. The other three options allow for a [Color Gradient][3] to be applied in different ways on the effect. See [Inline Gradient Editor][4]
  * **Single Color** This sets the color to be a simple color.
  * **Gradient Thru Effect** This will transition the colors on the chase over time to match the colors in the gradient. This allows you to have  a chase that goes from say red to blue over the duration.

    ![Gradient Thru Effect](/images/docs/usage/sequencer/effects/basic/chase/GradientThruEffect-300x38.png)

  * **Gradient Per Pulse** Each individual pulse within the chase will have the gradient applied to it. Each pulse will have the same color. So the pulse can go from red to blue.

    ![Gradient Per Pulse](/images/docs/usage/sequencer/effects/basic/chase/GradientPerPulse-300x41.png)

  * **Gradient Across Items** The gradient will be applied proportionately over group of items that the chase covers with each item receiving the color within the gradient that corresponds to it's percentage of the entire group.

    ![Gradient Accross Items](/images/docs/usage/sequencer/effects/basic/chase/GradientAcrossItems-300x38.png)
* **Color Gradient / Color** Depending on the **Color Handling** setting this will allow the simple color, or the [Color Gradient][3] to be set. See [Inline Gradient Editor][4].
  
---

### Brightness

* **Pulse Intensity** This setting controls the shape of the pulse [Curve][1]. Much like the same setting in the pulse effect, you can control is each pulse ramps up or down or any shape you can design with the [Curve][1]. See [Inline Curve Editor][2].

    The default setting represents a ramping on motion where each portion of the chase ramps up to full brightness

    ![Ramp Up](/images/docs/usage/sequencer/effects/basic/chase/PulseIntensityRamp-300x21.png)

    The shows a pulse ramping up and then down just by altering the shape of the [Curve][1] into a ^ shape.

    ![Ramp Up and Down](/images/docs/usage/sequencer/effects/basic/chase/PulseIntensityRampUpDown-300x23.png)

---

### Direction

* **Direction** This [Curve][1] controls the direction the chase moves across items. In it's simple form it is right to left, or left or right. But you can design custom movements to have it move right and then back left in the same effect. See [Inline Curve Editor][2]

    Normal Direction

    ![Forward Direction](/images/docs/usage/sequencer/effects/basic/chase/DirectionNormal-300x26.png)

    Reversing Direction

    ![Reverse Direction](/images/docs/usage/sequencer/effects/basic/chase/DirectionBothWays-300x25.png)

---

### Pulse

* **Extend Pulse To End** Extends the pulses to the end of the effect to enable a chase to on type effect. Each pule will foloow the curve and then maintain the last intensity to the end of the effect. Pulse Intensity must be above zero on the curve at the end.

    ![Extend To End](/images/docs/usage/sequencer/effects/basic/chase/ExtendToEnd-300x20.png)

* **Extend Pulse To Start**. This is the opposite of etendign to end. This allows the effect to be all on at the start, and then chase the elements off. Pulse Intensity must be > 0 at the beginning of the curve.

    ![Extend To Start](/images/docs/usage/sequencer/effects/basic/chase/ExtendToStart-300x21.png)

* **Pulse Overlap** Controls how much the pulses of the chase overlap with each other. This can be used to create a more smooth flowing effect by adding more overlap.

    Zero overlap

    ![Zero Pulse Overlap](/images/docs/usage/sequencer/effects/basic/chase/DirectionNormal-300x26.png)

    200 ms overlap

    ![200ms Pulse Overlap](/images/docs/usage/sequencer/effects/basic/chase/PulseOverlap-300x33.png)

---

### Depth

* **Levels Deep** Controls at what level the **Chase** is applied inside a group of elements. So you can have 8 items and then have 4 of them grouped to the left and 4 grouped to the right. All of these are grouped under on group. By placing the **Chase** at the top level group, you can **Chase** all 8 of the items or the left and the right group as a pair.

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
