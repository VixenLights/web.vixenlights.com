---
title: Falcon Pi Player
author: Vixen Team
weight: 30
description: This section covers exporting a sequences to be played on the Falcon Pi Player.
---

### Overview

The Falcon Player (FPP) is a lightweight, optimized, feature-rich sequence player designed to run on low-cost Single Board Computers (SBC). It was originally created to run on the $35 Raspberry Pi, hence the middle 'P' in the short name but now the FPP supports many more systems. It is still mostly commonly used on a Raspberry Pi (Zero, 2, 3, 4) or a Beagle Bone (Black, Green, Pocket).

The FPP shorthand is still used but it is now just called Falcon Player.

FPP aims to be controller agnostic, it can talk E1.31, DDP, DMX, Pixelnet, and Renard to hardware from multiple hardware vendors. Using various capes, FPP can also be a controller on P5 and P10 Matrixes, or strings of ws2811 pixels.

Useful Links:

- [FPP Documentation in Github](https://github.com/FalconChristmas/fpp/tree/master/docs/README.md)
- [Falcon Christmas forums](http://falconchristmas.com/forum/)
- [Falcon Player sub-forum](http://falconchristmas.com/forum/index.php/board,8.0.html)
- [Wiki](http://falconchristmas.com/wiki/index.php/Main_Page)
  
### Vixen Support

Vixen can export FSEQ files to be played on the FPP player or FPP based controller. There are two ways to export. Sequence at a time from within the [Sequencer][1] and via an Export Wizard than can export multiple sequences at a time.

### Export Wizard

The Export Wizard is the recommended way to export your sequences. It was added on to help automate the exporting of an entire shows worth of sequences instead of having to do them one at a time in the [Sequencer][1].

#### Getting Started

The Export Wizard can be started from the main Admin window. **Tools -> Export Wizard**. This will start the process of configuring an export or using a prevouisly configured one. The first screen will ask if you want to create a new configuration or use an existing one. If this is the first time using, you will choose to *Create new export configuration*. IF you have used it before and saved a configuration, then you will choose to *Use saved export configuration*. If you are using an existing, once you choose that option, you will have a drop down to select the saved configuration to use. Choose next to move on.

#### Selecting Sequences

The next screen will aloow you to select or review the sequences to be exported. If you used a save configuration, this will be pre-populated with the sequences used before. You can edit to add or remove to get the list of sequences you need. The folder open icon will allow you to browse and select the sequences you want to add. The second multifolder icon will automatically add all sequences in the seuence folder for the current profile. The last option is the red X to remove any selected sequences from the list. Once you have the sequences you need in the list, you can choose next.

#### Configure Outputs

The next screen allows you to choose the controller blocks and the order they should be exported in. The check boxes on each controller determine if it is included in the export. You can drag and drop the controllers into any order desired. The channel ranges will be adjusted to match the new order. This will need to directly match the intended setup in FPP. Vixen can export the controller config for use in FPP, so that can be automated. In that case the controller order is not really important. All that matters is they match. If you are exporting from other sequencers, then you need to ensure they are configured the same. Once you have the proper controllers and order set, you can choose next.

#### Output Format and Destination

The next screen will be used to setup how to do the export. Here you can choose the output format and the timing to be used. The default of Falcon Player Sequence 2.6+ should be used for modern versions of FPP. There are other options to support legacy versions as well as exporting to older Vixen 2 formats and even CSV.

Once you have chosen a format, the next section will adapt for the format. For Falcon 2.6+, the main options here are as follows.

- **Create Universe File** This specifies if the universe configuration file should be genrated that reflects the controller and channel mapping. This generated in the exact format that FPP uses. It can be directly uploaded to replace the existing configuration.
- **Include Audio** This specifies if the audio file should be included as part of the export. If enabled, the audio file will be named the same as the sequence file to ensure FPP can locate it automatically.
- **Backup Universe File** If the export location already has a universe file it will be renamed before it is replaced with the new one created when **Create Universe File** is enabled.
- **Enable Conpression** This enables the FSEQ file to be compressed. The default is enabled and recommended.

The last area is the output folder. This can be a file folder on your computer, or the shared location on the FFP device itself if Sambe file sharing is enabled on the FPP. This was enabled by default on FPP versions 5 and older, but on 6+ it has to be enabled in the settings under **FPP Settings -> System** In the section OS Settings select Enable Samba/CIFS. This will allow you to direcly export to the FPP folder over a network connection. You can use \\ip\\fpp by changing ip to either the ip addess of the FPP device, or the hostname if you have DNS. If you directly export to FPP, the export wizard can place all the files where they belong including the universe file, sequences, and audio. If you export to the file system, the output folder structure will mimic the structure on FPP. You can then manually upload the files for FPP. If you let the wizard export to FPP, you will need to restart the FPPD Daemon.  

#### Summary

The last screen is the summary screen that details what will be done. There is also an option to save thsi configuration for future use. You can enter the name, or choose an existing configuiration to update. After you hit next, it will commence exporting. There will be progress bars showing the progress through the process.

### Sequence Editor Export

Under **File -> Export** in the sequencer is the legacy export. It is very similar to the wizard, but much simplier in that it can only export the seuence you have open in the editor. You cannot save any setting in it either. This is retained for legacy purposes, but may be removed in the future, so the recomendation is to use the wizard.

[1]: {{< ref sequencer>}}
