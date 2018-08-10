# macosemushells
Modified emulators for all-in-one OS emulation.  Designed to display in doubled 640x360 or 1280x720 screen resolution (default 720P video for YouTube, etc, will not be scaled so stays crisp).

For "1983  Twiggy Mac (DP2/PR1.7).app" through "1994 Macintosh System 7.1.2 (Jirocho).app":

All the non-Performa apps are based on Mini vMac (mostly 3.4.1 and later).

A ROM image and a boot image will need to be placed in <file>.app/Contents/mnvm_dat/ -- the folder indicates the name needed for the ROM image and the boot image.  The ROM image has to be a valid Macintosh 128K ROM image, a valid Mac Plus ROM image or a valid Macintosh II-series ROM image as indicated; the dsk file should be a Disk Copy 4.2 compatible boot disk of the indicated OS version.  After these are added correctly, the application will boot into the OS automatically when double clicked.
  
  
For "1992  Macintosh System 7.0.1P (P200)" through "1995 Mac OS 7.5.1 (P630CD)":

All the apps targeting Performa computers in this range are using Basilisk II.

A ROM image for the Quadra 650 or compatible and a sparsebundle disk image of the OS will need to be added to <filename>.app/Contents/Resources/ or the file <filename>.app/Contents/Resources/Config will need to be modified to point to the new boot image and ROM.
  
For "1995 Mac OS 7.5.2 (Marconi) (PPC).app" through "1999-2000 Mac OS 9.0.4 (Sonata).app":

All the apps targeting non-OS X are using SheepShaver.

A New World ROM image and a sparsebundle disk image (2MB image segments) will need to be added to <filename>.app/Contents/Resources/Files/MacOS.sheepvm/ -- the file <filename.app>/Contents/Resources/Files/MacOS.sheepvm/prefs contains the configuration data.
