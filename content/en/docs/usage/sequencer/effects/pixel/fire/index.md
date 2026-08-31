---
title: Fire
description: Creates an effect that simulates burning fire.
aliases: [/vixen-3-documentation/sequencer/effects/fire/]
---

---

## Overview

Creates an effect that simulates burning fire.

---

## String Setup

* **Positioning** - Determines how the target elements are treated.  Either as individual strings or by their actual location in the display preview.
                      *Locations* is often referred to as whole house, but it can be any form of multiple props.
                      Generally you want *Strings* when applying to one prop and *Locations* if the target is multiple props.

* **Orientation** - Controls the orientation of the display area (matrix).

---

## Configuration

* **Location** - Selects the side of the grid for the base of the fire (_Bottom_, _Top_, _Left_, _Right_).

* **Height** - Adjusts the flame height. This parameter is a curve that allows you to vary the height over the duration of the effect.

---

## Color

* **Hue Shift** - Adjusts the color of the flame as a hue shift from normal fire colors.

---

## Brightness

* **Intensity** - This is an overall brightness intensity curve for over the duration of the effect.
                  This is a legacy parameter, consider using intensity overlay layers instead.

---

## Behavior

Since Build 1520.

* **Across Elements/Groups** is the default behavior and is equivalent to how the effect has always acted. Fire combines every element under the target into a single simulation area, so one fire simulation is rendered across the whole combined target.

* **Each Element/Group** applies an independent Fire simulation to each child element or group instead of combining them into one. Each child gets its own local simulation area, so the fire is generated separately for every group. This is useful for applying the same Fire effect to, say, each Arch in a group rather than simulating a single fire across all the Arches together.

  The **Behavior** section, and the **Depth** section below, only appear when the target has enough levels in its hierarchy for this choice to matter, or when more than one element/group is targeted. If only a single target with a shallow hierarchy is selected, Fire always behaves as **Across Elements/Groups**.

---

## Depth

* **Levels Deep** - Only available when **Behavior** is set to **Each Element/Group** and a single target is selected. Controls at what level of the target's hierarchy each independent Fire simulation is applied. Depth choices that would simply resolve to individual leaf elements are excluded from the list since they aren't useful for this effect. When more than one element/group is targeted, each selected target is treated as its own independent group and this setting doesn't apply.

---

## Video

{{< video src="Fire.m4v" height="110" width="110" preload="auto" autoplay="autoplay" loop="loop" type="video/mp4">}}

---
