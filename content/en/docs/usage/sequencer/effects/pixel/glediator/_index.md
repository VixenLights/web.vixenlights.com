---
title: Glediator
description: Creates an effect that is used to import effects created with the Glediator application.
aliases: [/vixen-3-documentation/sequencer/effects/glediator/]
---

---

## Overview

Creates an effect that is used to import effects created with the Glediator application.
More information on glediator can be found at:
[Glediator Website and Download][1]

Notes: You will need to change the Glediator Matrix size to match the Vixen matrix size you are using the effect on.

---

## Jinx

Jinx! can be used to create files to import to this effect also. In Jinx!, you will need to specify to output to Glediator file, which writes an .out file after starting output in Jinx! It is the .out file that you rename to .gled and then Vixen can read it using the Glediator effect.

[Jinx! Website][2]

---

## String Setup

* **Orientation** - Controls the orientation of the display area (matrix).
  
---

## Movement

* **Movement Type** - Select between _Iterations_ or _Speed_.  When set to iterations, the **Iterations** slider will adjust the number of times the pattern will repeat over the duration of the effect.
When Movement Type is set to Speed, the **Speed** slider will control the speed of each iteration.

* **Iterations** - Controls how many times the pattern repeats over the timespan.

* **Speed** - Controls the speed of the pattern.

---

## Configuration

* **File Name** - Selects the Glediator file you wish to use.

---

## Brightness

* **Intensity** - This is an overall brightness intensity curve over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

 [1]: https://lededittm.com/glediator-software-download-for-led-matrix-control/
 [2]: https://live-leds.de
