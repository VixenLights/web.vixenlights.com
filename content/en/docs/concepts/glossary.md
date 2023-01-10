---
title: Glossary
author: Jon Chuchla
date: 2013-10-31T20:33:22+00:00
weight: 150
---
### Channel

The individually controllable outputs of a Controller.

### Controller

A module that defines an specific hardware device or set of devices. The controler setup contains channel configuration, communications protocol, and how it&#8217;s connected to the show computer.

### Curve

Intensity that changes over time.  This is usually used to refer to a brightness value for an effect.  The curve control shows brightness on the vertical Y axis and time on the horizontal X axis.  Time is a percentage of the duration of the effect.  It is not possible to define a curve in terms of absolute time, it is always relative to the effect duration.

### Effect

An action on an element or group. Effects range from simple set level to more advanced like twinkle and chase. Effects can overlap in the sequencer. Some elements may only work with certain element types, and some effects may require a group of elements to be effective.

### Element

The controllable display elements. These are the strings of lights or the individual pixels that make up your display. Examples of an element are: A candy cane controlled as one unit, or a minitree(RGB) or a string of lights. Elements can be grouped together for convienent manipulation (see Group)   The horizontal tracks in the Sequencer where you assign effects to a display element.   In the Preview, it is the element you see that responds to effects in the timeline.

### Filter

An object inserted into the path between an element, and a controller channel that modifies, splits, or combines the information in some way.

### Gradient

A gradient is a color that changes over time.  It consists of one or more colors that are positioned horizontally along a timeline.  Similar to a curve, the horizontal axis represents time, relative to the length of a given effect.

### Group

A logical grouping of elements. This helps to organize elements into groups that are likely to be worked with together. Within the sequencer, effects can be applied to either elements, or groups. A level effect applied to a group, will affect all elements in that group. Groups may contain other groups. There is no limit to how deep groups can be nested.

### Mark

A line in the sequencer that helps visualize certain notable timing points. Marks might be used to show the beat of the music, or to show other transition points in the song.

### Module

A portion of the application that performs a specific task. Vixen 3 is built with a modular architecture to allow easy adding of new functionality by 3rd parties.

### Output

Deprecated &#8211; we don&#8217;t talk about those anymore because it can mean too many things and just gets confusing!

### Patch

A logical connection between Elements, Filters, and Controller Channels. A patch controls how information from an Element is routed through various filters and ultimately reaches the actual device being controlled.

### Preview

The screen used as a virtual lighinting display. The preview allows you to play your sequence on virtualized hardware so you can see how it will look.

### Program

A list of sequences. Used in the scheduler.

### Property

Elements may be assigned properties to define additional information about the specific element. Certain effects may make use of these properties to perform special actions. Properties might be used to specify coordinates for image mapping or other future uses.

### Scheduler

The tool used for setting up what to play, and when to play it. This tool allows you to define programs (aka playlists) and a schedule defining when the programs will play.

### Sequence

A set of ordered actions and effects that will be performed on your Elements

### Timed Sequence

A sequence that follows a timeline. These are most often used with music. Effects are assigned to groups and elements that happen at a certain point in time.

### Sequencer

This is the tool that you use to create your timed sequence.

### Timeline

The section of the sequencer located above the element effect workspace. It shows the position in time where you are working.

### Treeview

Several configuration windows use a heirarchical view to show the oranizational relationship of groups and their members.

### Waveform

The graphical representation of an audio file in the sequencer. By visually looking at the waveform, you can see the loud and soft points of the song, as well as identify the beat.
