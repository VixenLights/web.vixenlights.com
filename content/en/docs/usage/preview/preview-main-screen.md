---
title: Main Preview Screen
author: Vixen Team
weight: 10
description: This section covers the main Preview screen.
aliases: [/vixen-3-documentation/preview/main-preview-screen/]
aliases: [/vixen-3-documentation/preview/background-image/]

---

### Overview

The main preview screen is where the preview magic happens.

![Preview Setup](/images/docs/usage/preview/main-preview-screen/main-preview-screen.png)

From the top, you can see the main menu bar. You'll practically never need this unless you prefer words instead of pictures.

On the left, top of this screen is the Elements Tree. This is a duplicate of the elements tree you use to setup the [Display Elements & Groups][1].

Below the Elements Tree are the properties for the currently selected display item.

And, on the right is the stage. This is where you will do all the work to setup your display preview. As you add items, you&#8217;ll do it in this area.

### Toolbar

![Preview Toolbar](/images/docs/usage/preview/main-preview-screen/preview-toolbar.png)

The toolbar is used to tell the preview what you want to do. There are various groups in the toolbar.

### Background

To set the preview background, click the picture frame in the **Background** section of the toolbar.

The background image is usually a picture of your house that you use to define your lighting scene. Try to take the best shot you can looking directly your house. Stand way back and get the entire scene in a single picture - or stitch multiple pictures together. I would not recommend taking a panoramic picture as it tends to distort a lot toward the ends. You can try this, though, if you like.

#### Setting the Background Image

To set the background image, click on the picture icon in the preview editor toolbar (pictured above). This will bring up a standard Windows file selection dialog box. Most standard image formats are supported (JPG, GIF, PNG).

#### Background Image Intensity

Most lighting displays happen at night. You can use the slider next to the image toolbar button to set the intensity of the image on the screen. This can be changed at any time.

#### Resizing the Background Image

* From the **Edit** menu, select **Background Properties**
* Change the width. By default the height will adjust and keep the aspect ratio of the background image.
* Selecting the ![ChainLink](/images/docs/usage/preview/main-preview-screen/ChainLink.PNG) button will toggle between keeping the aspect ratio of the width and height fixed vs allowing
  both the width and height to be edited independently.
* All items on the preview will re-size and move to new locations to match the new preview image

* By unselecting **Scale Shapes** the preview can be expanded to allow more space for props.  
  This type of resize is often desired when a background image is not being used.

  ![Preview Background Resize](/images/docs/usage/preview/main-preview-screen/resize-background-dialog.png)

### Select

Clicking this button puts the preview in selection mode. This cancels any other item you may have selected.

### Basic Drawing

The basic drawing tools group the simple drawing tools for easy access. See the [Basic Shapes][2] for more information on how to use these items.

### Smart Objects

The more complicated items are grouped in the Smart Objects area. These are props such as your Mega Tree and Stars. For more information see [Smart Objects][3].

### Align

This section contains the tools for aligning and sizing preview objects to each other. The first preview shape you select is used as the reference for the alignment action. You need to select at least two preview shapes to use the alignment tools. Multiples can be selected with Ctrl Click, or the lasso selection. Alignment options include the following:

* Align Top - This will align the topmost edges of all selected shapes to the first shape selected.
* Align Bottom - This will align the bottommost edges of all selected shapes to the first shape selected.
* Align Left - This will align the leftmost edges of all selected shapes to the first shape selected.
* Align Right - This will align the rightmost edges of all selected shapes to the first shape selected.
* Distribute Horizontally - This will distribute the shapes evenly spaced between the leftmost and the rightmost shape.
* Distribute Vertically - This will distribute the shapes evenly spaced between the topmost and the bottommost shape.
* Match Properties - This will match similar properties on shapes like height and width.

### Location Offset

When using location based effects, the locations of your props on the preview screen provides the spatial location information used by the effects. This allows for a wipe across several props in a group, or whole house wipes or many other effects. But there are times when your whole display doesn’t fit into one preview. Or it isn’t convenient to work on when it’s all in a single preview. You may want to have multiple preview to show different sections of your display, but you still want to apply a wipe effect across all of them. One example is if you are sequencing for multiple houses. Each house would have its own preview. Another example is if you have a front yard and side yard display. You may want each view on a separate preview.
The Location Offset function in the **Settings** menu allows you to specify the relationship of a preview instance with respect to others. It lets you offset the coordinates of all the props on the preview by a given amount. For the side by side multiple houses, or side yard, front yard examples, You would look at the leftmost preview, and determine it’s dimensions. In the Edit menu, click on Background Properties. Make note of the existing image size dimensions. Then close this preview configuration screen and open the configuration screen for the next preview. In the Settings menu, select “Location Offset Setup”. If you want this second preview to appear to the right of the previous one, enter the width of the previous preview into the horizontal box. For example, if you have two previews that are 1920×1080 in size. You would enter 1920 into the Horizontal offset in the second preview.

### Help

Links you to this documentation.

### Close

When you're done editing this screen, click X button in the upper right or File -> Exit. Incremental changes may be saved using the File -> Save menu or Ctrl S. If you dod not save inside the preview you can save or cancel your changes in the [Previews Configuration][4]. If you made a huge mistake and want to lose your changes, click Cancel on the Previews Configuration dialog box and it will revert to the last saved change. That could be the save inside the preview, or to the last time you clicked OK in the Preview Configuration Dialog.

### Prop Wizards

Starting with Vixen 3.6, above the element tree is a drop down selector to add certain props that have wizards. This is similar to the same wizards in the Display Setup in that you can create the elements and the preview visual all in one step. You select the type of prop you want and then click the green + button to the right. You will be prompted by the wizard for the information needed to create it just like you would in Display Setup. Then once you fill in the info the preview visual will be created and automatically linked. You can then drag it around to position it where you wish. You can also drag the prop shape from the toolbar and it will also invoke the same wizrd as the template in the drop down.

### Element Tree

![Preview Toolbar](/images/docs/usage/preview/main-preview-screen/element-tree.png)

The Element Tree is the same tree used on the [Display Elements & Groups][2] screen. If you are using 3.6+, the best way is to create much of the setup in the preview. Most of the abilities to manipulate elements are available in the preview now. When using smart object or the templataes in the preview, it will walk you though setting up the color and dimming if desired. Patching and controllers are still managed in the Display Setup. If you are still using something older than 3.6, then you must start in the Display Setup and then link preview visuals to them. We highly recommend upgrading beyond 3.6 for the best experience. For the purposes of setting up elements, building a preview and then sequencing your display, you can skip the [Configure Controllers][5] section.

If you already have the elements created, then you can add a preview visual with the following steps.

  1. Select a single element or group of elements in the Element Tree
  2. Click on a shape
  3. Draw the element on the preview main display

For more information have a look at the section on [Linking Elements][6].

_Note:_ Clicking on an element or group of elements in the element tree will highlight individual pixels, individual strings or entire items depending on what is clicked on in the tree

### Item Properties

Display items all have properties associated with them. Along with multiple common properties, some items have custom properties that can be set. See the [Basic Shapes][2] and [Smart Objects][3] for more information on how to use these properties.

![Item Properties](/images/docs/usage/preview/main-preview-screen/arch-properties.png)

 [1]: {{< ref display-elements-groups>}} "Display Elements & Groups"
 [2]: {{< ref preview-basic-shapes>}} "Basic Shapes"
 [3]: {{< ref smart-objects>}} "Smart Objects"
 [4]: {{< ref preview-setup>}} "Previews Configuration"
 [5]: {{< ref controllers>}} "Controllers"
 [6]: {{< ref preview-linking-elements>}} "Linking Elements"
