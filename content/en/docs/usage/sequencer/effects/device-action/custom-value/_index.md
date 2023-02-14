---
title: Custom Value
author: Vixen Team
description: Custom Value effect allows the sequencer to specify custom numerical value, string, or color (RGB) value to a display element at precise time(s) during a sequence.
---

---

### Overview

Custom Value effect allows the sequencer to specify a custom numerical value, string, or color (RGB) value for an element at precise time(s) during a sequence.
The Custom Value effect is a special purpose effect intended primarily for testing and debugging of the Vixen application itself.
It is used to generate data of specific types to test downstream modules in the application.  This effect is not usually used for sequencing purposes.

Previously this effect was used to control special features of DMX moving heads and other intelligent fixtures.
Vixen now contains specialized [Intelligent Fixture Effects](/docs/usage/sequencer/effects/intelligent-fixture) to support controlling DMX moving heads and other intelligent fixtures.

---

### Configuration

* **Data Type** - Selects the type of data to generate as the custom value.  
	* _8 Bit Value_
	* _16 Bit Value_
	* _32 Bit Value_ 
	* _64 Bit Value_ 
	* _Color Value_
	* _String Value_ - (Consumable by the Launcher & RDS Controllers)

* **Value** - Custom numeric value, string, or color (RGB) as determined by the **Data Type** property.


---





