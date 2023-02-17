---
title: Text
author: Vixen Team
description: Creates an effect that displays text on the display element.
aliases: [/vixen-3-documentation/sequencer/effects/text/]
---

---

### Overview

Creates an effect that displays text on the display element.
The text can appear in any font. It can be static or moving.

---

### String Setup
    
  * **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      Locations is often referred to as whole house, but it can be any form of multiple props. 
                      Generally you want Strings when applying to one prop and locations if the target is multiple props.
  
  * **Orientation** - Controls the orientation of the display area (matrix).

---

### Configuration

* **Text Trigger** - Controls how the text is triggered to be displayed.
    * _None_ - Uses standard text with no trigger.
    * _Mark Collection_ - Uses marks to trigger when words are shown.
    * _Mark Collection - Labels_ - Uses marks to trigger when words are shown but addtionally uses the label on the mark as the text.

* **Direction** - The direction of the movement.

* **Iterations** - The number of times the pattern repeats over the duration of the effect.

* **Mark Collection** - Selects the Mark Collection to use to determine when words are displayed.
                        Switching the Text **Text Trigger** to _Mark Collections_ or _Mark Collection - Labels_ allows each word in the text string be displayed on each Mark.

* **Text Duration** - Adjust the way the duration is used between _Auto Fit_, _Mark duration_, and _User defined_.

* **Text Fade** - Fades the text choosing between _None, _In, _Out, _In/Out_.

* **Time Visible Length (ms)** - Shows each word for the selected period of time up until the next word.  Applies to **Text Duration** set to _User defined_.

* **Repeat Text** - When enabled will repeat the individual words if there are move Marks in the collection than the number of total words.

* **Direction Per Word** - When enabled will move the text based on **Direction** over the duration of each displayed word.

---

### Movement

* **Vertical Offset** - The vertical offset to help center text vertically on the grid.

* **Center Stop** - When enabled, causes the text to stop at the center of the grid and then disappear.

---

### Color

* **Text Color Gradients** - One or more colors or gradients to be applied to the text. One color will be applied to each line of text.

* **Cycle Color per Character** - Cycles through the color gradients for each character of the text.

* **Gradient Mode** - Specifies how gradients will be applied to the text. There are 8 combinations of direction and how it''s applied. 
The gradient can be applied across the letters of the text, or across the whole element group. 
If it is across the letters, the gradient will stay with the text. 
If it is across the element, it will appear that the text travels through the colors of the gradient.

* **Use Base Color** - If selected, allows you to select a background color to appear behind the text.

* **Base Color** - The color to use for the background.
   
---

### Text

* **Text Line(s)** - One or more lines of text to display.

* **Font** - Specifies the font, style and size to be used. You may use any font installed on the PC. Note that the fonts used must be installed on any PC where you will transfer this sequence.

* **Center Text** - Centers the text.

* **Text Layout** - The orientation of the letters. When _Normal_, the text appears normally. When set to _Stacked_, the letters are stacked vertically.

### Brightness

* **Intensity** - The overall brightness envelope for the text itself over the duration of the effect.

* **Base Color Intensity** - The overall brightness envelope for the background color over the duration of the effect.

#### Video Tutorial

{{< video src="/images/docs/usage/sequencer/effects/pixel/text/Text.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}

{{< youtube Vo4AI6vNi-0>}}
