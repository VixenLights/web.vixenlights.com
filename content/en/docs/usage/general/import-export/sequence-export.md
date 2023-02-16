---
title: Sequence Export
author: Vixen Team
weight: 10
description: This section covers exporting a sequence package for sharing with others.
---

### Overview

New in 3.6u1 is the ability to import/export a sequence package. This packages up all the necessary items to share sequence(s) from a profile with someone else, or another profile of your own with different elements. See the section on [Importing][1].

### Exporting

From the main admin window, select **Tools -> Export Sequence Package** menu. A wizard workflow will walk you through making an export package of the sequence(s) you want to share. 

Step one is selecting the sequences you want to package. There is a file browser to choose individual sequences, or you can select the middle icon which will add all sequences in the sequence folder. The last icon is used to delete selected sequences from the list. The list supports multiple selection with the normal Shift/Ctrl click or drag select.

Step two allows you to choose the package name and location to save it. The extension for packages is .vpkg. The wizard will suggest a file and path name based on the profile name. The default location to save the package is in the Export folder of the current profile. You can choose the path that makes sense for you. The other option is whether to include the audio files that are used in the sequence. In some cases you may not want to share the audio files and they can be specifically excluded. The default is to include them.

The last step is a Summary confirmation window to validate what will occur. If the summary is correct you can click next and the export will occur. Progress bars will show the status of the export as it proceeds. If there are many sequences, it may take a while to export all of them.

Once finished you have a package file that can be shared. It is fully standalone and has all the information necessary for the import process to use.

### Tutorial

{{< youtube wjpftzQ2hbk>}}

[1]: {{< ref sequence-import>}}
