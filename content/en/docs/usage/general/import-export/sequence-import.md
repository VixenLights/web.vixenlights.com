---
title: Sequence Import
author: Vixen Team
weight: 20
description: This section covers importing a sequence package of shared sequences.
---

### Overview

New in 3.6u1 is the ability to import/export a sequence package. This packages up all the necessary items to share sequence(s) from a profile with someone else, or another profile of your own with different elements. See the section on [Exporting][1].

### Importing

From the main admin window, select **Tools -> Import Sequence Package** from the menu. A wizard workflow will walk you through making an export package of the sequence(s) you want to share.

Step one is selecting the package file to import. This is generated from the Export process described above and has a .vpkg extension. Use the file browser to browse to and select the file to use. The next section is about the mapping file to map the profile elements for the imported sequences to the current profile. If this is the first time importing from the package or profile, you will need to create the map file. If you have previously imported sequences from this package or the same profile the package came from, you can use the file browser to select an existing saved mapping.

#### Creating a mapping file

You must have a package file selected before you can create a mapping. When you choose to create a mapping file, you will be presented with a screen that has the two element trees. One from the incoming package showing the source tree the sequence(s) are based on. The other tree is the destination tree of the current profile. These are presented in two columns and drag drop is used to drag the element from the destination tree to element on the source tree you want effects to map to. Once you drag it across to map it, the source tree will reflect the mapping. To replace a mapping, drag another item to it. To delete a mapping, select the mapped item and use the delete key. You do not need to map every item if you do not plan to use the effects from that source item. You only need to map what you want or what fits to your display. Once you are happy with all the items you want to map, then you can click Ok. Once clicking ok, you will be prompted to save the map file. Choose an appropriate name and location and save it. Once saved, the wizard will autofill the path you saved the map to in the map file entry box.

#### Selecting Sequences

Step 2 is selecting the sequences you wish to import. The screen will show you the sequences included in the package file and you can check the ones you wish to import. Multi-select can be used to select the items to change. Pressing space will toggle the state of any selected items.

#### Summary

Step 3 is a summary of what will be done. If the summary looks correct, then press next. 

Final step is the actual import with progress showing the steps. This will take each sequence selected and map the effects in it to the current profile using the mapping file. It will copy in any audio and media files used in the sequences that are imported. When it is complete the newly imported sequences will be in the sequence folder and can be opened in the editor to play or further edit.

### Hints and Tips

The import can map most everything including mark collections, layers, and media files like video and pictures that the effects use. One thing it cannot handle is Face mapping. If you map the Face elements from the imported sequences to Face elements in the destination that already have Face mappings created, they should generally just work. If the imported sequences used image mapping for faces, those will not be included. you may need to map those effects to your existing image maps, or create maps that are appropriate.

### Tutorial

{{< youtube wjpftzQ2hbk>}}

[1]: {{< ref sequence-export>}}
