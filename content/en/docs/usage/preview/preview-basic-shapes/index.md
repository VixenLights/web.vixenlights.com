---
title: Basic Drawing
author: Vixen Team
weight: 30
description: This section covers the Basic Shapes used for Props.
aliases: [/vixen-3-documentation/preview/adding-items-to-the-preview/basic-shapes/]
---

## Overview

The notion of how Props are represented in the Preview is denoted by Shapes. All Props have a Shape and there are 3 distinct types. The first are the Basic Drawing types. These are simple in nature, but can represent a wide variety of items effectively. These are selected from the Basic Drawing area in the toolbar.

### Point

Use the ![Point button](pencil.png) button that looks like a pencil. A point is a single light point on the screen. By setting the Light Size property, you can use this light to define spots, floods or other larger light areas on your scene.

### Light String

Use the ![Light String button](draw-line.png) button. A light string is a single, straight line of lights. This can be **Standard** or **Pixel** strings.

Light strings are defined by two points, Point1 and Point2 which are located on either end of the string.

### Rectangle

Use the ![Rectangle button](draw-rectangle.png) button. A rectangle is basically four strings of lights that are attached at each corner. Once the rectangle is placed, each corner can be individually moved so that it no longer keeps its rectangular shape.

To maintain a rectangular shape when adjusting its size, hold down the Ctrl key while moving the bottom, right corner.

### Ellipse

Use the ![Ellipse button](draw-ellipse.png) button. An ellipse is a single string of lights. It can be defined as a standard string of lights or a pixel string.

Ellipses are defined by two points, the top left point and the bottom right point. To adjust the size of the shape, click on one of the corners and drag it to a new size.

The first pixel of an ellipse is the right-most point. Pixels are in order clockwise from this point.

### Triangle

Use the ![Triangle button](draw-triangle.png) button. A triangle is composed of three strings of lights.

Hold Ctrl while resizing the shape to maintain the triangle as an isosceles triangle.

### Multi String

The Multi String is used to draw more complex light strings that are not just in a single straight line. They contain multiple points and line segments that join those points together. They can be **Standard** or **Pixel** strings. This can be used for rooflines and other shapes that change directions. You click to start the string and then hover the string out to the location it should change directions. Click again and the segment will hold and you can hover to the next location to click and set that segment. Once you are done, use the ESC key to end the drawing.

### Linked Elements

Like every shape in the Preview, Basic Shapes have a Linked Elements property to assign the elements that drive them. See [Linking Elements][1] for more information.

[1]: {{< ref preview-linking-elements>}} "Linking Elements"
