---
title: Setup and Configuration
date: 2017-01-05
weight: 10
---

### Display Configuration Concepts

When setting up a light display with Vixen, there are certain configuration steps that must be taken to tell the software what elements and output controllers you will be using. Vixen separates the elements you have in your physical display from the outputs and controllers you use to run your display. You can work all year designing and sequencing a display and setup your outputs as you setup your physical display.

### Elements

You can think of an element as an individually controlled item in your display. Examples of a single element is an incandescent or LED string of lights, multiple strings of lights you want to ALWAYS control as a single unit, a single node in an RGB pixel, or even a servo driven prop.

You’ll notice that we call a single pixel an element. In Vixen, all three colors are GROUPED into a single element based on filters (next section) so you can think of this RGB node as a single item. When you sequence this pixel later, you tell it you want it to be blue and it just is.

For a more in-depth discussion of Elements, see [Display Elements & Groups]({{< ref display-elements-groups.md>}}).

### Color Handling

Standard light strings (single color incandescent or LED strings, multi-color strings, etc.) are what Vixen calls “single color”. There are two ways to configure the color handling of these strings.

  1. **Single Color**: This is generically what Vixen calls a “standard” string of lights. A single string with all red lights or a single string with multi-colored lights are a both defined as a “single color” item.
  2. **Multiple Colors**: This selection is used when you have multiple light strings on a single prop in your display that are controlled separately. For example, a popular way to light mini-trees is to wrap them with red, green, blue and white strands of standard light strings but control each of the strings separately. This allows you to set the trees to any one of these colors (or some or all of the colors) at any time in your sequencing. In vixen, you define ONE ELEMENT and tell the software, by selecting this option, that this element is a set of multiple strings of lights. When sequencing, you select an effect and color (red fade for example) and just the red trees light automatically.

RGB strings are defined by choosing this filter. If you have a string of 50 RGB nodes, for example, you would select the string in the element tree and define the color handing as “Full RGB”. This tells each of the 50 nodes that there are 3 colors in EACH of the nodes (150 outputs total).

### Controllers

Controllers define single outputs to your physical display. So, for example, if you have an element that is a single color string of lights, this string would be linked to an individual controller. As another example, if you had defined a string with 50 RGB pixel nodes and defined their color handling as RGB, you would link each of these elements to 3 output channels. Your 50 pixel RGB string would be linked to 150 output channels.

For more information, see [Controllers]({{< ref controllers.md>}}).
