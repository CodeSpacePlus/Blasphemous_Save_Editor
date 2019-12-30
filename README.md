# Blasphemous Save Editor

Save editor for the game Blasphemous by The Game Kitchen

### Instructions for v2.0

The way you load your save or json file is pretty identical to the previous version of this application but now you're free to add and remove relics, hearts, beads, prayers, even modify your permanent buffs.

- Load the file you wish to edit (clicking `Load`), or create one by click `New`, the navigation bar will unlock and you'll be able to freely edit the save file.

- Navigating to the different tabs will indicate which items you already own or have equipped. To add new items simply click on the `owned` checkbox (`obtained` when adding new skills), try not to _unowned_ an item you have equipped I have no clue what could this cause<sup>[1]</sup>. To edit your current values or permanent buffs simply edit the text box with the stat you want to modify\*\*.

  - **\*\*NOTE:** These effects haven't been tested to its fullest editing these values could cause adverse effects to the gameplay.

- When you're done modifying your game click on `Save as...` you will be asked to select a folder where your file will be stored.

- Next type in the file name (**_Blasphemous only recognizes `savegame_0, savegame_1, savegame_2` you will have to change it's name later if you want the game to recognize it_**) and select in which format you'll want to save your game.

- Click on `save` will generate your file now you can share it or move it to save files folder of the game `AppData/Locallow/TheGameKitchen/Blasphemous/Savegame/[random series of numbers]/`.

- **Please remember to always backup your original save to prevent progress lost.**

## Known issues and untested events

- **Issue -** For some reason when you give yourself any of the combo moves (`Last Words`, `Ascending Edge`, `Azure Cyclone`) these don't work correctly while it is registered on your skill tree and the other skill work without any issue<sup>[2]</sup>.

- **Bug -** Yes I'm aware some of the beads of wax don't have an image and as well as `Marked Bead`, `Tainted Bead`, and `Weight of true Guilt`. I'll work on these later.

- **Untested -** Picking up and item you already own could do one of three things:

  - Crash the game (worst case scenario)
  - Duplicate the item (not too bad maybe try equipping both?)
  - Nothing (the event flag triggers<sup>[3]</sup>)

- **Untested -** Play the edited game (basically I just tested if the game could load correctly which it has so far)

## TODO

- <sup>[1]</sup>Unequip items that are removed and equip items using the editor.
- <sup>[2]</sup>Figure out how to make the combo work propperly. Missing event maybe?
- <sup>[3]</sup>Add the event flag for every item added

## Future plans

- Add collectibles
- Add quest items
- Teleport to different locations
- Trigger achievements (if I don't get in trouble)

## What I'd love to be able to do but I doubt it will happen

- Edit enemy stats (hp, damage output, etc)

### These are the instructions for the v1.0 of this tool and could change on future versions.

This is a pretty straight forward save editor. Here's the break down:

- Click on load and browse to your .save file. If you're on windows it should be located in your `AppData/Locallow/TheGameKitchen/Blasphemous/Savegame/[random series of numbers]/`

- Once you have open your file it should convert and load everything inside the larger textbox. You can either edit the file directly from here or save it as a json file and edit it using [notepad++](https://notepad-plus-plus.org/downloads/), [vscode](https://code.visualstudio.com/download), [sublime](https://www.sublimetext.com/3), etc.

- If you choose to modify it using another text editor you can take that modified json file and load it just as you did with the .save file. It will load your json data in the textbox as it would with a .save file.

- When you're done modifying it click on save as .save, there should be a **_savegame_0(Modified).save_** on the same folder where you ran the .exe

- Backup your initial save (just to be safe) and drag your modified file onto your blasphemous savegame folder and rename it so that the game can recognize it.

- Run your game and you're done.
