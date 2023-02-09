---
title: Fireworks
description: Creates an effect that simulates fireworks bursting in the sky.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/fireworks/]
---

---

## Overview

Creates an effect that simulates fireworks bursting in the sky. You can select to use random Fireworks, Fireworks to the Audio track or Fireworks to Marks in a Mark collection.

---

## Configuration

* **Fireworks Source** - Selects what source is used to determine explosions (_Standard Random Explosions_, _Mark Collections_, _Audio_)

* **Explosions** - The number of bursts over the duration of the effect.

* **Random Velocity** - Allows you to specify either a fixed velocity (speed) of the bursts when not checked, or when checked, a random velocity for each burst within a range from min to max.

* **Min Velocity** - Lower bound on the random burst velocity.

* **Max Velocity** - Upper bound on the random burst velocity.

* **Velocity** - Controls the velocity of the particls when **Random Velocity** is not selected.

* **Random Particles** - Controls the number of particles in each burst. If checked, allows you specify a maximum and minimum to define a range for particle count for each burst. If not checked, allows you to specify a fixed number of particles for all bursts.

* **Min Particles** - Lower bound on the number of random particles.

* **Max Particles** - Upper bound on the number of random particles.

* **Particles** - Controls how many particles will be created for each explosion when not using **Random Particles**.

---

## Color

* **Color Type** - Selects the type of color explosions between (_Standard Bursts_, _RainBow Particles_, _Range Particles_, _Palette Particles_, _Random Bursts_).

* **Colors** - Allows you to define one or more colors or gradients for the bursts. By defining multiple colors, you can allow for independent bursts of different colors. 
               If you use gradients rather than solid colors, you can have individual bursts that change from one color to another.

---

## Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.
                 
---

## Video Tutorial

{{< video src="/images/docs/usage/sequencer/effects/pixel/fireworks/Fireworks.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}

{{< youtube 7NWdu-J1ris>}}


---
