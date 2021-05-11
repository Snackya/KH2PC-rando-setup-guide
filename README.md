# KH2FM PC Randomizer Setup Guide
This guide will show you how to get the KH2FM randomizer running with sonic's GoA mod on PC using Topaz's internal LuaBackend.

## What you will need
- [LuaBackend](https://github.com/Topaz-Reality/LuaBackend/releases)
download LuaBackend.7z; if you don't have 7zip to extract the archive, you can download it [here](https://www.7-zip.org/download.html)
- [Rompatcher.js](https://www.marcrobledo.com/RomPatcher.js/)
Website to patch the .exe. Just keep it open in your browser for now.
- the [GoA.lua mod file](https://gist.github.com/1234567890num/1adde394770d5f7f1690493bd0ff7c34)
Click on "Download ZIP" in the top right corner. Alternatively, you can use the direct download link [here](https://gist.github.com/1234567890num/1adde394770d5f7f1690493bd0ff7c34/archive/df9edd1278c53844fc5ed6826cffa6e329698140.zip)
- a .pnach randomizer seed file generated on [Valaxor's website](https://randomizer.valaxor.com/#/seed)
Just choose whichever settings you want and click "Download Seed" -> "CrazyCatz..."
- [Num's Rando Converter](https://drive.google.com/file/d/1OLySE7NkXIag3NBnH0J3OukKzk9fdVkl/view)
Converts the old .pnach files to .lua files for LuaBackend

Make sure to extract all of them.

## Setup
For setting up the randomizer for PC, you have two options: external or internal.

| LuaBackend method                             | Internal | External |
|-----------------------------------------------|----------|----------|
| requires modifying the game .exe              |  yes     |   no     |
| requires running LuaBackend.exe on every run  |  no      |   yes    |

You will only have to do this setup once.

### Method A) Internal
The internal approach requires you to patch your KINGDOM HEARTS II FINAL MIX.exe.

#### Patching the KH2FM.exe
1. **Important:** Backup your original "KINGDOM HEARTS II FINAL MIX.exe".
2. Open up the Rompatcher.js website.
3. Under "ROM file", click "Choose File" and select your KINGDOM HEARTS II FINAL MIX.exe inside your game directory.
4. Under "Patch file" click "Choose File" and select the KINGDOM HEARTS II FINAL MIX.bps inside LuaBackend/Internal/patches.
5. Click "Apply patch" and save the resulting .exe file as "KINGDOM HEARTS II FINAL MIX.exe" into your game directory.

#### Setting up scripts
1. Create a folder called "scripts" inside Documents/KINGDOM HEARTS HD 1.5+2.5 ReMIX
2. Copy the FAF99301 GoA.lua into the scripts folder.

### Method B) External
The external approach does not modify game files. However, you will need to start an additional program every time you start your game for a randomizer run.

#### Setting up LuaBackend.exe
1. Open your LuaBackend/External folder.
2. Copy the KINGDOM HEARTS II FINAL MIX.ini from the "preset_configs" folder into the "External" folder, next to LuaBackend.exe.
3. Rename KINGDOM HEARTS II FINAL MIX.ini to "config.ini".
(If you cannot see the .ini file extension, just rename it to "config")
4. (Optional) If you want to change the refresh rate of the Backend, open "config.ini" and add “REFRESH = 240" on a new line at the bottom of the file. Viable values are 60, 120, 240.

#### Setting up scripts
Just copy all your .lua files into LuaBackend/External/scripts

## Creating a seed
You will need a new seed for every new run.
1. Get the .pnach seed file from [Valaxor's website](https://randomizer.valaxor.com/#/seed).
2. Drag your .pnach file and drop it onto "Rando Converter.exe".
(Alternatively, you can copy the file into the same directory, launch the .exe and input the file name.)
3. Copy the FAF99301.pnach.lua into the "scripts" folder you created before.

## Finally
Run your "KH2FM Randomizer.exe".

## Acknowledgments
- [Sonicshadowsilver2](https://github.com/sonicshadowsilver2) for creating the GoA mod.
- [Topaz](https://github.com/Topaz-Reality) for creating LuaBackend.
- [Valaxor](https://github.com/afresquet) for creating the seed generator.