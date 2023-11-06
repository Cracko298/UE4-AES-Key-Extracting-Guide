[![paypal](https://github.com/Cracko298/ISZ-2021-Plugin/blob/main/payp.png)](https://www.paypal.me/cracko298)

# AES-Key-Extracting-Guide
- This tutorial will go through the steps on how to extract an UE4/UE5 AES-256 Key.
- And also how to use it in extracting the *.pak* file in the "contents" folder.
- This *DOES* work with [Steam](https://store.steampowered.com/) & [Epic](https://store.epicgames.com/en-US/download) *However sometimes Epic-bought games are weird*.
- This guide does *NOT* include a guide for [Linux](https://www.linux.org/) users, or [MacOS](https://www.apple.com/in/macos/monterey/) users.

# Before We Begin:
- I am *NOT* resposible for how you use the keys you will find while using this guide.
- This was made in the thought of extracting files for modding purposes *ONLY*.

# Software Needed:
- [UEViewer](https://www.gildor.org/en/projects/umodel#files) - For Viewing and Extracting Files.
- [Steamless](https://github.com/atom0s/Steamless/releases/tag/v3.1.0.0) - For Removing the SteamStub/Steam DRM Restrictions on the *Shipping.exe*.
- [AES Key Finder](https://github.com/Cracko298/AES-Key-Extracting-Guide/files/9074659/AES.Key.Finder.zip) - For Finding AES Keys in the DRM-less *Shipping.exe*.
- [FModel](https://fmodel.app/) - You can use this too mod and view Assets your Games. (However I will not go into detail on this *arguably better than Umodel).
- [UE4 Mod Unlocker](https://illusory.dev/).

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
- After the "RUN Find 256-bit UE4 AES Key.bat" file has ran. Their should be 1-6 folders. Only one of them contains the AES-256 key.
- The folder(s) are just a few bits/bytes of the key. The ***file name*** inside of the folder *IS* the AES-256 key.

# Step 3 (Extracting the Encrypted *.pak* file):
- Last of all you'll need [UEViewer/Umodel](https://www.gildor.org/en/projects/umodel#files) to extract/save the game's file(s).
- As always extract the *.zip* and open/run the application. For simplicity we'll copy the *.pok* file to the newly extract [Umodel](https://www.gildor.org/en/projects/umodel#files) folder.
- Too access your game in [Steam](https://store.steampowered.com/) *again if you closed it* go to "[Steam](https://store.steampowered.com/) > Library > Your Game > Right Click Name > Manage > Browse Locale Files".
- As normal, file explorer should start in the background. Open the new tab, and navigate to "*Your Game Name* > Content > Paks".
- You should have at least 1 *.pak* file(s). It's normally the biggest one however, it depends on the game.
- Copy the *.pak* file and paste it into the [Umodel](https://www.gildor.org/en/projects/umodel#files) folder.
- Open/run [Umodel.exe](https://www.gildor.org/en/projects/umodel#files) and select all that you want to extract/save. Make sure to choose the game version.
- You can find the game version by right clicking *Shipping.exe* and then going into "Properties > Details".
- After you find your game version. [Umodel](https://www.gildor.org/en/projects/umodel#files) will come up with an AES-Encryption Window.
- Paste the AES-256 Keys into the AES-Encryption Window. Adding a line for each key you would like to try.

# Note(s):
- If you ***NEED*** the game version. *Right-Click* the original *Shipping.exe* and navigate to: *Properties > Details > File Version* that's your game version.
- If unsuccessful, you're probably using a non-Steam *.pak* file, or you have an unsupported version of UE. (Possibly UE3, or UE2).
- If successful you've just cracked the *.pak* file.
- Only works with *Win32* and *Win64* executables, (***.exe Only*!**) (***Not*** *.msi*, *.com*, *.bat*, or  *.cmd*).
- This guide does ***NOT*** work for *MacOS* or *Linux* games. That also includes *Nintendo Switch*, *Playstation Consoles*, and *Xbox Consoles*, (Obviously).

# Credits:
- Congrats! You've completed the tutorial, and now know how to extract AES-256 Keys from [UE4](https://unreal.fandom.com/wiki/Unreal_Engine_4) and possibly some [UE5](https://docs.unrealengine.com/5.0/en-US/hardware-and-software-specifications-for-unreal-engine/) games.
- Maybe consider giving me a [Follow](https://github.com/cracko298), possibly a [Golden-Star](https://github.com/Cracko298/UE4-AES-Key-Extracting-Guide/stargazers) or even a [Fork](https://github.com/Cracko298/UE4-AES-Key-Extracting-Guide/fork). Anything helps out!
- And, Thanks too everyone who supports me, it really helps. - [Cracko298 (Phinehas Beresford)](https://github.com/Cracko298)
- Hey! I made a new thing for UE4 games. This time, it isn't a guide. [UE4-FOV-Editor](https://github.com/Cracko298/UE4-FOV-Editor). ***Note: This ain't revolutionary.***

### Extra Notes:
- I accept donations if you want to help me out (No need too, this guide will ALWAYS be avaliable for free). This is via [PayPal](https://www.paypal.me/cracko298) if you want to donate.
- All software mention lead to the original repo's please consider supporting those developers.

# Software:
- [Glidor](https://github.com/gildor2) for The UE4 viewing and extracting tool UEViewer.
- [Atom0s](https://github.com/atom0s) for Steamless.
- [GHFear](https://github.com/GHFear) for The AES Key Finder & UE4 Mod Unlocker.
- [4sval](https://github.com/4sval) for The UE4/UE5 viewing tool FModel.
