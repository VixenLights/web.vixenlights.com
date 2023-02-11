---
title: Custom Value
author: Vixen Team
description: Custom Value effect allows the sequencer to specify custom numerical value, string, or color (RGB) value to a display element at precise time(s) during a sequence.
---

---

### Overview

Custom Value effect allows the sequencer to specify a custom numerical value, string, or color (RGB) value to a display element at precise time(s) during a sequence.
This effect is often used to control external hardware when precise 8-bit values are needed by the connected hardware.

Previously this effect was the primary means to control DMX moving heads and other intelligent fixtures in Vixen.  Vixen now contains specialized 
[Intelligent Fixture Effects](/docs/usage/sequencer/effects/intelligent-fixture) to support DMX moving heads and other intelligent fixtures.


---

### Configuration

* **Data Type** - Selects the type of data to generate as the custom value.  
	* _8 Bit Value_
	* _16 Bit Value_
	* _32 Bit Value_
	* _64 Bit Value_
	* _Color Value_
	* _String Value_

* **Value** - Custom numeric value, string, or color (RGB) as determined by the **Data Type** property.


---





