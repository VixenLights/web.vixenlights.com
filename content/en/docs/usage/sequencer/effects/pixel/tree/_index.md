---
title: Tree
author: Vixen Team
description: Creates an effect that simulates wrapping garland around a tree.
aliases: [/vixen-3-documentation/sequencer/effects/tree/]
---

---

### Overview

Creates an effect that simulates wrapping garland around a tree.
This effect is best used on megatrees.

---

### String Setup
    
  * **Orientation** - Controls the orientation of the display area (matrix).
---

### Configuration

* **Speed:** - How fast the garlands are drawn around the tree.

* **Overall Intensity** - The overall intensity envelope of the entire effect over the duration of the effect.

---

### Tree

* **Color** - One or more colors or gradients to be applied to the text. One color will be applied to each line of text.

* **Intensity** - The intensity of the tree background over the duration of the effect.

---

### Branches

* **Branch Direction** - The direction in which the branches are drawn (_Up_, _Down_, _Left_, _Right_, _Up/Right_, _Up/Left_, _Down/Right_, _Down/Left_, _Alternate_, _None_).

* **Branches** - The number of branches to divide the tree into.  Determines the number of garland rings to apply to the tree.

* **Color Type** - How colors are applied to the garlands.  
    * _Static_ - One color/gradient per garland level.
    * _Twinkle_ - Each pixel in the garland twinkles thru the defined colors.
    * _Alternate Segment_ - Each swagged segment of garland is colored alternately through the list of defined colors.  
    * _Alternate Pixel_ - Each pixel is colored by rotating through the list of defined colors.

* **Color** - One or more colors/gradients used to color the garlands around the tree.

---

### Blending

* **Blend** - Adjusts the amount of blending or tapering of each branch level.

* **Blend Direction** - Determines the direction of the blend.

---

#### Video

{{< video src="/images/docs/usage/sequencer/effects/pixel/tree/Tree.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}
