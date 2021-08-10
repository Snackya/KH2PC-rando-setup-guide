# KH2FM PC Randomizer Setup Guide
This guide will show you how to get the KH2FM randomizer running with sonic's GoA mod on PC using Topaz's LuaFrontend.

## What you will need
- DINPUT8.zip from [LuaBackend Hook](https://github.com/Sirius902/LuaBackend/releases/latest)
- the [GoA.RAM.lua mod file and Rando converter](https://github.com/1234567890num/Garden-of-Assemblage-Mod-Lua/releases/latest)
- a .pnach randomizer seed file generated on [Valaxor's website](https://randomizer.valaxor.com/#/seed)
Just choose whichever settings you want and click "Download Seed" -> "CrazyCatz..."

Make sure to extract all of them.

## Creating a seed
You will need a new seed for every new run.  
**Important:** Anything inside Experimental currently does not work with PC Rando. If you create a seed with boss rando, the seed will not work.
1. Get the .pnach seed file from [Valaxor's website](https://randomizer.valaxor.com/#/seed).
2. Open `converter.html` inside your extracted Rando Converter folder in your web browser (just double click it).
3. Follow the instructions on the web page.

## Setting up LuaBackend Hook
1. Copy `DINPUT8.dll` from the `DINPUT8` folder (LuaBackend Hook download) to the location of your `KINGDOM HEARTS II FINAL MIX.exe`
2. Create a folder called `scripts` inside `Documents\KINGDOM HEARTS HD 1.5+2.5 ReMIX`
3. Copy your scripts (`GoA.RAM.lua` and your seed .lua file) into the newly created `scripts` folder
4. Done. You can now run your game regularly. To see if the LuaBackend Hook is working, press the F2 key in game to open its console.  
 
Note: LuaBackend Hook will run with every game launch now. To uninstall it, just delete `DINPUT8.dll`.

## Acknowledgments
- [Sonicshadowsilver2](https://github.com/sonicshadowsilver2) for creating the GoA mod.
- [1234567890num](https://github.com/1234567890num) for all his contributions to KH2 modding.
- [Sirius902](https://github.com/Sirius902/LuaBackend) for maintaining LuaBackend Hook.
- [Valaxor](https://github.com/afresquet) for creating the seed generator.
