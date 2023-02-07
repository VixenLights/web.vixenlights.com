---
title: Spin Color Wheel
author: Vixen Team
description: Spin Color Wheel effect spins the intelligent fixture color wheel.
aliases: [/vixen-3-documentation/sequencer/effects/intelligent-fixture/spin-color-wheel/]
---

---

### Overview

Spin Color Wheel effect spins the intelligent fixture color wheel.
The effect configures the rotation speed and intensity of the light beam.
The display preview will show a beam changing colors but does not attempt to reflect the rotation speed as that is hardware dependent.

---

### Configuration

* **Function** - The function on the intelligent fixture that controls the color wheel.  If the fixture supports more than one color wheel this is where you pick the desired color wheel.

* **Setting** - Index setting on the color wheel to pick the direction and rate of speed.

* **Rotation Speed** - Curve configures the rotation speed over the duration of the effect.  How this curve is interpreted by the fixture is determined by the selected Setting.

* **Intensity** - Intensity of the light beam over the duration of the effect.


---

### Requirements 

* For an intelligent fixture to support the Spin Color Wheel effect it must have the following:

  1. Color Wheel function with '_Spin Color Wheel_' tag.
  2. One or more Color Wheel index items with the Use Curve option selected.


---





