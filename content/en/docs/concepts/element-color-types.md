---
title: Element Color Types
author: Vixen Team
weight: 30
---

### Overview

It's a common misconception that Vixen 3 is for RGB (Pixel) lights.  It is true that it's very easy to sequence RGB lights in Vixen 3, but it's also a great sequencer for standard Christmas lights as well.  When creating your elements, you'll need to define what kind of lights that element consists of.  If you don't configure the Color Handling, which creates the color properties, that element is assumed to be full RGB.  The different types of lights are as follows:

### Single Color (Discrete Color)

A single color string is usually a traditional strand of single color Christmas lights.  It could also be a floodlight, or other special light that can only be one color.  When configuring the Color handling for an element, you'll need to choose what color that light actually is.

When creating effects for a single color element, you will only be able to choose the one specific color that you've defined for this element.  They will be shown in the timeline in this color.  They will also appear in this color in the preview. Generally the Basic Effects category will be the effects used on these types of elements.

### Multiple Independent Colors (Discrete colors)

This is a way to use multiple single color channels as one element.  This is commonly used for mini-trees or super strings made from multiple strands of single color lights where each colored string is plugged into a different controller channel.  If you have an element that consists of a string of red lights, a string of green lights, and a string of white lights, this is the appropriate option to choose.  This differs from RGB in that the colors don't actually mix.  If you turn on red and green, you wouldn't see yellow, you would see red and green.  When choosing this option, you'll need to define what colors the individual lights are for this element.

Whenever you are selecting colors for basic effects on an element defined as multiple independent colors, you will only be able to choose the colors that this device supports.  You may chose more than one color at a time.  You will see the effect in the timeline with the separate colors you chose, they will not appear as mixed colors.  In the preview, these elements will appear as separate side by side strings for each color. Generally the Basic Effects category will be the effects used on these types of elements.

### RGB (Full Color)

This is used for a light that has multiple color components which mix to form secondary colors.  This can be pixels, *dumb RGB* strings, RGB floodlights or similar devices.  An RGB device is a full color-mixing device.  Unlike the discrete color option, if you turn on the red and green channel, you will see yellow.

When selecting colors for effects on RGB type elements, you will be able to choose any color and it will be shown in the timeline as that color.  These elements will render in full color in the preview. This opens the door to the Pixel Categories of effects.
