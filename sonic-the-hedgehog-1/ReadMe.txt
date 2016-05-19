                    SonED for Windows.50B

Thank you for downloading SonED for Windows.

Features as of this release:

- Edit Object Placement for Sonic 1, 2, 2 "beta", and 3K (ROM), and Sonic CD PC
- Edit Level Layout for Sonic 1, 2, 2 "beta", and 3K (ROM/Save-State), and Sonic CD PC
- Edit Palettes for Sonic 1, 2, 2 "beta", and 3K (ROM), and Sonic CD PC
- View PCX image as guide when editing Palettes not related to level tiles
- Edit Tiles and Mappings for Sonic 2 (ROM)
- Edit Tiles and Mappings for Sonic 1, 2 "beta" and 3K (Save-State)
- Edit Tiles and Mappings for Sonic CD PC (Game Files)
- List style tile selection in Tile Editor mode
- Dump PCX image map of the current level
- Read/Write menu system for ease of access to data and "swapping"
  (Please read lower in this text for instructions on saving your work)
- Object Listing Scripts in which descriptions and images of objects
  can be placed and called into the editor (Please pay very close
  attention to the section descriptions, as breaking the format will
  cause SonED to crash, and you will need to get a clean list file)
- All Genesis ROM formats are supported in loading and saving
- Fixes ROM header info (checksum and size) during saving

To keep up with current updates, please visit the Organized Chaos site:
http://stealth.emulationzone.org/SonED
The official SonED download page is located here:
http://stealth.emulationzone.org/SonED

Also, supplied with this editor is an example of an edited level.
The IPS patch must be applied to an unaltered Sonic 1 ROM and give
the resulting file the name "funky.bin" for the example to work.
This patch may be applied with StealthPatch, an IPS patcher included
with SonED, or any other IPS patcher program.

NOTE: The example is only a level layout and object hack for Sonic 1
      and does not reflect any newer features of the editor.

How to use this program:

All that's required to run this program is to store it with the correct
data files (included in the zip) and double-click it.

When the program first starts, an "Open File" dialogue is presented,
requesting the name of the desired ROM. Once a ROM is selected, a
save-state must also be loaded for games who's data can't be loaded
from the ROM (Sonic 2 and Sonic CD PC do not require save-states).
The save-state must be an in-level save-state of the level you'll
want to be editing. Anything else will not work properly.

The initial load attempts to automatically load everything from the
selected ROM, which will bring up some "error messages" on some games
which can be ignored. The data will then automatically be loaded from
the selected save-state. These messages serve as a reminder for the
manual save and load functions that will be available once the editor
starts. ROMs and Save-States may be loaded separately then as needed.

To load Sonic CD (for PC) instead, you'll need to find and select
"soniccd.exe". It must be in the Sonic CD full installation folder,
and every file must still be in it's original position. If any files
have been moved or swapped, this will cause errors.

With that said, you need to know how to use the editor on the inside.
For switching between editors, just use the Editors dropdown menu at
the top of the window, or use these hotkeys:

I:        Tile/Palette Editor
O:        Object Editor
P:        Level Layout Editor

The following is a list of other commands for each editor:

OBJECT TEDITOR:
The cursor is controlled with the mouse, and can be used to move objects,
show the editor which object you are editing with the keyboard, and draw
onto the level map. The keys are as follows:

A/Z:      Change value 1 (Object Type) on the selected object.
          Also for Ring formations in Sonic 2 and up.
S/X:      Change value 2 (Object Property) on the selected object.
D/C:      Change value 3 (Object Property 2) on the selected object.

CTRL:     Hold while pressing any of the above to scroll by 16 instead of 1

Q:        Press while hovering the mouse over an object to enter the object
          type listing, which lists the descriptions (and art if available)
          of objects listed in the current "Object Def" file for easy
          selection. Selecting a new type with the left mouse button will
          change the selected object to an object of that type. Clicking the
          right mouse button will go back to the object editor without changing
          the object. The list is in numeric order of object type IDs.

F/V:      Change grid snapping for precision object placement.

H/B:      Change the keyboard scrolling speed.

Arrows:   Scroll across the map.


LEVEL TEDITOR:
The cursor is controlled with the mouse, and below it is shown the
currently selected tile. This tile may be transluscent so that you can
see what's under it, or opaque, for faster rendering. The Left Mouse
button draws it onto the level map. The keys are as follows:

G:        (G)rab the 128x128/256x256 tile under the curor.

U:        Undo up to the last 20 modifications made in the Level Editor.

A/Z:      Change current selected 128x128/256x256 tile for drawing.

H/B:      Change the keyboard scrolling speed.

Arrows:   Scroll across the map.


TILE/PALETTE TEDITOR:
The cursor is controlled with the mouse, and it allows you to draw to
the tiles and mappings by clicking within the appropriate "sub-windows",
as well as selecting the various on-screen controll options. The Left
mouse button is used for drawing and clicking options, and the Right
is for selecting smaller tiles within larger ones. The keys are as 
follows:

A/Z:      Change current selected 8x8 tile
S/X:      Change current selected 16x16 tile
D/C:      Change current selected 128x128 tile


SAVING YOUR WORK:

When you are ready to save your progress, you must bear in mind that
there are two steps to this. First, you will have to use the "Write"
menus to save your work to the ROM, and then you will need to use
the "Save" feature to save the ROM to the disk. If you do not "Write"
before saving, an unaltered ROM will be saved to disk, and if you do
not "Save" after "Writing", your work will not be reflected in the 
on-disk file. This is very simple once you get used to it, and 
convenient in the ways of rearranging data, editing multiple pieces
in one session, and taking advantage of the ability to Save without
"Write"ing the newest altered data in-case you want to do away with
the most recent changes. In the case of Sonic CD PC, however, the
write menu options write directly to the files themselves.

An alternative to the above method is the "Quick-Save" shortcut.
By pressing F3 at any time, a "Write->ROM->All" will be performed,
and the ROM itself will be saved to disk at the same location it
was loaded from. This option writes to the last level that was
loaded with either a "Read->ROM->All" or through a save-state. If
other methods were used to load certain data from a different level,
that level will not be the target during the save. It also ignores
data that cannot be written to the ROM, and will not display warning
notices for that data.

Sonic 1 and Sonic 2 data can also be exported to individual files in
the same format in which they're stored in the ROMs, so that their
placement can be managed manually when SonED's automatic placement
isn't sufficient. The filenames are chosen automatically and are
preceded by "S1" or "S2" to signify the game they belong to, and the
files will appear in the SonED folder. Any previously dumped data from
either game will be overwritten by the next dump, so it must be copied
first. No other games are currently supported by this function.

IMPORTANT SONIC 2 NOTE:

The level and tile data for Sonic 2 are moved to the end of the ROM so
that they have room to grow as necesary, because when editing compressed
data, the size will almost always change. The first time SonED is used
on any one Sonic 2 ROM, the level data will be moved to the current end
of the ROM. If another program that does something similar was used first,
this data will appear after it's data. Otherwise, it will appear at
address 0x00100000 (the old end of the ROM). If a different editor was
used after SonED, it's data will likely appear after the level data at
the end of the ROM. This can cause problems, because if the level/tile
data grows, it will overwrite the other data. To avoid this, you must
either use (and if possible, finish the use of) other editors before
using SonED, or, pad the ROMsize after using SonED on that ROM for the
first time. Padding the ROM can set asside enough room for data created
by SonED to grow/shrink without overwriting other data if the proper
ammount of space is set, and if the other programs are flexible enough
to write their data at the end of the padding instead of picking a
predetermined location. To pad the ROM, open it in a hex editor, and
insert a number of bytes at the end of the file. This number must be
equal to or greater than the number of bytes that the data is expected
to grow. The total size of level/tile data will stay around the area of
524,288 bytes (512K). Adding 131,072 bytes (128K) to the end might leave
enough room, although a larger number would be safer.

MENUS RUNDOWN:

 File-
   Load-
     ROM-               This option will allow you to load the current
                        ROM image from disk.
     Save-State-        This option will allow you to load the current
                        Save-State from disk.
     PC Game-           This is a currently unimplemented option for
                        future supported games.
   Save-
     ROM-               This option will allow you to save the current
                        ROM image to disk.
     Save-State-        This option will allow you to save the current
                        Save-State to disk.
     PC Game-           This is a currently unimplemented option for
                        future supported games.
   Read Data-
     ROM-
       Palette-         This menu lists the palettes available for
                        this game.
       Objects-         This menu allows you to select the level who's
                        object layout you want to load.
       8x8 Tiles-       This menu allows you to select the level who's
                        8x8 Tiles you want to load.
       16x16 Tiles-     This menu allows you to select the level who's
                        16x16 Tiles you want to load.
       128x128 Tiles-   This menu allows you to select the level who's
                        128x128 Tiles you want to load.
       Level Layout-    This menu allows you to select the level who's
                        level layout you want to load.
       All-             This menu allows you to select the level who's
                        entire data set you want to load.
     Save-State-
       Palette-         This option loads a palette from the current
                        save-state (not yet implemented)
       8x8 Tiles-       This option loads 8x8 tiles from the current
                        save-state
       16x16 Tiles-     This option loads 16x16 tiles from the current
                        save-state
       128x128 Tiles-   This option loads 128x128 tiles from the current
                        save-state
       Level Layout-    This option loads level layout from the current
                        save-state
       All-             This option loads all above data from the current
                        save-state
   Write Data-
     ROM-
       Palette-         This menu lists the palettes available for
                        this game.
       Objects-         This menu allows you to select the level who's
                        object layout you want to Store.
       8x8 Tiles-       This menu allows you to select the level who's
                        8x8 Tiles you want to Store.
       16x16 Tiles-     This menu allows you to select the level who's
                        16x16 Tiles you want to Store.
       128x128 Tiles-   This menu allows you to select the level who's
                        128x128 Tiles you want to Store.
       Level Layout-    This menu allows you to select the level who's
                        level layout you want to Store.
       All-             This menu allows you to select the level who's
                        entire data set you want to Store.
     Save-State-
       Palette-         This option stores a palette to the current
                        save-state (not yet implemented)
       8x8 Tiles-       This option loads 8x8 tiles to the current
                        save-state
       16x16 Tiles-     This option stores 16x16 tiles to the current
                        save-state
       128x128 Tiles-   This option stores 128x128 tiles to the current
                        save-state
       Level Layout-    This option stores level layout to the current
                        save-state
       All-             This option stores all above data to the current
                        save-state
     File-              This submenu exports data for supported games to
                        individual files for manual management
   Exit-                This option exits the editor

 Editor
   Tile Editor-         This option switches to the Tile Editor
   Object Editor-       This option switches to the Object
   Level Editor-
     Plane A-           This option allows you to edit the "foreground"
     Plane B-           This option allows you to edit the "background"
   Visibility-
     Status-            Toggle the status elements in the various editors
     Plane Low-         Toggle "low" plane when viewing level and tiles
     Plane High-        Toggle "high" plane when viewing level and tiles
     Objects-           Toggle objects view in level layout editor
     Trans. Cursor-     Toggle translucency on the tile cursor

 Misc-
   Load PCX Image-      Load an image to be displayed in the palette
                        editor for reference while editing the colors.
   Dump Layer-
     Plane A High-      Dump a PCX map of "high" plane of the "foreground"
     Plane A Low-       Dump a PCX map of "low" plane of the "foreground"
     Plane A High and Low- Dump a PCX map of the full "foreground"
     Plane B High-      Dump a PCX map of "high" plane of the "background"
     Plane B Low-       Dump a PCX map of "low" plane of the "background"
     Plane B High and Low- Dump a PCX map of the full "background"

 Help-
   Contents-            This option is currently unimplemented.
   About-               Display the credits box.


If you have any questions, comments, or want to make a contribution, feel free
to contact me at MStealthA@aol.com.
