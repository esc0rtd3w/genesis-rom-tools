                              StealthPatch V1.4

What's New:

v1.4
Another BugFix. There was a problem that would cause the program to crash
immediately upon startup in Windows XP, and sometimes even in ME and 2K.
This has been fixed.

v1.3
Bugfix. If there was a string of different data that exceded 0xFFFF (65536)
bytes, the 65536'th byte would be ignored, thus causing part of the change
to not take effect. This would especially cause problems when adding excess
data into the patch itself. This has been taken care of, so now extremely
long strings of data changes/additions should not get corrupted.

v1.2
The protection idea sprang to mind when I tried to apply a patch created
from an unclean file to a clean file, however, I've found a patch for a
different file which expands the file while patching it, so I've taken out
the warning against patches that try to do that, and accomodated for them.
This program can now add excess data into the patch, or can still create
a new file for it (you will be prompted to choose if it is necesary). Some
other patchers will allow this, while some won't. Also, I've taken the DOS
call to "attrib" out of the file system, as apparantly it causes problems
with certain Windows systems under certain circumstances, and it's not
really necesary anyway. So if you were having problems concerning DOS, they
won't be happening anymore.

v1.1
Decided to add protection against using improper IPS files (ones that would
try to write outside the boundaries of the clean file, thus crashing the
program), and warning when overwriting files that already exist.

v1.0
Program created and released.


What it is:

This is just a simple little program to create or apply IPS patches.
It takes advantage of the ease-of-use of the Windows File Menu system,
and can also handle patching where the altered file is larger than the
original file.

The interface is simple enough, the file menu contains three selections:

Create IPS Patch:
 You will be prompted to select an unaltered file, then an altered version
 of the file, and then to name the resulting IPS patch. If the altered file
 is larger than the original file, you will also be prompted to name the file
 where the extra data will be stored.

Apply IPS Patch:
 You will be prompted to select an unaltered file, and then the patch to
 apply to that file. You will also be asked if you need to add extended
 data to the altered file. If yes, you will be prompted to select the file
 containing that data.

Exit:
 Exit the program.

I hope this program is helpful to many. It's functionality will be added to
the Windows version of one of my other programs, SonED, when it is ready for
release.

Please visit Organized Chaos to view my other projects:
http://stealth.emulationzone.org/

If you have any questions or comments, you may contact me at MStealthA@aol.com
