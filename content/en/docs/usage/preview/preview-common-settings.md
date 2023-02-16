---
title: Common Settings
author: Vixen Team
weight: 20
description: This section covers the common settings used for Prop Shapes.
---

### Overview

There are various common settings that are available in most, if not all of the items you can include in your preview. These options are detailed in this section. When you select a shape in the preview display a properties page will appear on the bottom left side of the preview editor screen.

![Preview Toolbar](/images/docs/usage/preview/basic-shapes/line-properties.png)

### Position

All of the elements have various position properties that can be set. The individual meaning of each of these properties is detailed in the section of help for that item. Everything in the preview is defined by a location based on pixels.

The screen is in (X, Y) coordinates with the top, left pixel being defined as (1, 1). So, if a prop needed to be right 100 pixels and down 10 pixels, it's location would be (100, 10).

These position properties give you fine control over the exact location and size of the items on your screen. You can usually accomplish what you want with the mouse and by nudging the item with the arrow keys.

### String Type

This defines the type of string you want to use for this item. A **Standard** string type is one where the entire prop is linked to a single element. A **Pixel** string type is one that has each of it's lights liked to an individual element. There is nothing wrong with linking multiple lights in a pixel string to the same element.

### Standard String

What makes a Standard string **Standard** is that all of the lights in the string are addressed via a single element.

A Standard string is what most people think of when they think Christmas lights. It is a string of lights that is either a single color or is multi-colored. These lights are static so their color cannot be assigned by the software. The are either on, off, or are in some state in-between.

_There is one exception:_ A string of **Pixel** lights that are all controlled as a group and are not individually addressable is a Standard string too.

### Pixel String

What makes a Pixel string **Pixel** is that all of the lights in the string are addressed with individual elements.

### Light Size

The diameter of the light on the screen. Adjust this until the light size looks the way you want. The defaut size is 3, and bigger numbers provide a larger light diameter.

### Light Count

The number of lights in the string or prop. This is very important if you are defining an item with individually addressed pixels. If you are designing with standard strings, this number can be whatever you want to get the look you are going for. Some items, such as the rectangle, have multiple strings each with their own light count.

Increasing the light count in a a string will add lights to the end of the string. If the item is defined as a **Standard** string type, there is no more configuration necessary. If the item is defined as a **Pixel** string type, these newly added pixels will be unassigned. You will have to link them to an element.

Decreasing the light count removes pixels from the end of the string. There is a side effect of this. If you have a **Pixel** string type and remove 10 pixels and then re-add 10 pixels, you will lose any Element linking information you may have had defined.

### Linked Elements

When you want to see what your display will look like when you run a sequence, you need to have your preview items linked to elements. See the [Linking Elements][1] section for more information.

[1]: {{< ref preview-linking-elements>}} "Linking Elements"
