---
title: Layers
date: 2017-01-05
weight: 40
description: This section covers the layering features when creating effects.
---

The 3.3 release brings support for layers. Layers are defined at the sequence level and effects belong to a layer. By default a new sequence has one layer called Default and this serves to act the same as things have been in previous releases. Older sequences opening in the 3.3 release will have the default layer and all effects will belong to that layer.

Layers are combined from the highest to the lowest by definable mixers. Each layer you create can have it's own mixer chosen from the available mixers. Each mixer defines how colors will combine between layers.

To assign an effect to a layer, right click on it in the timeline and navigate to the Layer menu. From there a list of the layer names will appear and you can select the layer to associate the effect to. The menu also will have a check next tot he layer the effect is currently associated with. Hovering over the effect will show a tooltip with effect information. In this tooltip will show the layer the effect is currently associated with.

New effects added to the timeline will be in the Default layer automatically. Copy and pasting effects will retain the layer of the original effect.
