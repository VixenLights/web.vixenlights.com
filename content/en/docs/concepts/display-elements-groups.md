---
title: Display Elements and Groups
author: Jeff
date: 2013-04-28T16:22:24+00:00
weight: 10
---
Elements are the new concept in Vixen 3. The purpose is to be able to model how a display is set up, and not be concerned with the physical realities of the hardware, controllers, channel numbers, etc. To assist in this, elements can be nested into groups to associate common elements. These groups are critical for some of the advanced sequencing tools, later on.

For example, a Megatree item in a display might be defined as a group called *Megatree*, with 16 elements inside it: *Megatree-1* through to *Megatree-16* that represent the 16 strings of lights around the tree. If those strings are pixels, then there might be 50 other elements nested within each string that represent each pixel. Or, a display might have multiple shrubs/bushes around a garden: 4 on the left, 8 in the middle, and 4 on the right. A user might decide to group each set of shrubs into one group (eg. *Shrubs-Left*, *Shrubs-Middle*, *Shrubs-Right*), and then group those 3 into another group called *Shrubs*. This allows effects to be used on all shrubs or just one area very easily. The idea is to apply effects at the highest level items that represent things we know, not the elements of the physical lights.

Elements and groups also have the ability for extra *Properties* to be defined and configured for each element or group. The intent of a Property is to give the user some way to provide extra information about that element in the display. This information will be used by the effects in the sequences. A color handling property can be used to restrict effects on that element to a certain range of colors. Or, a Position property, can represent the position of elements in their display. Some of these are configured by the user on setup, and others get created as part of another setup process. The Position properties are generally set automatically by the preview when it is configured and based on the location of elements in relation to each other.

The general intent for the development and creation of elements is that it should represent or model something in your display. (e.g. an item, or fixture, or prop) If you have elements that you#8217;re naming things like *Renard-37*, *Channel-21*, *Tree-1-Red lights*, then you're probably going about it the wrong way.

Elements are the entry point for data into the Vixen system. For example, when sequencing a song, the user would sequence data against the elements and groups in their configuration. When playing back the sequence, the effect is applied to one or a group of elements and then it is processed through to the to the appropriate controller in a way that abstracts the details from the user.
