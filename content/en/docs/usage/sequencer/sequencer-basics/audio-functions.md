---
title: Audio
author: Vixen Team
weight: 120
description: This section describes the Audio features.
---

## Overview

Most sequences will have an audio track that the lights are synchronized to. Vixen supports most formats of audio files and provides many features for incorporating audio into a sequence.

### Adding / Removing Audio

Audio can be added or removed from the options under the **Tools -> Audio** menu in the Sequencer. To add audio, click the **Associate Audio** menu or the musical note in the icon toolbar. A dialog will appear for you to select your audio file from the file system. Once you add an audio file, it will be copied into the Media folder in the Vixen profile. If the sequence is not the same length as the audio file, you will be prompted to ask if you would like to resize the sequence. If you choose yes, the sequence will be resized to match the audio file. This is generally the desirable state. You can replace the current audio file with another one by using the same **Associate Audio** menu. You will be prompted to ask if you want to replace the audio.

To remove an audio file, you can select the **Remove Audio** menu option. The audio that is currently associated will be removed. The length of the sequence will remain the same.

### Waveform

Once an audio file is associated, the Timeline will be updated with a waveform showing the general audio shape of the audio. This is similar to what you will see in other audio players or editors. It is based on sampling the audio and mapping that into the time available. Zoomming in and out of the timeline will increase or decrease the detail of the sampling. The waveform can take two shape. Either a full stereo waveform with each channel eminating from the the center, or a single mono form with the merged channels eminating upward. You can change toggle this under the **View -> Full Waveform** option in the toolbar menu. The vertical space the waveform occupies can be changed by hovering at the bottom of the waveform area until a cross bar cursor appears. Clicking and dragging will allow you to resize the area to the desired height.

### Beat / Bar Detection

Marks for audio beats and bars can be automatically detected on an audio track that has been added to the the sequence in the editor, under the menu in the toolbar **Tools -> Audio -> Beat/Bar detection**.  This will bring up a dialog to select the type of marks you want to generate. See [Beat / Bar Detection][1] under the section on Marks.

### Audio Playback Speed

The speed of the audio will change to follow along with the sequence playback speed. This can be changed by using the - + buttons on either side of the speed guage in the icon toolbar. 100 is normal speed. Numbers lower than 100 are slower, and numbers higher are faster.

### Speed / Tempo

Since Version 3.9.

The way in which the audi sounds when played at speed other than 100 can be changed by selecting the Speed / Tempo option in the toolbar under **Tools -> Audio**. The default is unchecked and will use speed as the playback option. If you select the option, it will use an algorythm to vary the tempo of the audio as the speed changes. Tempo may be useful in Lip Sync operations to better hear the words in an audio track.

[1]: {{< ref "marks#beat--bar-detection">}}
