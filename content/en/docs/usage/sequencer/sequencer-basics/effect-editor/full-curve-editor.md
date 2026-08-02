---
title: Full Curve Editor
author: Vixen Team
description: This section covers the Full Curve Editor features.
---

## Overview

The Full Curve Editor is a dedicated dialog for building and fine-tuning a curve with more precision than the [Inline Curve Editor][1] allows. It opens when you double click a curve control in the Effect Editor.

## Editing Curves

* To add a point, hold the Control Key and click on the grid where you want the new point.
* To delete a point, hold the Alt Key and click the point you wish to delete. A curve must always keep at least two points, so the last two can't be removed.
* To move a point, simply click and drag it to a new position.
* To move the entire curve up or down while keeping its shape, click and drag anywhere on the grid that isn't on a point.

## Shortcuts

* To flatten the curve into a horizontal line, hold the Shift key and click-drag anywhere on the grid. The flat line will follow your mouse up and down.
* To reverse the curve direction (flip left to right), use Alt+Shift while clicking the curve, or click the **Reverse Curve** button.
* To invert the curve (flip top to bottom), use Control+Shift while clicking the curve, or click the **Invert Curve** button.

## Precise Point Entry

Clicking or dragging a point selects it and shows its coordinates in the **X:** and **Y:** boxes below the grid. You can type exact values into these boxes and click **Update** to move the selected point to that precise location, which is useful when you need an exact number instead of an approximate mouse position.

## Draw and Generate

* **Draw Curve** lets you free-hand a brand new curve. Click the button, then click and drag the left mouse button from the left side of the grid to the right side to sketch the shape. The **Draw Interval** setting controls the minimum horizontal distance between the points that get recorded while you draw; a larger interval creates a smoother curve with fewer points.
* **f(x) Curve** opens a function generator where you can type a mathematical expression to generate the curve. The expression is evaluated for `x` from 0 to 100 (at the Draw Interval step size) and the result becomes the curve's Y value at that point. `Pi` is available as a constant. For example, `Sin(2 * Pi * (x / 100)) * 50 + 50` produces one full sine wave across the curve.

## Library

The Library section lets you save, load, and manage curves independently of any one effect:

* **Save Curve** saves the curve currently shown in the editor to the library under a name you choose.
* **Load Curve** opens the curve library so you can pick an existing curve and link the editor's curve to it.
* When a curve is linked to a library curve, it's shown in gray and can't be edited directly in this dialog.
* **Edit Library Curve** opens the linked library curve itself for editing; changes apply everywhere that curve is used.
* **Unlink Curve** breaks the link to the library curve, leaving you with an independent copy you can edit freely.

[1]: {{< ref inline-curve-editor>}}
