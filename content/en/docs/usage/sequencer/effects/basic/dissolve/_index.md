---
title: Dissolve
author: Vixen Team
description: Creates a Dissolving or Filling effect.
aliases: [/vixen-3-documentation/sequencer/effects/Dissolve/]
---

### Overview

TThe **Dissolve** effect simulates colors disolving from, or filling into a space. The effect name of Dissolve may seem to suggest that it can only dissolve, but it also supports the opposite with filling color into an element. It has many settings to adjust how the effect behaves.

![Dissolve](/images/docs/usage/sequencer/effects/basic/dissolve/dissolve-199x300.jpg)

---

### Configuration

* **Timing Source** Controls if the effect is driven by the time duration, or by [Marks][5] in a Mark Collection.
* **Density** A [Curve][1] that governs how dense the coverage of the elements and how the dissolve itself acts. See the [Inline Curve Editor][2].
* **Group Level** Controls how many elements in the group have the same Dissolve applied to them. Defaults to 1 meaning each element gets it's own unique Dissolve.
* **Random Disolve** Controls if the Disolve pattern is random (Checked) as to the order elements Disolve, or if the user can take more control.
  * **Starting Element** Starting location where the Dissolve or Fill will commence from.
  * **Dissolve Flip** Flips the direction of the sequential Dissolve.
  * **Both Directions** Dissolves or Fills in both directions, one after the other.

---

### Color

* **Gradients** Sets the [Color Gradient][3] and intensity [Curve][1] for the effect. You can have more than one Gradient and each Gradient will have its own intensity [Curve][1]. See the [Inline Gradient Editor][4] and [Inline Curve Editor][2].
* **Color Per Step** When enabled, color will change for each step variation. When disabled, each step variation will have all colors.
* **Random Color Order** When enabled the colors will be chosen at random instead of in order.
* **Group Color** When enabled, each element will have all colors generated in parallel.

---

### Depth

* **Effect Depth** Controls the depth level in groups that the effect should be applied to. If there are multiple levels of props in a group, the same Dissolve can be applied to each group instead of using multiple effects by using this setting.

---

[1]: {{< ref curves>}}
[2]: {{< ref inline-curve-editor>}}
[3]: {{< ref color-gradients>}}
[4]: {{< ref inline-gradient-editor>}}
[5]: {{< ref marks>}}
