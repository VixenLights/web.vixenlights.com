---
title: Twinkle
author: Vixen Team
description: Creates a twinkling effect.
aliases: [/vixen-3-documentation/sequencer/effects/twinkle/]
---

## Overview

The **Twinkle** effect was designed to simulate the effect of twinkling lights on a Prop.

---

## Color

* **Color Handling** This controls how the colors are applied on the effect. The simplest is a single color which will create a simple Twinkle with only that color on it. The other three options allow for a [Color Gradient][3] to be applied in different ways on the effect. See [Inline Gradient Editor][4].
  * **Single Color** This sets the color to be a simple color.
  * **Gradient Thru Effect** This will transition the colors on the Twinkle over time to match the colors in the gradient. This allows you to have a Twinkle that goes from say red to blue over the duration.
  * **Gradient Per Pulse** Each individual pulse within the Twinkle will have the gradient applied to it. Each pulse will have the same color. So the pulse can go from red to blue.
  * **Gradient Across Items** The gradient will be applied proportionately over group of items that the Twinkle covers with each item receiving the color within the gradient that corresponds to its percentage of the entire group.
* **Color Gradient / Color** Depending on the **Color Handling** setting this will allow the simple color, or the [Color Gradient][3] to be set. See [Inline Gradient Editor][4].

---

## Brightness

* **Max** Controls the peak brightness a twinkle pulse can reach.
* **Min** Controls the baseline brightness maintained across the whole effect. Each twinkle pulse ramps up from this level and back down to it, rather than starting from fully off.
* **Variation** Controls how much the peak brightness of each individual twinkle randomly varies below **Max**, as a percentage of the Min-Max range. Higher values mean some twinkles will noticeably dimmer than others instead of all peaking at the same brightness.

---

## Configuration

* **Avg Pulse Time** Controls how long the average pulse time of each twinkle is in milliseconds. The default is 400 ms.
* **Coverage** Controls how densely packed the twinkles are in time — essentially how much of the time an element spends twinkling versus sitting idle at the minimum brightness between twinkles. Higher values produce more frequent, overlapping twinkles; lower values produce sparser, more occasional ones. This is a percentage, and the default is 50%.
* **Variation** Controls the percent variation in the time (duration) of each twinkle, relative to **Avg Pulse Time**.

---

## Depth

* **Effect Depth** Controls whether each targeted element twinkles independently, or whether elements are grouped together and twinkle in sync. Enabled by default.
  * When **enabled**, this reveals the **Levels Deep** option below, and every element or group at that depth is given its own independently randomized twinkle pattern — this is the classic, organic-looking twinkle.
  * When **disabled**, grouping is turned off entirely (the effect always targets individual leaf elements, regardless of **Levels Deep**), and every element is given the exact same randomly generated twinkle pattern, so they all twinkle in perfect sync rather than independently. This can be useful for a uniform pulsing look across a whole prop.
* **Levels Deep** Only shown when **Effect Depth** is enabled. Controls at what level the **Twinkle** is applied inside a group of elements. So you can have 8 items and then have 4 of them grouped to the left and 4 grouped to the right. All of these are grouped under one group. By placing the **Twinkle** at the top level group, you can **Twinkle** all 8 of the items or the left and the right group as a pair — with each group's twinkle pattern still independently randomized from the other group's. The default is 0, which targets individual leaf elements.

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
