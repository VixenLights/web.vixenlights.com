---
title: Alignment Helpers
author: Vixen Team
weight: 60
description: This section covers the Alignment Helpers for aligning effects.
---

### Overview

Alignment Helpers allow you to quickly align effects in a number of ways.

Unless specifically noted, the reference effect is the effect that you right click on  
to access the context menu or selection based if you use the keyboard shortcuts.

To access the Alignment Helpers, you will need to have a minimum of two effects selected,  
then right click the effect you wish to use as a reference, then Navigate to the Alignment menu item,  
this will give you a sub menu of the alignment helpers available.

### Align Start Times

This helper allows you to align the start time of multiple effects in one quick action.

By default, when you align start times, the end time of the effects are not changed, thus increasing, or decreasing the duration of the effect. The shortcut for this is to press the S key while the mouse pointer is over the selected effect to use as the reference.

To prevent the duration from changing, hold the shift key while clicking this helper.  
This will move the start time of the selected effects to match the start time of the reference  
effect, and will not change the duration of the selected effects.

In the event that one of the selected effects end time is before the start time of the reference  
effect, that effect will be moved to match the start time, and the duration will be held.

### Align End Times

This helper allows you to align the end time of multiple effects in one quick action.

By default, when you align end times, the start time of the effects are not changed, thus increasing, or decreasing the duration of the effect. The E key is the shortcut while hovering over the reference effect.

To prevent the duration from changing, hold the shift key while clicking this helper.  
This will move the start end time of the selected effects to math the end time of the reference  
effect, and will not change the duration of the selected effects.

In the event that one of the selected effects start time is after the end time of the reference  
effect, that effect will be moved to math the end time, and the duration will be held.

### Align Both Times

This helper allows you to quickly align effects, with matching start and end times. Use the B key as a shortcut while hovering over the reference effect.

### Align Center Points

This helper aligns the center of all selected effects to the reference effect.

### Match Duration

This helper allows you to match the duration of selected effects, to that of the reference effect.

By default, the end time of the effect is changed to match duration.  
Hold the shift key while clicking this helper to change the start time to match duration.

### Align Start to End

This helper allows you to align the start time of selected effects to the end time of the reference effect.

At this time the duration of the effect is held, there is no modifier key to maintain the effects end time.

### Align End to Start

This helper allows you to align the end time of selected effects to the start time of the reference effect.

At this time the duration of the effect is held, there is no modifier key to maintain the effects start time.

### Distribute Equally

This helper distributes a number of selected effects over a period of time, determined by the starting time of the top most  
selected effect, and the end time of the bottom most selected effect.

This total amout of time is determined by subtracting the starting time from the end time. The result of that calculation  
is divided by the number of selected effects which results in the duration to be used for the selected effects.

The effects are then aligned Start to End, in a stair stepped pattern.

### Distribute Effects (Dialog)

This helper is an advanced version of the Distribute Equally helper, you will be presented with a dialog window, which allows you full control over the distribution of the selected effects.

The options for this helper are:

* Time Control
  * Start Time
  * End Time
* Duration Control
  * Equal Duration
  * Do Not Change Duration
  * Specified Duration
* Placement Control
  * Stair Stepped
  * Overlapped
  * Spaced
* Starting Point
  * First
  * Last

![Distribute Effects Dialog](/images/docs/usage/sequencer/sequencer-basics/alignment-helpers/distribute-effects.png)

### Mark Alignment

Effects can be aligned to marks using the mark alignment functions.

#### Align Start to Nearest Mark

To align the start of the effect to a mark, select the effect(s) and then right click and click Alignment-> Align End to Nearest Mark or use the CTRL + SHIFT + S shortcut while hovering over the selected effect.

#### Align End to Nearest Mark

To align the end of the effect to a mark, select the effect(s) and then right click and click Alignment-> Align End to Nearest Mark or use the CTRL + SHIFT + E shortcut while hovering over the selected effect.

#### Align Both to Nearest Mark

To align the both ends of the effect to a mark, select the effect(s) and then right click and click Alignment-> Align Both to Nearest Mark or use the CTRL + SHIFT + B shortcut while hovering over the selected effect.
