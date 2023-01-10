---
title: Sequence Import / Export
author: Jeff
date: 2019-08-09T14:35:17+00:00

---
### Introduction

New in 3.6u1 is the ability to export/export a sequence package. This packages up all the necessary items to share sequence(s) from a profile with someone else, or another profile of your own with different elements.

### Exporting

From the main admin window, select Tools -> Export Sequence Package menu. A wizard workflow will walk you through making an export package of the sequence(s) you want to share. 

Step one is selecting the sequences you want to package. There is a file browser to choose individual sequences, or you can select the middle icon which will add all sequences in the sequence folder. The last icon is used to delete selected sequences from the list. The list supports multiple selection with the normal Shift/Ctrl click or drag select.

Step two allows you to choose the package name and location to save it. The extension for packages is .vpkg. The wizard will suggest a file and path name based on the profile name. The default location to save the package is in the Export folder of the current profile. You can choose the path that makes sense for you. The other option is whether to include the audio files that are used in the sequence. In some cases you may not want to share the audio files and they can be specifically excluded. The default is to include them.

The last step is a Summary confirmation window to validate what will occur. If the summary is correct you can click next and the export will occur. Progress bars will show the status of the export as it proceeds. If there are many sequences, it may take a while to export all of them.

Once finished you have a package file that can be shared. It is fully standalone and has all the information necessary for the import process to use.

### Importing

From the main admin window, select Tools -> Import Sequence Package menu. A wizard workflow will walk you through making an export package of the sequence(s) you want to share.

Step one is selecting the package file to import. This is generated from the Export process described above and has a .vpkg extension. Use the file browser to browse to and select the file to use. The next section is about the mapping file to map the profile elements for the imported sequences to the current profile. If this is the first time importing from the package or profile, you will need to create the map file. If you have previously imported sequences from this package or the same profile the package came from, you can use the file browser to select an existing saved mapping.

#### Creating a mapping file

You must have a package file selected before you can create a mapping. When you choose to create a mapping file, you will be presented with a screen that has the two element trees. One from the incoming package showing the source tree the sequence(s) are based on. The other tree is the destination tree of the current profile. These are presented in two columns and drag drop is used to drag the element from the destination tree to element on the source tree you want effects to map to. Once you drag it across to map it, the source tree will reflect the mapping. To replace a mapping, drag another item to it. To delete a mapping, select the mapped item and use the delete key. You do not need to map every item if you do not plan to use the effects from that source item. You only need to map what you want or what fits to your display. Once you are happy with all the items you want to map, then you can click Ok. Once clicking ok, you will be prompted to save the map file. Choose an appropriate name and location and save it. Once saved, the wizard will autofill the path you saved the map to in the map file entry box.

#### Import Continued

Step 2 is selecting the sequences you wish to import. The screen will show you the sequences included in the package file and you can check the ones you wish to import. Multi-select can be used to select the items to change. Pressing space will toggle the state of any selected items.

Step 3 Summary of what will be done. If the summary looks correct, then press next.

Final step is the actual import with progress showing the steps. This will take each sequence selected and map the effects in it to the current profile using the mapping file. It will copy in any audio and media files used in the sequences that are imported. When it is complete the newly imported sequences will be in the sequence folder and can be opened in the editor to play or further edit.

### Things to be aware of

The import can map most everything including mark collections, layers, and media files like video and pictures that the effects use. One thing it cannot handle is Face mapping. If you map the Face elements from the imported sequences to Face elements in the destination that already have Face mappings created, they should generally just work. If the imported sequences used image mapping for faces, those will not be included. you may need to map those effects to your existing image maps, or create maps that are appropriate.

[Video Tutorial]({{< ref seq-import-export-videos>}})
