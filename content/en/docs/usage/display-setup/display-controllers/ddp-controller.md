---
title: DDP
author: Vixen Team

---

## Description

The DDP Controller is used for sending DDP data packets to a controller that supports the DDP protocol. Later Falcon and FPP based controllers are known to support the DDP protocol. But there may be others. It's an ethernet based protocol. It's not nearly as universal as Streaming ACN. It's slightly more efficient than sACN, but lacks many of the features. Because it's so simple and has no features, there's really nothing to configure beyond the unicast destination address.

See [DDP Protocol][1] for more information.

## Setup

There is minimal setup for this controller unlike the e1.31 controllers which have universes. You simply add the controller to your list of controllers and set the number of channels needed. In the setup screen accessed from the gear icon, you can set the destination ip address. Patching your Props to it is just like any other controller.

## Patching

Elements / Props are patched to this controller just like any other controller. Select the controller and when you patch, the selected elements will be patched to the next available channels. You can also select a range of channels and patch elements to those directly.

[1]:http://www.3waylabs.com/ddp/