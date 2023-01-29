---
title: Spin
description: Creates a spinning effect.
aliases: [/vixen-3-documentation/sequencer/effects/basic-lighting-effects/spin/]
---
The **Spin** is similar to the [Chase][5] effect. It can be thought of as repeating chases back to back which creates a spinning effect.

### Behavior

Since Version 3.6u1

* **Across Elements/Groups** is the default behavior and is equivalent to how the effect acted prior. When the effect is applied on an element that has multiple levels deep, then the Behavior section will appear.

* **Each Element/Group** This is a new behavior that changes how the effect looks at the elements and targets them. Previously you could use the levels and spin across a group of Arches or similar props, but if you wanted to apply the same Spin to each Arch in the group, you would need to put a Spin on each Arch specifically. Now you can choose the Each Element/Group behavior and the proper level to get an identical Spin on each arch. This also allows the possibility to Spin up/down a Pixel tree instead of just around it. Many combinations are possible using variations of the Behavior and Level options.

---

### Color

* **Color Handling** This controls how the colors are applied on the effect. The simplest is a single color which will create a simple Spin with only that color on it. The other three options allow for a [Color Gradient][3] to be applied in different ways on the effect. See [Inline Gradient Editor][4]
  * **Single Color** This sets the color to be a simple color.
  * **Gradient Thru Effect** This will transition the colors on the Spin over time to match the colors in the gradient. This allows you to have  a Spin that goes from say red to blue over the duration.

    ![Gradient Thru Effect](/images/docs/usage/sequencer/effects/basic/chase/GradientThruEffect-300x38.png)

  * **Gradient Per Pulse** Each individual pulse within the Spin will have the gradient applied to it. Each pulse will have the same color. So the pulse can go from red to blue.

    ![Gradient Per Pulse](/images/docs/usage/sequencer/effects/basic/chase/GradientPerPulse-300x41.png)

  * **Gradient Across Items** The gradient will be applied proportionately over group of items that the Spin covers with each item receiving the color within the gradient that corresponds to it's percentage of the entire group.

    ![Gradient Accross Items](/images/docs/usage/sequencer/effects/basic/chase/GradientAcrossItems-300x38.png)
* **Color Gradient / Color** Depending on the **Color Handling** setting this will allow the simple color, or the [Color Gradient][3] to be set. See [Inline Gradient Editor][4].
  
---

### Brightness

* **Pulse Intensity** This setting controls the shape of the pulse [Curve][1]. Much like the same setting in the pulse effect, you can control is each pulse ramps up or down or any shape you can design with the [Curve][1]. See [Inline Curve Editor][2].

    The default setting represents a ramping on motion where each portion of the chase ramps up to full brightness

    ![Ramp Up](/images/docs/usage/sequencer/effects/basic/chase/PulseIntensityRamp-300x21.png)

    The shows a pulse ramping up and then down just by altering the shape of the [Curve][1] into a ^ shape.

    ![Ramp Up and Down](/images/docs/usage/sequencer/effects/basic/chase/PulseIntensityRampUpDown-300x23.png)

* **Minimum Brightness** This allows you to set a minimum level of the color across areas that are not spinning. So you could have a green spin over a dim green background. The background will have the same color attibutes chosen above.
  * **Minimum Level** Enabled when you choose minimum brightness and allows you to set the 0 - 100 percent intensity via a slider.

---

### Direction

* **Direction** the direction the spin rotates can be choosen from this drop down. The possible values are Forward and Reverse.

---

### Speed

* **Speed Format** This controls the way the speed of the spin is controlled.
  * **Revolution Count** This sets the speed to be a number of revolutions over the span of the effect.
    * **Count** The number of revolutions.
  * **Revolution Frequency** This controls the speed as a factor of frequency over the span of the effect.
    * **Revolution** The frequency of the revolutions.
  * **Fixed Time** This controls the speed of the spin as a function of time.
    * **Revolution Time** Time in milliseconds for a revolution to take.

---

### Pulse

* **Pulse Type** This controls the type of the pulse behavior.
  * **Distribute Evenly** This distributes the pulses evenly over the timespan of the revolution. This is the default.
  * **Fixed Time** This sets the duration of each pulse in milliseconds.
    * **Duration** Duration of the pulse in milliseconds.
  * **Percent Revolution** This sets the duration of the pulse to be a percent of the revolution time.
    * **Pulse Length** A 0 - 100 percent value determining the percent of the revolution.

---

### Depth

* **Levels Deep** Controls at what level the **Spin** is applied inside a group of elements. So you can have 8 items and then have 4 of them grouped to the left and 4 grouped to the right. All of these are grouped under on group. By placing the **Spin** at the top level group, you can **Spin** all 8 of the items or the left and the right group as a pair.

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
[5]: {{< ref "chase">}}
