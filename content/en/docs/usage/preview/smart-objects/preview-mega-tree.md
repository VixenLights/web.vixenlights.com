---
title: Mega Tree
author: Vixen Team
description: This section covers using the Mega Tree Smart object.
aliases: ['/vixen-3-documentation/preview/adding-items-to-the-preview/smart-objects/mega-tree/']
---

### Overview

A Mega Tree can be either **Pixel** based or **Standard** string based. A pixel Mega Tree has individually addressable pixels across the entire cane and a standard cane has a single strand of lights that span the cane.

### Adding a Mega Tree in Vixen 3.6+

**Start in the Preview instead of in Display Setup as you may have done in the past.**

You can add a Mega Tree using the wizard buy clicking the Mega Tree icon in the Smart Objects toolbar and then with the mouse, click a point in your preview to start the Mega Tree and drag from upper left to lower right. This will create a basic Mega Tree shape and launch the wizard. Next a dialog will appear to setup the basic attributes of the Mega Tree.

![Mega Tree Wizard](/images/docs/usage/preview/smart-shapes/mega-tree/mega-tree-std-setup.png)

In this dialog, you will provide the name for your Mega Tree. It defaults to Megatree, but if you are adding multiples, you will want to name them Megatree-1, Megatree-2, etc. The next entry is the string count and the prefix name for each string. This defaults to 16 and a prefix of S. Adjust the string count to the number of strings you have.

The next choice is to determine if you have a pixel tree or an analog tree of traditional light strings. If yours is a **Pixel** tree, then check the Pixel Tree box. You will then choose the number of pixels on each string and the pixel name prefix. The default is 50 nodes. Adjust the count to match your setup. If you have a **Standard** light tree, then skip over the pixel count.

The next section concerns the startign location for the wiring on your tree. Typical is the bottom left. If yo uare using zig zag strings, then set the option for Zig Zag and enter the number of pixels in each Zig Zag. This is only if you are not setting up the Zig Zag in hardware. This will affect the patching to compensate for hardware that cannot do Zig Zag or if you choose to do it in software istead. It will setup a patching order, so you can just patch it straight through on the Display Setup screen. This does not generally apply to **Standard** light trees.

Setup for a **Pixel** Tree

![Mega Tree Wizard](/images/docs/usage/preview/smart-shapes/mega-tree/mega-tree-pixel-setup.png)

Once you select Ok, the next step will be whether to add a Dimming Curve or not. See the section on [Dimming Curves][3]

After the Dimming Curve, is a dialog to set up the color type of the prop. Depending on the type of lights you are using, the choice here will vary depending on the type of lights used in your Mega Tree. See the section on [Color Handling][4].

After setting the Color Handling, the Mega Tree will be completed and the elements will show up in the tree. All the linking will be done and you are ready to use it. You can resize or move it around using the preview tools.

### Adding a Mega Tree Manually

There are two different ways to add a mega-tree to the preview display. You can either auto-assign elements to the mega tree when it is drawn, or you can draw the object and define the linked elements later. Both methods have their benefits.

If you have already taken the time to define your element groupings, then you can save a lot of time vs linking the tree manually to elements.

Sometimes, it is nice to just start drawing& on the screen to test your ideas and plan the props you may want to add to your display. In this case, you might just want to play around with placement of objects that you may or may not have created in your element tree. Vixen allows you do place items on the preview without pre-linking them to elements.

Method 1: Auto-Linking Elements

* Click on the main element group for your mega-tree.
* Click on the Mega Tree icon on the toolbar.
* Left-click and hold the mouse button at the top left corner where you want to position the mega tree and, while holding the mouse button, drag to the bottom right to size the tree.

Notes on Auto Linking

* A mega tree without pixels must have 4 or more strings. Each of the child strings in your mega tree must not be a group.
* A pixel mega tree must have a main group with more than 4 sub-groups. Each string in the mega tree (sub-groups) must define more than 4 pixels each and all strings must have the same number of pixels.

Method 2: Manually Linked Elements

* Click on the main element group for your mega-tree.
* Click on the Mega Tree icon on the toolbar.
* Left-click and hold the mouse button at the top left corner where you want to position the mega tree and, while holding the mouse button, drag to the bottom right to size the tree.

### Settings

After the tree is drawn, there are many options that can be set to adjust the look of the tree on the preview.

### Element Links

Click on the Setup button to link elements to the strings in the Mega Tree. Elements are linked to the mega tree in the [Element Links Screen][1].

## String Type

See the [common settings][2] section for more information.

### Light Size

See the [common settings][2] section for more information.

### String Count

The string count is the total number of visible strings you have in your mega tree. If you&#8217;ve got a 180 degree mega tree and you want 10 strings, set the string count to 10.

### Lights per String

Enter the number of lights in each string. This is the same for all strings in the tree.

### Top Height

A mega tree is made up of a top ellipse and a bottom ellipse connected by light strings. This is the height of the top ellipse.

### Top Width

A mega tree is made up of a top ellipse and a bottom ellipse connected by light strings. This is the width of the top ellipse. It can be as small as 1 or as large as you want. It can even be larger than the base if that&#8217;s the way you want it.

### Base Height

A mega tree is made up of a top ellipse and a bottom ellipse connected by light strings. This is the height of the bottom ellipse. The width of the ellipse is defined by re-sizing the tree on the preview screen.

[1]: {{< ref preview-linking-elements>}} "Linking Elements"
[2]: {{< ref preview-common-settings>}} "Common Settings"
[3]: {{< ref dimming-curves>}} "Curves"
[4]: {{< ref color-handling>}} "Color Handling"
