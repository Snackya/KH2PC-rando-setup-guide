# KH2FM PC Randomizer Setup Guide
This guide will show you how to get the KH2FM randomizer running with sonic's GoA mod on PC using Topaz's LuaFrontend.

## What you will need
- [LuaFrontend](https://github.com/Topaz-Reality/LuaFrontend/releases/latest)
download LuaFrontend.7z; if you don't have 7zip to extract the archive, you can download it [here](https://www.7-zip.org/download.html)
- the [GoA.lua mod file](https://gist.github.com/1234567890num/1adde394770d5f7f1690493bd0ff7c34)
Click on "Download ZIP" in the top right corner.
- a .pnach randomizer seed file generated on [Valaxor's website](https://randomizer.valaxor.com/#/seed)
Just choose whichever settings you want and click "Download Seed" -> "CrazyCatz..."
- [Num's Rando Converter](https://drive.google.com/file/d/1OLySE7NkXIag3NBnH0J3OukKzk9fdVkl/view)
Converts the old .pnach files to .lua files for LuaBackend

Make sure to extract all of them.

## Creating a seed
You will need a new seed for every new run.  
**Important:** Anything inside Experimental currently does not work with PC Rando. If you create a seed with boss rando, the seed will not work.
1. Get the .pnach seed file from [Valaxor's website](https://randomizer.valaxor.com/#/seed).
2. Drag your .pnach file and drop it onto "Rando Converter.exe".
(Alternatively, you can copy the file into the same directory, launch the .exe and input the file name.)

## Setting up LuaFrontend
1. Open `LuaFrontend.exe`
2. On the left side under "Games:", choose your game. ("[GL]" stands for global here and is usually what you'll want unless you specifically bought the japanese release.)
3. Right-click inside the box on the right under "Scripts:". Then click `Open Script Folder...`. Windows should open that folder in its File Explorer.
4. Copy your script files (GoA.lua and your [seed file](##Creating-a-seed)) into this folder.
5. Right-click inside the right box of LuaFrontend again and click `Refresh List`. Every script you have should now be listed inside the box with a green checkmark icon. If it shows a red X, double click the script to get a detailed error about what the problem is.
6. Click Engine > `Start Engine`.
7. **Optional:** To reduce CPU load on single cores, enable multithreading under Engine > `Enable Multi-Threading`. This will require one logical CPU thread for each script, so make sure your CPU has enough of them. (If you only run GoA and a rando seed file, this option should work for most CPUs).

## Acknowledgments
- [Sonicshadowsilver2](https://github.com/sonicshadowsilver2) for creating the GoA mod.
- [Topaz](https://github.com/Topaz-Reality) for creating LuaFrontend.
- [Valaxor](https://github.com/afresquet) for creating the seed generator.
