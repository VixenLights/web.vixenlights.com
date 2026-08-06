---
title: LipSync
author: Vixen Team
description: Creates an effect used to syncronize lyric phomemes to a prop.
aliases: [/vixen-3-documentation/sequencer/effects/lipsync/]
---

## Overview

The Lip-sync effect helps to facilitate sequencing singing faces. It is a multi purpose effect that has evolved over the years into a powerful tool for syncronizing lyrics to your face mapped props.

The phoneme codes used throughout this effect (and in your Mark labels) are the standard Preston Blair/Papagayo set: **AI**, **E**, **O**, **U**, **FV**, **L**, **MBP**, **WQ**, **ETC**, and **REST** (mouth closed/idle).

When **Mapping Type** is set to **Face Mapping** (the default and most common setup), this effect relies on the target elements having a [Face property][3] configured, mapping individual elements or lights to mouth phonemes, eyes, and an outline.

---

### Configuration

* **Phoneme/Marks** This setting determines how the **LipSync** effect gets its phoneme information.
  * **Mark Collections** Since Version 3.5. This is the default and the most common way to use the effect. It sets the effect to get its phoneme information from the [Marks][1] in a Mark Collection.
    * **Mark Collection** This sets the Mark Collection that contains the Marks with the Phonemes in it.
      * Since Build 1465, the dropdown is filtered to only show Mark Collections that are tagged as **Phoneme** collections, so Phrase, Word, and other unrelated collections no longer clutter the list. If the effect already has a non-Phoneme collection selected (for example from an older sequence), that collection remains selected and is shown in the list like before so you can still see and continue using it. Once you pick a real Phoneme collection, that legacy entry drops out of the list.
    * **Allow Mark Gaps** When enabled, the effect does not fill gaps between the Marks with a REST.
  * **Phoneme** This allows the effect to be used in manual mode where you configure a single phoneme for the whole effect, rather than pulling one from Marks.
    * **Phoneme** Selects the single phoneme mouth shape to hold for the entire length of the effect.
    * **Lyric** A free-text label for the lyric this phoneme is associated with. It's purely informational — it's shown on the effect block for your own reference and doesn't affect rendering.
* **Mapping Type** This allows you to choose the mapping type. This controls how phonemes are mapped to the individual elements in your Prop.
  * **Face Mapping** This option is used when you have a Prop that is usually a defined shape and you have mapped specific elements to the mouth phonemes via the [Face property][3]. Selecting this reveals the **Eye Mode** and **Show Outline** options below.
  * **Image Mapping** This option is used for matrix type props that use an image for a mouth shape rather than mapping individual lights or elements — it treats the target like a pixel matrix and draws a phoneme image onto it, similar to the Picture effect. It doesn't require a Face property. Selecting this reveals the [Image Mapping](#image-mapping) options below instead of Eye Mode and Show Outline.
* **Eye Mode** Only available when **Mapping Type** is **Face Mapping**. This sets how the eyes should be handled when the effect is active.
  * **Open** This sets the eyes to open using the open eyes mapping.
  * **Closed** This sets the eyes to be closed using the eyes closed mapping.
  * **Off** This sets the effect to ignore turning on the eyes.
* **Show Outline** Only available when **Mapping Type** is **Face Mapping**. This sets the effect to turn on the outline using the outline mapping.

---

### Image Mapping

These settings only appear when **Mapping Type** above is set to **Image Mapping**.

* **Image Map** Chooses which phoneme-to-image library to use for mapping phonemes to mouth images. See [LipSync Image Maps][6] for how to create and edit these.
* **Orientation** Defines the direction of the strings and controls how the effect is oriented on the element — **Horizontal** or **Vertical**.
* **Scale To Grid** When enabled (the default), automatically scales the phoneme images to match the element's pixel grid size.
  * **Scale** Only shown when **Scale To Grid** is off. Controls the percentage to scale images down by, to fit large images onto the grid. Range is 1-100%.
* **X Offset** and **Y Offset** Two [Curves][4] that let you shift the phoneme image's horizontal and vertical position over the course of the effect, instead of leaving it centered the whole time. See the [Inline Curve Editor][5].

---

### Brightness

* **Intensity** Only available when **Mapping Type** is **Image Mapping**. Controls the overall brightness the phoneme images are rendered at. Range is 1-100%.

---

### Lip-Sync Enhancements

Since Vixen 3.5

{{< youtube id="i3quOLEFHv8" title="Lip-Sync Enhancements">}}

{{< youtube id="RhBecwSIAfo" title="Lip-Sync Enhancements (Continued)">}}

---

### Lyric Tracks

A good way to get lyric tracks that are very close to begin with is to use a track generator. One that works pretty well is the [Autolyrics][2] site. One of our users made a video that gives an overview of the process. When selecting the mark track to use in the effect, be sure to use the Phoneme one. If you need to make adjustments, you can adjust the phoneme marks to better align with the lipmovements you want. If the track is slightly off, you can select and move the blocks of phrases, words, phonemes to meet your needs. In most cases this gets you very close.

{{< youtube id="BJoWTXzQQew" title="Lyric Tracks">}}

[1]: {{< ref marks>}} "Marks"
[2]: <https://autolyrics.lightingfanatics.com> "Autolyrics"
[3]: {{< ref face-property>}} "Face Property"
[4]: {{< ref curves>}} "Curves"
[5]: {{< ref inline-curve-editor>}} "Inline Curve Editor"
[6]: {{< ref lipsync-image-maps>}} "LipSync Image Maps"
