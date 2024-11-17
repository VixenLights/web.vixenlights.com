---
title: Inline Curve Editor
author: Vixen Team
description: This section covers the Inline Curve Editor features.
featured_image: /docs/usage/effect-editor/EffectEditor.png
---

### Overview

The Inline Curve Editor is a powerful tool that allows many features of the larger [Curve][1] editor dialog to be done inline in the effect editor. This improves efficency for the user since they do not have to keep opening and closing a bulky dialog box.

![Inline Curve Editor](/images/docs/usage/effect-editor/inline-curve-editor/InlineCurve-300x49.png)

### Editing Curves

* To add a node, hold the Control Key and Click the line where you want to add the node.
* To delete a node, hold the Alt Key and Click the node you wish to delete.
* To move a node, simply Click and Drag any node to the position you want. (The full editor provides more precision if needed)

### Shortcuts

* To flatten the curve into a horizontal line, hold the shift key and click anywhere in the curve control. Holding shift while dragging will allow you to position that horizontal flat line up and down. This function is intended to replace the functionality of the old simple sliders that have now been replaced with curves.
* To reverse the curve direction, (flip left to right) use Control+Shift while clicking the curve.
* To invert the curve (flip top to bottom), use Alt+Shift while clicking the curve.

### Drag and Drop

* Using the curve library, you can drag curves and drop them onto the curve in the effect editor. This works from the full library panel, or the toolbar. The opposite also works. You can drag the curve from the effect editor pane to the preset library or toolbar to add them to the library.
* You can drag a curve from the effect editor onto any other effect or selected effects on the timeline. If the effect has more than one curve, you will be prompted to choose which curve to replace.
* To invoke the full curve editor, simply double click on the black area of the curve control.
* When a curve is linked to a library curve, the line will be gray and a link icon will appear over the control.  

### Full Gradient Editor

* To invoke the full curve editor, simply double click on the curve in the effect editor.

A linked Curve denoted by the chain link in the upper left corner.
![Inline Curve Editor](/images/docs/usage/effect-editor/inline-curve-editor/LinkedInlineCurve-300x49.png)

You will not be able to edit the linked curve in the effect editor pane.  Double clicking the curve control will allow you to link or unlink library curve. Once it is unlinked, you can edit it in the inline editor or the larger Curve dialog.

[1]: {{< ref curves >}}
