---
title: Intelligent Fixture
author: Vixen Team
description: This section covers using the Intelligent Fixture Smart object.
aliases: ['/vixen-3-documentation/preview/adding-items-to-the-preview/smart-objects/intelligent-fixture']
---

### Overview

Intelligent Fixtures are only supported in the OpenGL Preview due to performance and the need for 3D rendering capability.

There are two ways of adding an intelligent fixture to the preview.  If the intelligent fixtures have already been created in the Display Setup then perform the following steps:

  1. Select the fixture in the **Elements** tree.
  2. Select the Intelligent Fixture button on the toolbar.
  3. Click on the preview and drag to add the intelligent fixture.

If the intelligent fixtures do not exist in the Display Setup perform the following steps:

1. Click on the preview and drag to add the intelligent fixture.

2. Follow the steps on the Intelligent Fixture Wizard to create the intelligent fixture(s).

Once the Intelligent Fixture graphics have been created the following Intelligent Fixture Properties may be adjusted.  Select the fixture by clicking on it in the Preview area.

### Beam Properties

* **Beam Length** - Percentage of the background height.  If a background image is not being used then the beam length is the percentage of the height of the preview window.  Note percentages greater than 100 are allowed.

* **Beam Transparency** - Transparency of the light beam. 0% is completely opaque.  100% is completely transparent.  Note at 100% transparency the beam is not visible. 

* **Beam Width Multiplier** - Determines the beam width at the top of the beam.  The multiplier is multiplied times the base width to determine the top width.

### Color Wheel Properties

* **Color Wheel Rotation Speed Maximum (s)** - The time in seconds it takes the color wheel to make a complete rotation when configured to the fastest setting.

* **Color Wheel Rotation Speed Minimum (s)** - The time in seconds it takes the color wheel to make a complete rotation when configured to the slowest setting.

### Pan Properties

* **Invert Pan Direction** - Changes the start point of the pan by 180 degrees and inverts the direction of movement.  This setting is often used with **Top** (upside down) mounting position.

* **Maximum Pan Travel Time (s)** - The time in seconds it takes the fixture to travel from the start position to the stop position.

* **Pan Start Position (Degrees)** - Defines the resting position of the fixture.  This value helps ensure the Preview matches the movement of the actual hardware.

* **Pan Stop Position (Degrees)** - The stop position defines the maximum range of movement.  This value helps ensure the Preview matches the movement of the actual hardware.

### Position Properties

The following cooordinate properties define a rectangle determing the preview drawing area for the Intelligent Fixture.

* **Bottom Left** - Bottom left coordinate of the drawing area.

* **Bottom Right** - Bottom right coordinate of the drawing area.

* **Top Left** -Top left coordinate of the drawing area.

* **Top Right** - Top right coordinate of the drawing area.

### Settings

* **Linked Element** - Determines the Intelligent Fixture element the graphic is linked to.  Selecting the **...** button allows you to pick an Intelligent Fixture element. 

* **Mounting Position** - Selects the mounting position of the fixture.  This property allows for simulating the fixture being mounted upside down.

* **Name** - Name of the intelligent fixture.

* **Show Legend** - When true enables a legend that will show a function label and the corresponding channel value.  The legend can be used to debug problems and to provide feedback for functions that are not directly supported by the preview. The legend is only applicable to index and range functions that were populated with a Preview Legend character.

* **Zoom Narrow To Wide** - Indicates whether the fixture zooms from a narrow beam to a wide beam or vice-versa.

### Strobe Properties

* **Maximum Strobe Duration** - Determines the maximum amount of time an intelligent fixture's beam will be active in the preview when it's shutter is in strobe mode.
This time may be reduced depending on the strobe interval time such that the beam is ON (active) for 25% of the interval.
This property should be configured to allow the preview to simulate the actual strobe duration of the physical hardware.

* **Strobe Rate Maximum (Hz)** - Defines the maximum rate in Hz at which the intelligent fixture should strobe in the preview.
This property should be configured to allow the preview to simulate the actual strobe rate of the physical hardware.

* **Strobe Rate Minimum (Hz)** - Defines the minimum rate in Hz at which the intelligent fixture should strobe in the preview.
This property should be configured to allow the preview to simulate the actual strobe rate of the physical hardware.


### Tilt Properties

* **Invert Tilt Direction** - Swaps the start position with the stop position and inverts the direction of movement.  This setting is often used with **Top** (upside down) mounting position.

* **Maximum Tilt Travel Time (s)** - The time in seconds it takes the fixture to travel from the start position to the stop position.

* **Tilt Start Position (Degrees)** - Defines the resting position of the fixture.   This value helps ensure the Preview matches the movement of the actual hardware.

* **Tilt Stop Position (Degrees)** - Defines the maximum range of tilt movement.  This value helps ensure the Preview matches the movement of the actual hardware.

### Video Tutorial

{{< youtube 3wQTXoXmWCY>}}
