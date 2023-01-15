---
title: Intelligent Fixture
author: John Baur
alias: /vixen-3-documentation/preview/adding-items-to-the-preview/smart-objects/intelligent-fixture
---

Intelligent Fixtures are only supported in the OpenGL Preview due to performance and the need for 3D rendering capability.

There are two ways of adding an intelligent fixture to the preview.  If the intelligent fixtures have already been created in the Display Setup then perform the following steps:

  1. Select the fixture in the **Elements** tree.
  2. Select the Intelligent Fixture button on the toolbar.
  3. Click on the preview and drag to add the intelligent fixture.

If the intelligent fixtures do not exist in the Display Setup perform the following steps:

1. Click on the preview and drag to add the intelligent fixture.

2. Follow the steps on the Intelligent Fixture Wizard to create the intelligent fixture(s).

Once the Intelligent Fixture graphics have been created the following Intelligent Fixture Properties may be adjusted.  Select the fixture by clicking on it in the Preview area.

### Beam Length  

Beam length is the percentage of the background height.  If a background image is not being used then the beam length is the percentage of the height of the preview window.  Note percentages greater than 100 are allowed.

### Beam Transparency

Determines the transparency of the light beam. 0% is completely opaque.  100% is completely transparent.  Note at 100% transparency the beam is not visible. 

### Beam Width Multiplier

Determines the beam width at the top of the beam.  The multiplier is multiplied times the base width to determine the top width.

### Invert Pan Direction

Changes the start point of the pan by 180 degrees and inverts the direction of movement.  This setting is often used with **Top** (upside down) mounting position.

### Invert Tilt Direction

Swaps the start position with the stop position and inverts the direction of movement.  This setting is often used with **Top** (upside down) mounting position.

### Linked Element

Determines the Intelligent Fixture element the graphic is linked to.  Selecting the **...** button allows you to pick an Intelligent Fixture element. 

### Mounting Position

Selects the mounting position of the fixture.  This property allows for simulating the fixture being mounted upside down.

### Name

Name of the intelligent fixture.

### Pan Start Position (Degrees)

Defines the resting position of the fixture.  This value helps ensure the Preview matches the movement of the actual hardware.

### Pan Stop Position (Degrees)

Defines the resting position of the fixture. The stop position defines the maximum range of movement.  This value helps ensure the Preview matches the movement of the actual hardware.

### Show Legend

When true enables a legend that will show a function label and the corresponding channel value.  The legend can be used to debug problems and to provide feedback for functions that are not directly supported by the preview. The legend is only applicable to index and range functions that were populated with a Preview Legend character.

### Tilt Start Position (Degrees)

Defines the resting position of the fixture.   This value helps ensure the Preview matches the movement of the actual hardware.

### Tilt Stop Position (Degrees)

Defines the maximum range of movement.  This value helps ensure the Preview matches the movement of the actual hardware.

### Zoom Narrow to Wide

Indicates whether the fixture zooms from a narrow beam to a wide beam or vice-versa.

### Video Tutorial

{{< youtube 3wQTXoXmWCY>}}
