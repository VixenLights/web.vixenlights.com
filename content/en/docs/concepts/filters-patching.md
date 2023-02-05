---
title: Filters and Patching
author: Vixen Team
weight: 50
---

### Overview

Patching is the idea used to tell Vixen how a element relates to an output. In a simple setup, a user might have 12 mini-trees, and a single Renard to control them. They might patch each mini-tree channel directly 1:1 to a corresponding output on the Renard. This is a simple use case, and is the equivalent to the way Vixen 2.x works: a direct 1:1 correlation between elements that the user sequences with and the outputs from the controller.

However, in a more complicated setup, there may not be 1:1 mappings. For example, say the user has a large tree that has been wrapped in 8 strings of lights, and they have each string on a different output on a controller. If they wanted to treat the tree as one single object (eg. not control each string individually), they can map the one "Tree" element to the 8 controller outputs that correspond to the strings.

### Filters

In this patching system we have also introduced the concept of 'filters' which can be inserted in the path from elements to controller outputs. Filters are intended to take data in, manipulate it in some way, and then output the data. For example, a simple filter might be a dimming curve. The Dimming Curve filter has a single input and a single output. It transforms the intensity value of any lighting data it gets according to a user-configured curve. It wouldn't affect the data in any other way, or doesn't distinguish between multiple pieces of data coming in: for example, if there are two lighting values that come in at the same time, it transforms them independently, then outputs the two lighting values.

A more complex filter might be the Color Breakdown filter. This can be configured to take any given lighting value, and split up the data based on the color component of the lighting value. It will then output the broken-down values on independent filter outputs. For example, a common example would be an RGB breakdown filter. The filter would be configured with 3 components: pure red, green and blue and when it gets a lighting value, it would split it up into the red part, green part, and blue part, and output those (component) lighting values on the 3 filter outputs.

Filters can also be stacked, so you could have a dimming curve (to adjust the intensity of all data), which then goes through a color breakdown filter to split it out suitable for a particular controller scheme.

Finally, there are other possibilities for filters that haven't yet been implemented: for example, some DMX systems might control a movable lighting fixture with a 16-bit value for a movement axis. However, since DMX is 8-bits per channel, it combines two for the full 16 bits. A filter might be created which takes in a generic "movement" data item, and splits it into a 16-bit value, but on two separate outputs (for the high 8 bits and the low 8 bits). These might then be patched to the appropriate DMX channel.

One current limitation of the patching/filtering system is that any component, filter or outputs, can only have a single source item. That is, you can't patch two different channels to a single output. This is scheduled to be changed, but is probably not that common a use case, so it may be a while until we get to it.
