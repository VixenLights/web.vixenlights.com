---
title: Candle Flicker
author: Vixen Team
description: Creates a candle flicker effect.
aliases: [/vixen-3-documentation/sequencer/effects/candle-flicker/]
---

## Overview

The **Candle Flicker** effect was designed to simulate the effect of a candle flickering. It has many settings to adjust how the flicker behaves.

---

## Configuration

* **Group Level** Controls how many elements in the group have the same flicker applied to them. Elements are grouped in blocks of this size, and every element in a block shares the same randomly generated flicker pattern. Range is 1-5000. Defaults to 1, meaning each element gets its own unique flicker.

---

## Color

* **Color** Sets the single solid color used for the flicker. Unlike some other effects, Candle Flicker does not support a Color Gradient — only brightness is varied over time.

---

## Brightness

* **Max** Controls the maximum brightness a flicker can reach. This is a 0-100 percent range of the overall color brightness. Default is 100%.
* **Min** Controls the minimum brightness a flicker can drop to. This is a 0-100 percent range of the overall color brightness. Default is 10%.

---

## Flicker

The flicker is generated as a series of random brightness steps between the **Min** and **Max** brightness. Each step has a duration and a size, and both are randomized around the values below so that no two flickers look exactly alike.

* **Frequency** Sets the baseline flicker rate, in changes per second. For example, a value of 20 targets a new brightness step roughly every 1000/20 = 50 ms on average. The actual duration of each step is then randomized using **Flicker** below. Default is 20.
* **Change Percent** Sets the average size of each brightness step, as a percentage of the overall brightness range. The actual size of each step is then randomized using **Deviation** below, and each step is randomly chosen to move brightness up, down, or not at all. Default is 20%.
* **Flicker** Sets how much the timing of each step can randomly deviate from the **Frequency** setting, as a percentage. Higher values make the flicker's timing less regular. Default is 25%.
* **Deviation** Sets how much the size of each brightness step can randomly deviate from the **Change Percent** setting, as a percentage. Higher values make the flicker's intensity less consistent. Default is 50%.
