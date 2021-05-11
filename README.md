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
You will only have to do this setup once.
### Patching the KH2FM.exe
1. **Important:** Backup your original "KINGDOM HEARTS II FINAL MIX.exe".
2. Open up the Rompatcher.js website.
3. Under "ROM file", click "Choose File" and select your KINGDOM HEARTS II FINAL MIX.exe inside your game directory.
4. Under "Patch file" click "Choose File" and select the KINGDOM HEARTS II FINAL MIX.bps inside LuaBackend/Internal/patches.
5. Click "Apply patch" and save the resulting .exe file as "KINGDOM HEARTS II FINAL MIX.exe" into your game directory.

### Setting up scripts
1. Create a folder called "scripts" inside Documents/KINGDOM HEARTS HD 1.5+2.5 ReMIX
2. Copy the FAF99301 GoA.lua into the scripts folder.

## Creating a seed
You will need a new seed for every new run.
1. Get the .pnach seed file from [Valaxor's website](https://randomizer.valaxor.com/#/seed).
2. Drag your .pnach file and drop it onto "Rando Converter.exe".
(Alternatively, you can copy the file into the same directory, launch the .exe and input the file name.)
3. Copy the FAF99301.pnach.lua into the "scripts" folder you created before.

## Finally
Run your "KH2FM Randomizer.exe".