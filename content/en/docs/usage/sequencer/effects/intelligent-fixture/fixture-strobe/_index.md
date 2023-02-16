---
title: Fixture Strobe
author: Vixen Team
description: Fixture Strobe effect enables the strobe hardware support on the fixture and controls the strobe speed.
aliases: [/vixen-3-documentation/sequencer/effects/intelligent-fixture/fixture-strobe/]
---

---

### Overview

Fixture Strobe effect enables the strobe hardware support on the fixture and controls the strobe speed. 
The display preview will show a blinking beam when this effect is active but does not attempt to reflect the strobe speed which is hardware dependent.

---

### Configuration

* **Function** - The function on the intelligent fixture that controls the strobe (shutter).

* **Setting** - Index setting that controls how the strobe speed is interpreted.

* **Strobe Speed** - Controls the speed of the shutter's strobe.  The setting determines how this curve is interpreted by the hardware.

---

### Requirements 

For an intelligent fixture to support the Strobe effect it must have the following:

  1. Shutter function with the _Shutter_ tag.
  2. One or more Shutter index items with the Use Curve option and _Strobe_ tag.

---





