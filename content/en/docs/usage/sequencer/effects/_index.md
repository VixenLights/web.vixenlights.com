---
title: "Effects"
linkTitle: "Effects"
date: 2017-01-05
description: >
  This section covers all of the effects in Vixen and details the features and how to use them.
---

### String Based Effects ###

All effects support being applied to the elements in a string like format. Depending on the setup of the elements, groups of elements can form a representation of a string. Most effects apply their logic based on those groups acting like a string. This mode is designated by the Target being set to Strings

### Location Based Effects ###

Location based effects create their effects by using the relative location of the elements as defined by their location in the preview. When creating you elements, they should be positioned in relative space to each other the same as they would be when in the display. This allows the effect to apply its logic based on where they lie in 2D space. This is sometime referred to a whole house model, but int he case of Vixen it relates to whatever elements are in the group you place the effect. This can be your entire house or just several props. You have complete flexibility here based on your group definitions.

As of 3.5 release the following effects support rendering based on location or as strings: Balls, Bars, Border, Butterfly, Circles, Colorwash, Coutdown, Curtain, Picture, Pinwheel, Plasma, Text and Video. In the editor set the Target drop down to Locations.
