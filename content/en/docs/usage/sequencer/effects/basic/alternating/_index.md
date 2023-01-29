---
title: Alternating
author: Vixen Team
description: Creates an alternating effect.
aliases: [/vixen-3-documentation/sequencer/effects/basic-lighting-effects/alternating/]
---

### Overview

The **Alternating** effect does what it's name implies. It automates the process of alternating elements between colors. A simple example is a row of mini trees alternating back and forth from red to green.

![Alternating Settings Screen](/images/docs/usage/sequencer/effects/basic/alternating/Alternatingsettings-174x300.png)

![Alternating Trees](/images/docs/usage/sequencer/effects/basic/alternating/AlternatingTrees-300x31.png)

### Configuration

* **Timing Source** This sets the source of how the alternating timing occurs.
  * **Time Interval** This sets the timing of the alternates to be based on time.
    * **Change Interval** This controls the interval that the alternates change on. The value is in milliseconds.
    * **Static Effect** This option allows you to specify if the effect actually changes back and forth between colors over the duration of the effect or just sets up an alternating color pattern that is the same over the duration of the effect. This can be easily used to set alternating color patterns without having to use a pulse on all the individual elements. An example of this is the American flag that has red and white bars alternating, but are the same color for the length of the flag.
  * **Mark Collection** Since Version 3.5. This sets the reference for the alteranates to be based on the [Marks][5] in a Mark Collection. 
    * **Mark Collection** This allows you to choose the Mark Collection for the [Marks][5] to be used in aligning the alternates. The following is an example of being aligned to the Marks.

        ![Alternating Aligned to Marks](/images/docs/usage/sequencer/effects/basic/alternating/AlternatingMarks-300x88.png)
* **Group Level** Specifies how many elements are of the same color before switching to the next color in the list. In the case of pixels with color of red and white set, if you set it to 5, there will be 5 lights that are red and then 5 that are green and then 5 more red and back to green and so on. This works for non pixel elements as well. The default is 1.
* **Change Interval** Defines on a non static effect, how often the colors switch back and forth. It is specified in ms. So if you want the colors to switch back and forth every 500 ms, set it to 500.
* **Color offset** Specifies how many colors to jump when the alternating pattern starts over. This can create interesting marquee style effect.

---

### Color

* **Gradients** This allows you to choose the color sets to be used. The alternating supports what we can a Color Gradient Level Pair. In this case the color and the brightness level work together. With this you can specify fading colors or any other combination. This works just like a pulse, only within that color portion of the alternating. Each [Color Gradient][3] has a [Curve][1] to control it. You can add or remove these pairs of colors. Both the [Color Gradient][3] and the [Curve][1] support drag and drop. See [Inline Curve Editor][2] and [Inline Gradient Editor][4].

---

### Depth

* **Levels Deep** When enabled it controls at what level the **Alternating** is applied inside a group of elements. So you can have 8 items and then have 4 of them grouped to the left and 4 grouped to the right. All of these are grouped under on group. By placing the **Alternating** at the top level group, you can **Alternating** all 8 of the items or the left and the right group as a pair.

---

### Tutorials

{{< youtube id="A5DrPmhCIqo" title="Using Marks with the Alternating Effect">}}

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
[5]: {{< ref marks>}} "Marks"
