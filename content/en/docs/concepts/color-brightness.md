---
title: Color and Brightness
author: Jon Chuchla
weight: 20
date: 2014-08-13T14:06:27+00:00

---
Color and brightness are handled a bit differently in Vixen 3.  To understand the color system in Vixen 3, you need to know a little bit about color models.

### RGB (Red Green Blue)

The **RGB** (**R**ed, **G**reen, **B**lue) color model is the most well known and is what is used most commonly in other sequencers. It defines a color space in terms of three components:

* **R**ed, which ranges from 0-255
* **G**reen, which ranges from 0-255
* **B**lue, which ranges from 0-255

The **RGB** color model is an additive one. In other words, **R**ed, **G**reen and **B**lue values (known as the three primary colors) are combined to reproduce other colors. For example, the color "Red" can be represented as [R=255, G=0, B=0], "Violet" as [R=238, G=130, B=238], etc.

Its common graphic representation is the following image:

![RGB Color Space](http://colorizer.org/img/rgb.png "RGB Color Space")

### HSB (HSV) color space

The **HSB** (**H**ue, **S**aturation,  **B**rightness) color model defines a color space in terms of three constituent components:

* **H**ue : the color type (such as red, blue, or yellow).
  * Ranges from 0 to 360° in most applications. (each value corresponds to one color : 0 is red, 45 is a shade of orange and 55 is a shade of yellow).
* **S**aturation : the intensity of the color.
  * Ranges from 0 to 100% (0 means no color, that is a shade of grey between black and white; 100 means intense color).
Also sometimes called the 'purity' by analogy to the **colorimetric** quantities excitation purity.
* **B**rightness (or **V**alue) : the brightness of the color.
  * Ranges from 0 to 100% (0 is always black; depending on the saturation, 100 is the brightest version of the color in the given hue and saturation.).

Its common graphic representation is the following image:

![The conical representation of the HSV model; Wikipedia image.](http://colorizer.org/img/hsv.png "The conical representation of the HSV model; Wikipedia image.")

The **HSB** model is also known as **HSV** (**H**ue, **S**aturation, **V**alue) model. The **HSV** model was created in 1978 by [Alvy Ray Smith](http://en.wikipedia.org/wiki/Alvy_Ray_Smith "Alvy Ray Smith"). It is a nonlinear transformation of the RGB color space. In other words, color is not defined as a simple combination (addition/substraction) of primary colors but as a mathematical transformation.

**Note:** **HSV** and **HSB** are the same, but **HSL** is different.  HSL and other color models are beyond the scope of this document and will not be explained here.

### Color Models and Light Sequencers

As mentioned earlier, most sequencers other than Vixen 3 use the RGB color model.  While this corresponds conveniently with most basic RGB lighting devices, it's not particularly convenient for actually working with color and brightness transitions in lighting design.  For lighting applications, the HSV color model is a more suitable system for conceptually working with color and brightness.  It is actually more useful to think about color and to interact with it using the parameters of the HSV system.  For example, in the RGB color model, if you wanted to make the lights brighter, you would have to take all three values and increase them proportionally.  In the HSV model, you would just increase the V value.  Similarly, if you want to make a color more or less vibrant, you would increase or decrease the saturation.

Of the 3 parts of a HSV color, only two parts describe the color: the Hue and Saturation.  The Value describes how bright the color is.  In vixen 3, the Hue and Saturation are controlled by the color controls (color picker or gradient editor). This describes the color itself.   The Value is always tied to the brightness controls (intensity or curve).  This is how bright the light is.

You'll notice in the color picker, that the V is always 100.  You can only choose the full brightness version of any given color.    This is often a point of confusion with users who are used to other sequencers. If you want to adjust the intensity, you don't use the color picker.  That is done using the intensity controls.  For example, if you wanted to create a dark green color, you might be familiar with using like RGB values 17, 130, 41.  This translates to a Hue of 133, Saturation of 87 and a Value of 51.  The value will always be 100 on the Vixen 3 color picker.  Vixen will automatically correct this to 100, and you will see your RGB values change to 33, 255, 80.  This looks like a bright green.  There's nothing wrong here, this is how it is designed to work.  To get that dark green, you then need to set the intensity (or curve, depending on the effect) to 51.

### Colors and Gradients

The word Color is used to refer to a color that doesn't change over time.  Colors that change over time are referred to as Gradients.  Gradients contain one or more colors, and the timing relationship of when the colors change.  The time relationship is not absolute.  It is a percentage relative to the length of the effect.

### Intensity and Curves

Similar to the concept of colors and gradients above; an intensity is a fixed brightness value.  A Curve is a change in brightness over time.  The time relationship is not absolute.  It is a percentage relative to the length of the effect.

&nbsp;

**Color model explanations and imagery from colorizer.org.*
