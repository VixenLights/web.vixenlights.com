---
title: Fan
author: Vixen Team
description: The Line Dance Fan effect coordinates the pan of a group intelligent fixtures to make fan shape with the light beams.
---

---

### Overview

The Line Dance Fan effect coordinates the pan of a group intelligent fixtures to make fan shape with the light beams.
This effect pans pairs of intelligent fixtures.  The amount of pan increases from the center of the collection of fixtures.
The intelligent fixtures on both ends have the most pan.

This effect should be used with color effect like _Set Level_.
This effect also works well when the Tilt is modified with the _Set Position_ effect.

---

### Configuration

* **Fan Mode** - Selects the type of fan.
  * _Synchronized_ - All intelligent fixtures in the collection synchronously start their pan at the beginning of the effect and complete the pan at the end of the effect's duration.
  * _Staggered_ - The fan is performed by panning pairs of intelligent fixtures.  Starting with the center two fixtures and moving outward.  Generally only two fixtures are moving at any given time.
  * _Concurrent_ - All the intelligent fixtures start their pan at the start of the effect and finish based on the degrees of pan.

* **Pan Increment** - Controls the Pan angle increment between each fixture.  This curve or slider determines how much each pair of intelligent fixtures 
                      are panned.  The first pair are panned the increment.  The second pair are panned 2 times the increment.  The third pair are panned 3 times the increment and and so on.

* **Invert Pan** - Inverts the pan movement for the intelligent fixtures that are mounted upside down (inverted).

* **Center Handling** - Controls the pan of the center fixture when the effect is targeting an odd number of fixtures.
  * _Centered_ - The middle intelligent fixture is not panned. 
  * _Left_ - The middle intelligent fixture is panned left.
  * _Right_ - The middle intelligent fixture is panned right.

* **Advanced Overrides** - Display or hides advanced override settings.  These settings are generally not expected to be changed.

* **Pan Start** - Controls the initial pan of all the fixture participating in the fan.  The default is a pan of 360 degrees.

---

### Requirements

This effect requires 3 or more intelligent fixtures that support the Pan function with _Pan_ tag.
The effect requires that the intelligent fixtues can pan greater than 360 degrees.


---





