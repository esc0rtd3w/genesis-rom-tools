                               SonED .14B/.16B

Thankyou for downloading SonED. I hope that you opened this text file
by yourself, but if an error has been made in starting the program,
you will be sent here automatically so that you may look for the
solution to your problem.

Note: Included with SonED are Microsoft's expand and compress
      (expand.exe and compress.exe). These files are to enable
      SonED to read and write the .cm_ files in Sonic CD PC.

This demo of SonED shows the functionality of the current full version.

SonED.exe  is release .14B
SonED2.exe is release .19B

The two utilities will become one again once I create a means of selecting
whether you want to edit the ROM or Save-State.

When editing ROMs, you must still load a Save-State. This is how you select
the level you want to edit, and also where the art for viewing the level
comes from. Currently, you can only edit Level Layout in the ROM. This
eliminates the need to download bulky art sets. Although you can change the
art within the editor, it cannot be saved into the ROM because I do not have
the information to do so. The altered art will only be saved when you are
editing the level within a Save-State.

As of release .14B, you can alter object placement (binary), palette colors
(binary/save-state), level layout(save-state), and 8x8, 16x16, and
128x128/256x256 tiles (save-state) for Sonic 1, 2, and 3K. You may also
do the same with Sonic CD PC (both OEM and DirectX versions), however,
you cannot change the palette in that game.

Release .16B functions in the same manner as .14B, with a few exceptions.
Firstly, the level layout for Sonics 1, 2, and 3K are loaded directly from
the ROM, and if you are a registered user, they are also saved back to the
ROM. In this release, you may also edit the player starting positions. Also,
this release will automatically disable the checksum on Sonic 1 so that the
edited ROM will not crash upon startup.

Release .19B is an upgrade to .16B. Release .19B will read and write 8x8 tile
art and both 16x16 and 128x128 tile mappings for Sonic 2 through the ROM.
(Writing back to the ROM is only available for registered users.) This release
also brings another feature to registered users, which allows them to create
image files containing maps of the current levels. Images can be dumped from
any individual plane, or from both High and Low plane of A or B at the same
time.

Many other features will be added through the course of development. Please
visit Organized Chaos (http://stealth.emulationzone.org/) for specifics on
these, for contact and ordering info, and for any current events.

Note again, this editor is -NOT- complete, so some features you want
may not be implemented yet. I'll be getting to them though, so don't
worry.

Also, in this demo release, the saving of your work is not allowed.
Sorry, I really need the money from the registration fee. You may
however view any altered or unaltered data within the editor and play
around with it to get the feel of the editor's current state.

Also, supplied with this editor is an example of an edited level.
You must apply the IPS patch to an unaltered Sonic 1 ROM and give
the resulting file the name "funky.bin" for the example to work.

NOTE: The example is only a level layout and object hack for Sonic 1
      and does not reflect any other features of the editor.

How to use this program:

Before you attempt to run the program, you must have the file
DOS4GW.exe in your windows folder (or any other folder that is
named in the "path" statement within your autoexec.bat file).
It -can not- be in the same folder as the editor, or else it
will not run correctly.

Also in this version is a graphical loading interface, which
replaces the command line requirements of previous versions. Simply
type the program's name (SonED) at the command line or double-click it
within windows, and it will prompt you to load a ROM and Save-State, or
(in the case of Sonic CD PC) find the exe (example: SonicCD.exe) for the
PC game you wish to edit.

All you need to do from here is select the game you will be loading for,
find the ROM using the file menus, and then select the Save-State file
in the same manner. In the case of SonicCD, you will notice that the
file menu changes. You will need to select the zone, act, and time you
wish to edit, select your version of Sonic CD, and then find SonicCD.exe
and click on it, then click OK. The OEM version of SonicCD was distributed
with new PC's and does not use DirectX. The DirectX version was the retail
version you may have bought in a store. If you are unsure which version
you have, just chose one and if it doesn't work, quit and chose the other.

When loading another file during use of the program, you will notice that
the file filter is set to *.*, and the load type is set to "general".
This will let you view all files within the folder, and will load the
file for general use (NOTE: general use files are useless in this version)
You may select the filter to view only certain types of files for ease of
access, and you must set the load type for the type of file it is (ROM or
Save-State) so that SonED will recognize it, and begin to let you edit it.

With that said, you need to know how to use the editor on the inside.
For switching between editors, you may use the Gui. To activate the menu,
just click the right mouse button. You may also use the old keyboard
shortcuts to move between editors. The following is a list of commands:

The cursor is controlled with the mouse, and can be used to move objects,
show the editor which object you are editing with the keyboard, and draw
onto the level map. The keys are as follows:

A/Z:      Change value 1 (Object Type) on the selected object.
          Also for Ring formations in Sonic 2 and up.
S/X:      Change value 2 (Object Property) on the selected object.
D/C:      Change value 3 (Object Property 2) on the selected object.

(Sonic CD has two extra object properties that the other games don't.)
(These may control what time zone the object appears in.)
G/B:      Change value 4 (Object Property 3) on the selected object.
H/N:      Change value 5 (Object Property 4) on the selected object.

F/V:      Change grid snapping for precision object placement.

P:        Switch between object editor and level map editor.

G:        (G)rab the 128x128/256x256 tile under the curor.
Alt/Ctrl: Change current selected 128x128/256x256 tile for drawing.

O:        Switch between tile/mapping/palette editor and object editor.

Esc:      Exit the program.

Within the tile editor, there are a few options that can be changed with
the arrows on the screen. The tiles may also be selected by the following
keyboard keys:

A/Z:      Change 8x8 tile.
S/X:      Change 16x16 Tile.
F/V:      Change 128x128/256x256 Tile.
Arrow Key:Move around the 256x256 tile within the 128x128 window.

Note:     The tile selection screens are not yet implemented, so you
          have to use the arrows or the keypresses described above.

Also, while in select mode, you may click part of a larger tile with the
right mouse button to select the smaller tile within it for editing. The
left button will only select the part of the larger tile who's attributes
you want to edit. In draw mode, the left button will draw onto the tile
you are pointing at. The 8x8 tile is displayed in the set of colors
currently selected by the color selector. Bear in mind that it can only
use colors from one set. As for the palette selector, the top four rows
are the above-water colors, and the bottom four are the below-water
colors, which can't be selected unless the level actually does have water.
You may alter the currently selected color by using the arrows beside the
R, G, and B just below the palette. And on a final note, the "T" is for
Transparant.

That's about it.

This program was written by Stealth. (MstealthA@aol.com)

Thanks go to Saxman/Rocket (saxman@shentel.net) for his trememdous
contribution in the "Sonic 2 Hacking Guide"
(http://ssrg.emulationzone.org/s2hack)

Thanks also to Brett Kosinski (brettk@gpu.srv.ualberta.ca) for cracking
the Sonic 2 level compression, and explaining to me how it works.



You may also want to check out Sonic Hacking Wiz Pro, which makes a great
companion program with SonED. It can edit level select layout, level title
cards, and more. It can be found at the Gerbil Software homepage at:

http://ssrg.emulationzone.org/gerbil
