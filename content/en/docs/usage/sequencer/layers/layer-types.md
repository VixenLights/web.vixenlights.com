---
title: Layer Types
author: Vixen Team
weight: 10
description: This section covers the Layer Types.
---

## Overview

Layers are a method of controlling how separate Effects on the same element interact with each other. It can be very powerful to create variations on the existing effects. Each layer (other than Default) has a mixer assigned to it in the [Layer Editor]({{< ref layer-editor >}}), and that mixer defines how the effects in the layer combine with whatever is in the layer immediately below it.

Throughout this page, "higher layer" refers to the layer the mixer is assigned to, and "lower layer" refers to the result of everything beneath it. If you stack more than two layers, mixing happens one pair at a time from the top down, so the "lower layer" a mixer sees may already be a blend of several layers below it.

Some mixers **require a mixing partner** — they only make sense when there is an effect in the layer below to combine with. If a layer's mixer requires a partner and there is no effect on a lower layer at that moment in time, the higher layer's effect will not be visible either, rather than showing on its own.

### Highest Value (Default)

Highest Value is the mixer every new layer starts with, and it's also the same behavior the old Default layer has always used. For each color channel, it simply keeps whichever of the two layers is brighter. There's no configuration, and it doesn't require a mixing partner — an effect in a layer using Highest Value will show normally even if nothing is on the layer below.

### Intensity Overlay

The Intensity Overlay Layer takes the brightness of the higher layer's effect and uses it to scale the brightness of the lower layer, without changing the lower layer's color. This is useful for fading or pulsing effects that don't already have a level curve applied — for example, placing a white pulse effect in an Intensity Overlay layer will cause whatever is beneath it to dim and brighten along with the pulse. Intensity Overlay requires a mixing partner, so it has no effect on its own without something in a lower layer.

### Mask

The Mask Layer uses the higher layer's effect to cut out, or mask, parts of the effect(s) beneath it. Anywhere the higher layer's effect is lit, the lower layer is fully blacked out at that point; anywhere the higher layer is unlit, the lower layer passes through unchanged. The color of the masking effect doesn't matter — only whether it is lit or not.

### Mask and Fill

Mask and Fill works like Mask, but instead of leaving unlit gaps where the masking effect is, it fills those areas with the masking effect's own color. The result is the higher layer's effect drawn directly on top of the lower layer, using the higher layer's exact colors rather than a blend. This mixer has a Configuration dialog with two options:

- **Exclude zero values** (on by default) — areas where the higher layer's effect has zero brightness show the lower layer instead of black. Turning this off makes the higher layer fully replace the lower layer everywhere, including its unlit gaps.
- **Require Mixing Partner** (off by default) — when enabled, the higher layer's effect will only display where a lower layer effect also exists at that time.

### Color Change

Color Change replaces the color of the lower layer with the color of the higher layer's effect, while preserving the lower layer's brightness/intensity. This lets you recolor an existing effect by placing a differently-colored effect above it, without affecting its timing or brightness pattern. Color Change requires a mixing partner.

### Proportional Mix

Proportional Mix blends the two layers based on the higher layer's brightness: as the higher layer's effect gets brighter, it proportionally overtakes the lower layer at that point, and as it dims, more of the lower layer shows through. Unlike Mask, which is an all-or-nothing cutout, Proportional Mix produces a smooth cross-fade between the two effects.

### Multiply Color

Multiply Color uses the higher layer's channel values to darken the corresponding channels of the lower layer — the brighter the higher layer's color in a channel, the more that channel is darkened on the lower layer. It's useful for tinting or dimming an effect using another effect as a control input, rather than for a hard replacement of color like Color Change.

### Luma Key

The Luma Key Mixer matches areas of the lower layer whose brightness falls within a configured range, and replaces just those areas with the higher layer's effect color. Areas outside the range are left untouched. The Configuration dialog lets you set the **Brightness Range** (lower and upper limits) used for the match.

### Chroma Key

The Chroma Key Mixer works like Luma Key, but matches on a specific color (hue and saturation) instead of only brightness, replacing matching areas of the lower layer with the higher layer's effect color. The Configuration dialog provides:

- **Color** — the key color to match against the lower layer.
- **Brightness Range** — lower and upper brightness limits the lower layer must fall within to be considered for a match.
- **Hue Tolerance** and **Saturation Tolerance** — how far a pixel's hue and saturation can differ from the key color and still be considered a match.
- **Treat Zero Brightness as Transparent** — when enabled, if the higher layer's effect is completely unlit, the lower layer is passed through unchanged instead of being evaluated for a match.

Chroma Key requires a mixing partner.
