# AES-Key-Extracting-Guide
- This tutorial will go through the steps on how toi extract an UE4/UE5 AES-256 Key.
- And also how to use it in extracting the *.pak* file in the "contents" folder.
- This *DOES* work with [Steam](https://store.steampowered.com/) & [Epic](https://store.epicgames.com/en-US/download) *However sometimes Epic-bought games are weird*.


# Before We Begin:
- I am *NOT* resposible for how you the keys you will find while using the guide.
- This was made for modding purposes *ONLY*.

# Software Needed:
- [UEViewer](https://www.gildor.org/en/projects/umodel#files) - For Viewing and Extracting Files.
- [Steamless](https://github.com/atom0s/Steamless/releases/tag/v3.1.0.0) - For Removing the SteamStub/Steam DRM Restrictions on the *Shipping.exe*.
- [AES Key Finder](https://github.com/Cracko298/AES-Key-Extracting-Guide/files/9074659/AES.Key.Finder.zip) - For Finding AES Keys in the DRM-less *Shipping.exe*.
- [FModel](https://fmodel.app/) - You can use this too mod your Games. (However I will not go into detail on this).

# Guide:

# Step 1 (Getting rid of the DRM restriction):
- Firstly open/run [Steamless](https://github.com/atom0s/Steamless/releases/tag/v3.1.0.0) to get rid of the DRM restrictions on your *Shipping.exe* file.
- Too access your *Shipping.exe* file(s) go into "[Steam](https://store.steampowered.com/) > Library > *Your Game*". Right click on *Your Game's Name* and go into "Manage > Browse Locale Files"
- The file explorer should have opened *probably in the background*. Go into "*Your Game Name Folder* > Binaries > Win64/32".
- Paste the directory link into [Steamless](https://github.com/atom0s/Steamless/releases/tag/v3.1.0.0), or find the *Shipping.exe* directory in the "browse" button.
- Hit the extract button in [Steamless](https://github.com/atom0s/Steamless/releases/tag/v3.1.0.0) it'll take a few second(s)/minute(s).
- The newly created *.exe* file is the DRM-LESS game.

# Step 2 (Finding the AES keys):
- Secondly you'll need the [AES Key Finder](https://github.com/Cracko298/AES-Key-Extracting-Guide/files/9074659/AES.Key.Finder.zip) to find the AES-256 Keys.
- Take the newly created *DRM-LESS Shipping.exe* file and copy it into the [AES Key Finder](https://github.com/Cracko298/AES-Key-Extracting-Guide/files/9074659/AES.Key.Finder.zip) folder which you extracted from the *AES.Key.Finder.zip* file.
- Open/run the *.bat* file called *RUN Find 256-bit UE4 AES Key.bat* this will find all keys it can recover from the DRM-LESS *Shipping.exe*.
- After the *RUN Find 256-bit UE4 AES Key.bat* file has ran. Their should be 1-6 folders. Only one of them contains the AES-256 key.
- The folder(s) are just a few bits/bytes of the key. The file name inside of the folder *IS* the AES-256 key.

# Step 3 (Extracting the Encrypted *.pak* file):
- Last of all you'll need [UEViewer/Umodel](https://www.gildor.org/en/projects/umodel#files) to extract/save the game's file(s).
- As always extract the *.zip* and open/run the application. For simplicity we'll copy the *.pok* file to the newly extract *Umodel* folder.
- Too access your game in [Steam](https://store.steampowered.com/) *again if you closed it* go to "[Steam](https://store.steampowered.com/) > Library > Your Game > Right Click Name > Manage > Browse Locale Files".
