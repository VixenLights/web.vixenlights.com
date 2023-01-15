---
title: Basic Shapes
author: Vixen Team
weight: 30
alias: /vixen-3-documentation/preview/adding-items-to-the-preview/basic-shapes/
---
### Shape Properties

All of the basic shapes in Vixen share similar properties.

When you select a shape in the preview display a properties page will appear on the bottom left side of the preview editor screen.

![Preview Toolbar](/images/docs/usage/preview/basic-shapes/line-properties.png)

### Position

The position of each item is defined by various X and Y coordinates. Each item has different XY coordinates that can be set, for example, a line is defined by two points (labeled Point1 and Point2) in the image above. These can be set manually set in the properties sheet, set via dragging the selection boxes around the item in the preview window or by using the arrow keys after the item is selected.

### Light Count

This defines the number of lights in the item. Some items, such as the rectangle, have multiple strings each with their own light count.

Increasing the light count in a a string will add lights to the end of the string. If the item is defined as a **Standard** string type, there is no more configuration necessary. If the item is defined as a **Pixel** string type, these newly added pixels will be unassigned. You will have to link them to an element.

Decreasing the light count removes pixels from the end of the string. There is a side effect of this. If you have a **Pixel** string type and remove 10 pixels and then re-add 10 pixels, you will lose any Element linking information you may have had defined.

### Light Size

The diameter of the light on the screen. Adjust this until the light size looks the way you want. The defaut size is 3, and bigger numbers provide a larger light diameter.

### String Type

This defines the type of string you want to use for this item. A **Standard** string type is one where the entire prop is linked to a single element. A **Pixel** string type is one that has each of it's lights liked to an individual element. There is nothing wrong with linking multiple lights in a pixel string to the same element.

### Linked Elements

This is where you tell the preview what elements each item and pixel should respond to. Every item on the preview is linked to an element or, in the case of pixels, elements.

For more on linking elements, look at the [Linking Elements][1] section.

### Point

Use the button that looks like a pencil. A point is a single light point on the screen. By setting the Light Size property, you can use this light to define spots, floods or other larger light areas on your scene.

### Light String

A light string is a single, straight line of lights. This can be **Standard** or **Pixel** strings.

Light strings are defined by two points, Point1 and Point2 which are located on either end of the string.

### Rectangle

A rectangle is basically four strings of lights that are attached at each corner. Once the rectangle is placed, each corner can be individually moved so that it no longer keeps its rectangular shape.

To maintain a rectangular shape when adjusting it's size, hold down the Ctrl key while moving the bottom, right corner.

### Ellipse

An ellipse is a single string of lights. It can be defined as a standard string of lights or a pixel string.

Ellipses are defined by two points, the top left point and the bottom right point. To adjust the size of the shape, click on one of the corners and drag it to a new size.

The first pixel of an ellipse is the right-most point. Pixels are in order clockwise from this point.

### Triangle

A triangle is composed of three strings of lights.

Hold Ctrl while resizing the shape to maintain the triangle as an isosceles triangle.

### Multi String

The Multi String is used to draw more complex light strings that are not just in a single straight line. They contan multiple points and line segments that join those points together. They can be **Standard** or **Pixel** strings. This can be used for rooflines and other shapes that change directions. You click to start the string and then hover the string out to the location it should change directions. Click again and the segment will hold and you can hover to the next location to click and set that segment. Once you are done, usethe ESC key to end the drawing.

 [1]: http://www.vixenlights.com/vixen-3-documentation/preview/how-to/linking-elements/ "Linking Elements"
