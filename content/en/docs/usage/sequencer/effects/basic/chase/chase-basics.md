---
title: Basics
linkTitle: Basics
author: Jeff
---
The **Chase** Effect allows you to have a series of Pulse effects spaced out across the duration of the effect. Instead of having to place and distribute individual pulses over time, this effect will do the math to distribute them evenly for you.

The effect has several options:

### Behavior (3.6u1+)

There are two types of behaviors. Across Elements/Groups is the default behavior and is equivalent to how the effect acted prior to 3.6u1.

Each Element/Group is a new behavior that changes how the effect looks at the elements and targets them. Previously you could use the levels and chase across a group of Arches or similar props, but if you wanted to apply the same chase to each Arch in the group, you would need to put a Chase on each Arch specifically. Now you can choose the Each Element/Group behavior and the proper level to get an identical Chase on each arch. This also allows the possibility to Chase up/down a Pixel tree instead of just around it. Many combinations are possible using variations of the Behavior and Level options.

### Color Handling

This is how the colors are applied on the effect. The simplest is a single color which will create a simple chase with only that color on it. The other three options allow for a color gradient to be applied in different ways on the effect.

Gradient though the effect will transition the colors on the chase over time to match the colors in the gradient. This allows you to have  a chase that goes from say red to blue over the duration.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/GradientThruEffect-300x38.png)

The gradient per pulse means that each individual pulse within the chase will have the gradient applied to it. Each pulse will have the same color. So the pulse can go from red to blue.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/GradientPerPulse-300x41.png)

Gradient across items means that the gradient will be applied proportionately over group of items that the chase covers with each item receiving the color within the gradient that corresponds to it&#8217;s percentage of the entire group.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/GradientAcrossItems-300x38.png)

### Pulse Intensity

This setting controls the shape of the pulse. Much like the same setting in the pulse effect, you can control is each pulse ramps up or down or any shape you can design. The default setting represents a ramping on motion where each portion of the chase rams up to full brightness.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/PulseIntensityRamp-300x21.png)

### Pulse ramps up then down

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/PulseIntensityRampUpDown-300x23.png)

### Direction

This controls the direction the chase moves across items. In it&#8217;s simple form it is right to left, or left or right. But you can design custom movements to have is say move right and then back left in the same effect.

Normal Direction

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/DirectionNormal-300x26.png)

Reversing Direction

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/DirectionBothWays-300x25.png)

### Pulse

These setting control aspects of the pulses behavior. Extend to end or start keep the pulse on after it completes allowing you do have a chase that moves across turning everything on, or off.

Extend to end. Pulse Intensity must be above zero on the curve at the end.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/ExtendToEnd-300x20.png)

Extend to start. Pulse Intensity must be > 0 at the beginning of the curve.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/ExtendToStart-300x21.png)

The pulse overlap controls how much the pulses of the chase overlap with each other. This can be used to create a more smooth flowing effect by adding more overlap.

Zero overlap

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/DirectionNormal-300x26.png)

200 ms overlap

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/PulseOverlap-300x33.png)

### Levels Deep

This setting controls at what level the chase is applied inside a group of elements. So you can have 8 items and then have 4 of them grouped to the left and 4 grouped to the right. All of these are grouped under on group. By placing the chase at the top level group, you can chase all 8 of the items or the left and the right group as a pair.

![Gradient Through The Effect](/images/docs/usage/sequencer/effects/basic/chase/PulseOverlap-300x33.png)
