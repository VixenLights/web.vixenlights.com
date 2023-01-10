---
title: Zip Wizard
author: Jeff
date: 2019-09-18T16:29:50+00:00

---
### Introduction

The zip wizard screen is accessed from the profile System => Profiles menu on the main admin form. It can be used to create backups, copy a profile to another PC, provide a copy to developers to help debug, or share with others and has several options to configure it. Profiles are stored in the My Documents folder by default. This PC\Documents or c:\Users\bob\Documents where bob is the current logged in user. This shows up in various forms depending on the version of windows, but it is the traditional My Documents folder. Profiles generally start with Vixen 3 in the folder name if the defaults are used, but that is not mandatory. 

![Zip Backup Wizard](/images/docs/usage/general/zip-wizard/ZipWizard_Backup.png)

### Backups

The primary use of the zip wizard is to make a backup of your profile to restore in case something goes wrong, move it to another machine, or share with others. The settings above are the most common for this use. This will recreate the profile structure into a zip file and save it in the name and location specified. It will cover any changes to the Display Setup / Preview as well as sequences and audio files. This files in the zip archive will be relative to the profile location which is normally in the users My Documents folder.

### Restoring Backup

If you need to restore a backup, it can be extracted into the users My Documents folder. This is typically in the form of c:\Users\bob\Documents where bob is the logged in user on the PC. If you are restoring on the same PC where the backup was made, then extracting it is all you should need to do. Your unzip utility should prompt you to overwrite the existing files. If you do not get that prompt, you are likely not extracting it to the same location it was backed up from.

### Transfer to another PC

Copying a profile to another PC. In order to transfer the backup to another Vixen instance on another PC, you will extract the files to the users My Documents folder as described above. If you are not using multiple profiles in the source or destination, then that will likely just be the Vixen 3 folder inside My Documents and nothing further will be required. If you have multiple profiles, then the profile may need to be configured in the destination instance of Vixen if it is the first time you are copying it over.

### Extracting a Foreign Profile

If you are using a Profile from another user, additional care should be taken to ensure the location of the profile they provided. If they are using a default profile, it may have a folder name of Vixen 3 which is the same as your default profile folder. You do not want to overwrite your default profile which is in My Documents Vixen 3, so when extracting make sure to change the name of the folder it is being extracted to under My Documents.

### Profile Management

If this is the first time the profile has been copied to a PC you will need to establishing the the new profile for Vixen to find it. After extracting the profile, start Vixen up. To do this we want to open the Profile Editor. Depending on how you have it setup, you may see the profile selection screen at startup or not. If you see the profile selection screen at startup, the [Profile Editor][1] can be opened from there. Otherwise, it can be opened from the System => Profiles menu on the main screen.

![Zip Backup Wizard](/images/docs/usage/general/zip-wizard/ProfileSetup.png)

In this screen (shown above) you need to add a new profile and give it a name. Ideally this would be the same name as you used in the source Vixen PC. Then you need to set the Data Folder to the path of where you extracted the profile you copied. This should be in your My Documents folder. In the example above, the path is C:\users\bob\Documents and the profile folder is Small Test. If you used the default path for the profile name on the source machine and named the profile the same on the destination, this may already be correct. Otherwise you can use the file explore to navigate to it. Choose the options to ask you which profile to load, or default to a specific profile and click ok. If you do not choose to ask, then you should select the new profile if you want it to load by default. Vixen will validate that the path entered is correct. If it asks you if you want to create the folder, you have misconfigured the path and should cancel and check the path. You will then need to restart Vixen once the path is correct. Once you restart, then you will either be prompted to choose the profile, or it will load the default profile you chose. You should only need to setup the profile the first time you copy a profile over to establish it. After that, just extracting the backup over the existing profile should work without any changes to the profile setup.

![Zip Backup Wizard](/images/docs/usage/general/zip-wizard/ZipWizard.png)

### Diagnostics

The use shown above is for capturing the entire profile to provide when creating bug ticket that that has requested the profile to help debug the issue. This provides everything that a developer will need to recreate the profile in it; entirely including the logs which may not be in the affected profile if you are using multiple profiles.

 [1]: {{< ref profiles>}}
