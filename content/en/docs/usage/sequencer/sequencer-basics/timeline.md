---
title: Timeline
author: Vixen Team
weight: 25
description: This section covers the Timeline features.
---

### Overview

The Timeline is the heart of the sequence editor. It is divided up from left to right in minutes and seconds. Top to bottom in rows are the [Elements][1] you have defined in the [Display Setup][2]. These should correspond to the props in your display and may have [Groups][1] of props that you have organized. Any groups can be expanded to reveal the sub elements or other groups. The Timeline can be zoomed in or out to show as much or little of the time the sequence covers. There are keyboard and mouse shortcuts to control the zoom and allow panning from left to right and up and down. See the [Editor Shortcuts][3] section for more details on these commands.

### Time Ruler

The ruler along the top contains the hash marks for the time intervals. These will vary from minutes to seconds to milliseconds as you zoom in and out. You can also click here to place a caret as the starting place or drag and select a range for the sequence when playing. See [Playing Sequences][4] for more information on this feature. Marks can be added here to mark beats or other important parts of the sequence and can be used as alignment references. Hovering the mouse near the bottom of the ruler will transition the cursor to a horizontal bar that you can click and drag to resize the height of the ruller. The time numbers will scale in size relative to the height. Marks can be added via the ruler. See [Adding Marks][13].

### Mark Bar

Below the ruler is the Mark Bar. This area will only show up if you have [Marks][11] that have the [Mark Bar][12] enabled. Marks can be edited in this area to change their start time, duration, text and location. This works similar to how effects are managed. See [Editing Marks][14] for more details.

### Rows

As mentioned above the Timeline consists of rows of the elements organized in an expandable tree. This mirrors the tree created in the [Display Setup][2]. Clicking the plus icons in front of a group element will expand that row to reveal its children. Rows can be selected by clicking in the area where the element name is. You can use this to [Cut, Copy and Paste][10] entire rows of Effects.

The rows can have a highlight indicator showing if they have any effects on them, or any of their chidren have effects. Enabling the menu option **View -> Highlight Rows With Effects** will turn this feature on. The element names will be highlighted in yellow if that row has any effects on it. The plus expander icon will be outliend in yellow if any of the children have effects on them. With the combination of the two, you can quickly see where effects may be hiding.

You can resize the height of any row in the Timeline. In the element name section hover over the bottom border for any element. Then the horzontal cross cursor appears, you can click and drag the row to the height you want. There are also keyboard short cuts increase or decrease all the rows sizes together. They can be found under the menu options in **View** to zoom the rows in or out. To reset the row heights to the default click the option under **View -> Reset Row Height to Default**. The height settings are saved when you close the sequence editor and will be restored when returning. 

Rows can also be collapsed quickly by clicking the **View -> Collapse All Element Groups** option. This will return all the rows to the collapsed state. The expanded states of the rows are also saved from session to session.

### Effects

[Effects][5] can be added to the elements in multiple ways. You can drag the effect from the Effect list docker onto any place in the timeline. They can also be added from the context menu by right clicking in the place you wish to add it and then navigating to the effect and selecting the desired one. Effects are added with a default length of 2 seconds and default settings that are helpful to get you going. More control over how effects are added can be obtained by using the [Draw Mode][6] feature. Once an effect is on the timeline it can be edited in the Effect Editor docking widow by selecting it. See the [Effect Editor][7] section for details on editing effects.

Effects can be moved around on the timeline by simply clicking on them and dragging it to the desired location. The length can also be changed by dragging on the beginning or end of the effect. A tool tip will appear when resizing to show the start and duration of the effect. The same tool tip will appear when hovering over the effect. Multiple effects can be moved or resized at the same time by multi selecting them. This uses standard select means of Ctrl/Shift click as you would see in any modern windows app. Once you have multiples selected, they can be moved or resized as a group. See the section on [Alignment Helpers][8] and the [Draw Indicator][9] sections for further ways to manipulate effects in relation to each other.

Effects can also be [Cut, Copied and Pasted][10] from one place to another. Normal paradigms apply for this mechanism. Another way to make a quick copy of an effect is to Ctrl click and then drag on the effect. This will clone the selected effect(s) and allow you to quickly drag a copy of it else where. Holding the Shift key while dragging the effect will hold it at the time so you can drag it to another element and not change its position in time.

Each effect can have an info popup when the mouse is hovered over them. This provides information such as the name of the effect, the start and end time, the duration, and the layer the effect is in. This can be enabled or disabled under **View -> Show Effect Info** or with Ctrl+I.

### Marks

[Marks][11] will be shown on the timeline as vertical lines in the color and style of the collection they are part of. These can be very helpful in aligning effects to beats or other important features in a sequence.

### Timeline Shuttling

Movement up and down and right and left in the Timeline can be done with a mouse and scroll wheel. The mouse wheel will scroll up and down when hvered over the Timeline. Holding Shift while scrolling the mouse wheel will move left and right.  

Holding Ctrl while scrolling will zoom in and out the visible time span. Where the point of zoom occurs can be controlled by the option in the menu **View -> Zoom Under Mouse Position**. When selected the point of zoom will be where the mouse is. Otherwise it will be the center of the visible Timeline. Ctrl + and Ctrl - will also alow you to zoom with the keyboard.

### Persisted Settings

Many of the Timeline settings are saved with each sequence you edit. Thus when you return, the place on the Timeline will be restored along with expanded groups and row sizings to get you back sequencing as quickly as possible.

 [1]: {{< ref display-elements-groups>}}
 [2]: {{< ref display-element-basics>}}
 [3]: {{< ref editor-shortcut-keys>}}
 [4]: {{< ref playing-sequences>}}
 [5]: {{< ref effects>}}
 [6]: {{< ref draw-mode>}}
 [7]: {{< ref effect-editor>}}
 [8]: {{< ref alignment-helpers>}}
 [9]: {{< ref resize-draw-indicator>}}
 [10]: {{< ref "edit-functions#cut-copy-and-paste">}}
 [11]: {{< ref marks>}}
 [12]: {{< ref "marks#marks-bar">}}
 [13]: {{< ref "marks#adding-marks">}}
 [14]: {{< ref "marks#editing-marks">}}
