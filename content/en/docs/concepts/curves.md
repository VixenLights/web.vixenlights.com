---
title: Curves
author: Jeff
date: 2014-08-13T02:03:00+00:00
weight: 40
---
The curve editor allows you to define how a parameter changes over time. The most common place you see curves is for intensity. The Pulse effect is a key example where this is used. To create a ramp effect, the curve will be a diagonal line from the lower left to the upper right. To create a ramp down, the curve is reversed. Additional points can be added to the curve to change how it acts. The points can be dragged to the proper place, or the actual values can be edited.

Curves can also be used for non-intensity parameters as well. One example of this is the movement curve in the Chase Effect. In this case, the curve defines the motion of the chase where the Y axis represents the chase position over the Z axis which is relative time.

Once you are happy with a custom curve, you can save it to a the library and link it to other effects so they can look the same. The curve library can be edited from within the effect editor or from the Tools menu in the main sequencer window.

Since the 3.4 releases the curves can now be edited directly in the effect editor without needing to launch the full dialog curve editor. Basic adjustments can be made here to quickly shape a curve. If needed final adjustments can then be made in the full dialog editor. See [Effect Editor]({{< ref "effect-editor">}}) 

![Inline Color/Gradient Editors](/images/docs/concepts/curves/InlineCurveEditor-300x262.png)

The full curve editor supports many features. There are buttons to reverse a curve, invert a curve, free hand draw and use a mathematical function to generate one. There are also key mouse combinations that allow a curve to be adjusted. Holding the Shift Key and click dragging a point on the line will convert it to a flat line curve. It can be freely moved up and down to any point on the graph. This mimics functionality in the inline curve editor.

![Inline Color/Gradient Editors](/images/docs/concepts/curves/DefaultDimmingCurve-220x300.png)

#### Curve Library

The Curve library can be accessed in several ways from the Sequence Editor.

  * Tools -> Curve Editor &#8211; This bring up a dialog window with the Curve library and allows new curves to be added and existing ones to be edited or deleted.
  * View -> Curve Library Window &#8211; This opens a docking window that can be placed in docked locations in the editor. This allows the same features as above, but you can also drag them out and drop them on effects. You can also import/export the library to share between profiles or others.
  * Toolbar &#8211; By right clicking in the toolbar you can add other toolbars such as the curve library. The toolbar has the same features as the docker window. The features can be accessed by right clicking on the toolbar to bring up the menu. 

![Inline Color/Gradient Editors](/images/docs/concepts/curves/CurveLibraryDialog-300x251.png)

![Inline Color/Gradient Editors](/images/docs/concepts/curves/CurveLibraryDocker-154x300.png)

![Inline Color/Gradient Editors](/images/docs/concepts/curves/CurveLibraryToolbar-300x50.png)
