---
title: Basic Edit Functions
author: Jeff
date: 2016-11-20T04:14:54+00:00
weight: 10
---

### Cut, Copy, Paste ###

The cut, copy and paste features of the sequencer follow the well established patterns in the OS world. You can select any effect with the mouse and cut/copy it using the normal Ctrl C, Ctrl V and Ctrl X keyboard shortcuts or the right click mouse conventions. Selected effects will have a white dotted line around them whereas non selected ones will have a solid black outline.

Pasting works like it does in most all other applications. Standard keyboard and context menus are provided. To paste effects that are on the clipboard, select the row and time position in the timeline you want to paste and invoke the paste function. Effects will paste in the time and row spacing they were copied in. For example, if you copy effects from two side by side rows, they will be pasted at the new location in the side by side rows starting with the one you selected to paste to. If there are skip rows when it is copied, those same skips will occur during pasting. You can paste an entire row or rows of data copied from the row selection. They will paste at the entire row level. To copy an entire row, select the element name label and the enture row will be come selected. Use the keyboard shortcuts to copy or cut it. Then select the new row in the same manner and use the Ctrl V shortcut to to paste it. Effects can be copied between two open editors or even two open instances of Vixen.

### Copy / Paste with Layers ###

Layer information will be copied along with the effects if they are located in a layer. The same is true when copying between two sequences if the same layer exists in the target sequence. You must have the layer created in the target location for this to work.

### Effect Multi-Selection ###

Multi select of effects can be done by holding down the CTRL key while selecting the effects you want. You can select multiples in a range on the same row by clicking the first one to elect it and then SHIFT click one further before or after it in the row. All effects in between will be selected. You can click on the element name in the row and this will select the entire row. It will be outlined in blue and all effects will show selected.

Clicking the timeline and dragging the mouse with the left mouse button held will create a rectangular selection lasso that will select all effects inside or touching the lasso. You can also utilize the drag box filter by clicking the drag box icon in the toolbar to choose which effects the drag box will select. This will filter the selections to only those effects matching your criteria.

Additional capabilites for selection are provide by the Draw Mode. See the section on [Draw Modes]({{< ref draw-mode.md>}}) for further details.
