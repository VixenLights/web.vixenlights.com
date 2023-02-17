---
title: LipSync
author: Vixen Team
description: Creates an effect used to syncronize lyric phomemes to a prop.
aliases: [/vixen-3-documentation/sequencer/effects/lipsync/]
---

### Overview

The Lip-sync effect helps to facilitate sequencing singing faces. It is a multi purpose effect that has evolved over the years into a powerful tool for syncronizing lyrics to your face mapped props. This effect relies on the mapping of the face properies in your elements in order to work properly.

---

### Configuration

* **Phoneme/Marks** This setting determine how the **LipSync** effect behaves.
  * **Mark Collections** Since Version 3.5. This set the effect to get its phomeme information from the [Marks][1] in a Mark Collection. This is the default and the most common way to use the effect.
    * **Mark Collection** This sets the Mark Collectin that contains the Marks with the Phonemes in it. There are typically 3 types of collections. Phrases, Words, and Phonemes. You select the Phonemes one here.
    * **Allow Mark Gaps** When enabled, the effect does not fill gaps between the Marks with a REST.
  * **Phoneme** This allows the effect to be used in manual mode where you configure the phoneme you want to use specifically.
* **Mapping Type** This allows you to choose the mapping type. This controls how phonemes are mapped to the individual elements in your Prop.
  * **Face Mapping** This option is used when you have a Prop that is usually a defiend shape and you have mapped specific elements to the mouth phonemes.
  * **Image Mapping** This option is used for matrix type props that use an image for a mouth shape rather than mapping individual lights or elements.
* **Eye Mode** This sets how the eyes should be handled when the effect is active.
  * **Open** This sets the eyes to open using the open eyes mapping.
  * **Closed** This sets the eyes to be closed using the eyes closed mapping.
  * **Off** This sets the effect to ignore turning on the eyes.
* **Show Outline** This sets the effect to turn on the outline using the outline mapping.

---

### Lip-Sync Enhancements

Since Vixen 3.5

{{< youtube i3quOLEFHv8>}}

&nbsp;

{{< youtube RhBecwSIAfo>}}

[1]: {{< ref marks>}} "Marks"
