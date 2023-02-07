---
title: Snap points
author: Vixen Team
weight: 80
description: This section covers the Snap Point features.
---

### Overview

Snap Points are a common feature in many drawing or editing applications. Vixen provides a very powerful version of this feature to enable snapping effects to things like marks or other effects. There are two items in the editor that support snapping. Those are [Marks][1] and Effects.

### Configuration

Snap points can be enabled with the Magnet icon in the tool bar. When the Magnet icon is selected, the feature will be enabled. To the right of the Magnet icon is a drop down that will allow you to select the strength multiplier of the snap. This governs how close something needs to be to the other object for it to snap into place. 1 is the weakest and 4 is the strongest.

### Snapping to Effects

Effects support snapping to each other. When dragging or resizing an Effect, when it geets close to to another Effect it will jump to or attract to the other Effect. This enables you to easily get two effects back to back without trying to align them precisly. Effects favor being glued to another Effects.

### Snapping to Marks

In addition to snapping an Effect to another Effect, they will also attract to [Marks][1]. This makes it easy to align an effect to a Mark when you are editing them. There are other [Alignment tools][3] for aligning effect to Marks as well. Effects will favor another Effect over a Mark when they are in the same area. You can increase the strength of the Marks in the Mark Docker by increasing their [Weight][2] setting.

[1]: {{< ref marks>}}
[2]: {{< ref "marks#mark-weight">}}
[3]: {{< ref "alignment-helpers#mark-alignment">}}
