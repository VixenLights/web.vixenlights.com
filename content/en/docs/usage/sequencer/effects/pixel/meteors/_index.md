---
title: Meteors
author: Vixen Team
description: Creates an effect that simulates falling meteors. Can also be used to create an explosion, or a swarm of flies.
aliases: [/vixen-3-documentation/sequencer/effects/meteors/]
---

---

## Overview

Creates an effect that simulates falling meteors. Can also be used to create an explosion, or a swarm of flies.

---

### String Setup
  
* **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Motion** - Chooses the overall meteor movement style.
  * _Falling_ - Uses the selected direction.
  * _Random_ - Creates meteors within the min/max angle range.
  * _Explode_ - Sends meteors outward from the center.

* **Direction** - The direction of movement of the meteors.

* **Speed** - Controls the base speed of the meteors over the effect duration. Speed Variation is applied around this value to create slower and faster individual meteors. (available when Random motion is not selected)

* **Speed Variation** -  Controls how much individual meteor speeds vary from the main Speed value. Higher values create a wider mix of slow and fast meteors. The random speed will only deviate from the base speed by the amount of variation set here.

* **Count** -  Controls how many meteors are active during the effect. Higher values create a denser meteor field.

* **Tail Length** - The length of the meteor tail.

* **Tail Taper** - Controls the brightness taper of the meteor tails.

* **Start Position** - Determines where the meteors will start from (Random, Random the Zero Position, Zero Position)

* **Meteor Effects** - Applies special motion effects to the movement of the Meteors

* **Movement** - Adjusts the type of movement (None, Bounce, Wrap, Speed, Wobble, Wobble Both Directions).

* **Ground Level Enable** - Adds a ground level for the meteors to hit.

* **Ground Level** -  A Curve that sets the height of the ground area across the display when ground level is enabled. Meteors stop and break up when they hit this area.

* **Flip Direction** - Flips the directions the meteors will move.

* **Count Per String** - Generates meteors for each string.

---

### Color

* **Color Type** - Selects how colors are applied to the effect.
  * _Rainbow_ - Uses random colors on all meteors and their tails  
  * _Range_ - Uses one solid color for each meteor. The colors are chosen from a range between the colors/gradients in the gradient list.  
  * _Palette_ - Uses one solid color for each meteor. The colors are chosen from the specific colors/gradients in the gradient list.  If the colors in the list are gradients, only the starting color is used.  
  * _Gradient_ - Uses one gradient for each meteor. The gradients are chosen from the specific colors/gradients in the gradient list.

* **Gradients:** The colors/gradient list used by the effect.  See the color type above for how the colors/gradients are applied.

* **Ground Color** -  Sets the color gradient used to draw the ground area when ground level is enabled. Only visible if the **Ground Level** curve is non-zero.

---

### Brightness

* **Intensity** - his is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/meteors/Meteors1.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
