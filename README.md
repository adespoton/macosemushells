# macosemushells
Modified emulators for all-in-one OS emulation.  Designed to display in doubled 640x360 or 1280x720 screen resolution (default 720P video for YouTube, etc, will not be scaled so stays crisp).


<B><U>For "1983  Twiggy Mac (DP2/PR1.7).app" through "1994 Macintosh System 7.1.2 (Jirocho).app":</U></B>

All the non-Performa apps are based on Mini vMac (mostly 3.4.1 and later).

A ROM image and a boot image will need to be placed in <filename.app>/Contents/mnvm_dat/ -- the folder indicates the name needed for the ROM image and the boot image.  The ROM image has to be a valid Macintosh 128K ROM image, a valid Mac Plus ROM image or a valid Macintosh II-series ROM image as indicated; the dsk file should be a Disk Copy 4.2 compatible boot disk of the indicated OS version.  After these are added correctly, the application will boot into the OS automatically when double clicked.
  
  
<B><U>For "1992  Macintosh System 7.0.1P (P200)" through "1995 Mac OS 7.5.1 (P630CD)":</B></U>

All the apps targeting Performa computers in this range are using Basilisk II.

A ROM image for the Quadra 650 or compatible and a sparsebundle disk image of the OS will need to be added to <filename.app>/Contents/Resources/ or the file <filename.app>/Contents/Resources/Config will need to be modified to point to the new boot image and ROM.
 
 
<B><U>For "1995 Mac OS 7.5.2 (Marconi) (PPC).app" through "1999-2000 Mac OS 9.0.4 (Sonata).app":</B></U>

All the apps targeting non-OS X are using SheepShaver.

A New World ROM image and a sparsebundle disk image (2MB image segments) will need to be added to <filename.app>/Contents/Resources/Files/MacOS.sheepvm/ -- the file <filename.app>/Contents/Resources/Files/MacOS.sheepvm/prefs contains the configuration data.


<B><U>For "1999 Mac OS X Server 1.2v3.app" through "2007-9 Mac OS X 10.5.8 (PPC) (Leopard).app":</B></U>

No ROM image is needed, but you will need to modify the <filename.app>/Contents/Resources/script file to point to the install image and hard disk image you wish to use.  Make sure each line of the qemu command ends with a \ except the last one.
