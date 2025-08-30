---
title: RDS
author: Vixen Team
description: RDS effect for sending text to the RDS controller at precise time(s) during a sequence.
---

---

### Overview

This effect sends text to the RDS controller at the precise time(s) during a sequence and is used in conjunction with the [RDS Controller][1]. Position the effect in the sequencer timeline at the point you want the text sent to the device. This would typically be at the very beginning of the sequence for a typical RDS artist / song. The duration of the effect has no real purpose. It is triggered once at the beginning of the effect time. 

---

### Configuration

* **RDS Text** - Text to send to the RDS controller. This is typically the artist or song name. Anythign your device supports as text.

---

![RDS Effect](/images/docs/usage/sequencer/effects/device-action/rds/rds-effect.png)

[1]: {{< ref "docs/usage/display-setup/display-controllers/rds-controller">}} "RDS Controller"
