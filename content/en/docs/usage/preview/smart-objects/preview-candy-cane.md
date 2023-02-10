---
title: Candy Cane
author: Vixen Team
description: This section covers using the Candy Cane Smart object.
alias: /vixen-3-documentation/preview/adding-items-to-the-preview/smart-objects/candy-cane/
---

### Overview

A Candy Cane can be either **Pixel** based or **Standard** string based. A pixel Candy Cane has individually addressable pixels across the entire cane and a standard cane has a single strand of lights that span the cane.

### Adding a Candy Cane in Vixen 3.6+

**Start in the Preview instead of in Display Setup as you may have done in the past.**

You can add a Candy Cane using the wizard buy clicking the Candy Cane icon in the Smart Objects toolbar and then with the mouse, click a point in your preview to start the Candy Cane and drag from upper left to lower right. This will create a basic Candy Cane shape and launch the wizard. Next a dialog will appear to setup the basic attributes of the Candy Cane.

![Candy Cane Wizard](/images/docs/usage/preview/smart-shapes/candy-cane/candy-cane-setup.png)

In this dialog, you will provide the group name for your Candy Cane. It defaults to CandyCane, but if you are adding multiples, you will want to name them CandyCane-1, CandyCane-2, etc. The next entry is the name the segments will be called. This defaults to CandyCane Px. If you are adding multiple Candy Canees, you would name this CandyCane-1 Px or CandyCane-2 Px. The Px is just a shortcut for pixel, you can use anything you like for the segments. Each segment will have a number appended to this name. Example CandyCane-1 Px-1, CandyCane-1 Px-2.

Last is the number of segments. If this is a **Pixel** Candy Cane it would be the number of pixels. If it is a *Standard** Candy Cane wrapped with segments of light strings, it will be the number of light segments. It defaults to 25.

Once you select Ok, the next step will be whether to add a Dimming Curve or not. See the section on [Dimming Curves][3]

After the Dimming Curve, is a dialog to set up the color type of the prop. Depending on the type of lights you are using, the choice here will vary depending on the type of lights used in your Candy Cane. See the section on [Color Handling][4].

After setting the Color Handling, the Candy Cane will be completed and the elements will show up in the tree. All the linking will be done and you are ready to use it. You can resize or move it around using the preview tools.

### Linking Elements

[See Linking Elements][1]

### Properties

### Position

See Position in [Common Settings][2]

### Light Count

For an Candy Cane, this is commonly the number of segments in the Candy Cane. If your Candy Cane has 25 pixel segments, it will be 25. If you have 9 segments of analog lights, the number will be 9.
See Light Count in [Common Settings][2]

### Light Size

See Light Size in [Common Settings][2]

### Linked Elements

See [Linking Elements][1]

### String Type

The string type of a Candy Cane will probably be Pixel for nearly everyone.

[1]: {{< ref preview-linking-elements>}} "Linking Elements"
[2]: {{< ref preview-common-settings>}} "Common Settings"
[3]: {{< ref dimming-curves>}} "Curves"
[4]: {{< ref color-handling>}} "Color Handling"
