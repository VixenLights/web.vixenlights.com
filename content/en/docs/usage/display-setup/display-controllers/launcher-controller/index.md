---
title: Launcher
author: Vixen Team

---

## Description

The Launcher Controller is used for triggering an external command from within Vixen. It is used in combination with the [Launcher Effect][1] that passes the command line executable and any arguments through to this controller at a specified time.

## Setup

There is minimal setup for this controller. Just add it to your controller list and ensure it is enabled. You typically only need one ouput which is the default.

## Patching

A single Element is normally directly patched to this controller. There should be no color breakdown or dimming handlers in the path. It should resemble the following.

![Launcher Display Setup](/images/docs/usage/controller-setup/launcher/launcher-setup.png)

[1]: {{< ref "docs/usage/sequencer/effects/device-action/launcher">}} "Launcher Effect"
