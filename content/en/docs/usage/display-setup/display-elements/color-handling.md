---
title: Color Handling
author: Vixen Team
weight: 40
---

### Color Handling

Color handling provides information on how the elements use color. There are 3 common types of lights.

1. Traditional analog incandesent, or LED string lights. These have been around for a long time and are typically a string of single color lights.
2. Dumb Pixels. These are LED pixels, but the whole string color can be controlled and will all be the same color at the same time. They lights are not individually addressable.
3. Pixels. These are modern addressable string of lights that can be made any color and each light can be any color.

The color configuration can occur from multiple places. If you add elements in display setup using the templates, the color setup will typically be presented as part of the setup workflow for each type of prop. If you create individual elements outside of one of the wizards, then it will be presented when you use the Add Properties -> Color Handling.

### Color Configuration

![Color Configuration](/images/docs/usage/display-setup/display-elements/color-configuration.png)

The Color Configuration dialog will be presented from multiple places. It is key to getting the color setup correct on your elements so the sequencer can properly manage them. There are 3 options on this dialog and they relate to the information above on what type of lights you are using.

1. Single color. This is for traditional lights where the element is a single color only.
2. Multiple colors that do not mix. This is for waht is known as super strings of traditional lights. A single prop may have multiple strings of different color lights covering the same area. You would configure this to have the set of colors that match what your strings are.
3. Mixing color types. This is typical of a pixel that can be any color. Typically they are RGB.
