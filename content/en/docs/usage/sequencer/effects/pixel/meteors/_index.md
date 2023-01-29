---
title: Meteors
author: Vixen Team
description: Creates an effect that simulates falling meteors. Can also be used to create an explosion, or a swarm of flies.
aliases: [/vixen-3-documentation/sequencer/effects/pixel-lighting-effects/meteors/]
---

---

### Overview

Creates an effect that simulates falling meteors. Can also be used to create an explosion, or a swarm of flies.

---

### String Setup
  
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Motion** - Controls the type of meteor between (Falling, Random, and Explode).

* **Direction** - The direction of movement of the meteors.

* **Speed** - The speed at which all meteors move (available when Random motion is not selected)

* **Speed Variation** -  Allows you to add a bit of dynamic variation to the meteors.  This value combines with the Speed setting to allow each meteor to use a random speed.  The random speed will only deviate from the base speed by the amount of variation set here.

* **Count** - The number of meteors.

* **Tail Length** - The length of the meteor tail.

* **Tail Taper** - Controls the brightness taper of the meteor tails.

* **Start Position** - Determines where the meteors will start from (Random, Random the Zero Position, Zero Position)

* **Meteor Effects** - Applies special motion effects to the movement of the Meteors

* **Movement** - Adjusts the type of movement (None, Bounce, Wrap, Speed, Wobble, Wobble Both Directions).

* **Ground Level** - Adds a ground level for the meteors to hit.

* **GroundLevel** - A curve that establishes the ground level over the duration of the effect.

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

* **Ground Color** - Determines the color of the ground.  Only visible if the **Ground Level** curve is non-zero.

---

### Brightness

* **Intensity** - his is an overall brightness intensity curve over the duration of the effect. 
                  This is a legacy parameter, consider using intensity overlay layers instead.

---


#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/meteors/Meteors1.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
