---
title: Basics
author: Jeff
date: 2017-09-14T01:01:08+00:00

---

![Wipe Settings Screen](/images/docs/usage/sequencer/effects/basic/wipe/Wipe_Properties-216x300.jpg)

The Wipe was one of the first location aware effects in Vixen. The goal of this effect is somewhat similar to the chase, however it is aware of the position of the elements as defined in the Preview. It uses this location awareness to simulate a chase across all of its elements in a Wiping fashion.

### Type

It can be controlled by the number of passes, by a measure of the pulse length and with a Movement curve. The most common use case is the by count.

The Wipe on/off options are similar to the [Chase]({{< ref "chase-basics">}}) extend to start/end options. These are most useful for wiping the stage on or off. The pulses have the same rules as the Chase and need to have a > zero end value for wiping on and a > zero start value for wiping off. The default pulse curve has a zero start and end value, so to use this you would need to adjust to a ramp on  for the wipe on case or ramp off for wipe off as an example.

### Direction

It can move in a number of directions, horizontal, vertical, diagonal up, diagonal down, burst, circle burst and diamond burst. Each direction can then be reversed.

### Color

The wipe supports the Color Gradient like most effects.

### Brightness

A Curve is used to control the brightness of the individual pulses. This behaves just like it does on a Pulse effect. Numerous pulses are used to make the wipe happen. This curve is what those pulses will look like.

### Pulse

The pulse length is also similar to the pulse overlap feature of the Chase and allows for the pulses to be adjusted to smooth out the Wipe or lengthen the amount of visible time any part of the lights are lit.
