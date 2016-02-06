This is a modifications of yellows8's hblauncher_loader, which you can get here:
https://github.com/yellows8/hblauncher_loader

Modifications:
* When downloading the payload it always gets saved even without pressing Y
* A duplicate from the payload get created with the extension _GRD
* The duplicated payload gets modified to boot "bgrd.3dsx" instead of "boot.3dsx" (Every occurence of boot.3dsx gets replaced with bgrd.3dsx -> might not always work, but can't break anything)
* Removed some print instructions
* Added some print instructions
* Icon to implicate a grid view
* Different Banner


This is a 3DS homebrew application intended for running under a NCCH(which can be installed via .cia), for booting the *hax payloads. https://smealum.github.io/3ds/  
The only difference tho yellows8s version is that the payload gets modified to boot bgrd.3dsx instead of boot.3dsx

This app was mostly finished in October 2015, this was finally released on November 25, 2015, due to the custom logo being finished.

This will first attempt to load the payload from SD, if that isn't successful it will then automatically download the payload for your system with HTTP. SD payload loading can be skipped if you hold down the X button. If you hold down the Y button, this will write the downloaded payload from HTTP to SD, if it actually downloaded it via HTTP.  

The exact filepath used for the SD payload depends on your system. Since this app can handle writing the payload here itself, writing the payload here manually isn't really needed. Example SD filepath with New3DS 10.1.0-27U: "/hblauncherloader_otherapp_payload_NEW-10-1-0-27-USA.bin". The Old3DS filepath for the same system-version and region as that example is the same, except that "OLD" is used instead of "NEW".

If you want to manually build this, you'll need a "Resources/hblauncher_loader_logo-padded.lz11" file, which should be the "prebuilt_homebrew_logo-padded.lz11" file from here: https://github.com/yellows8/ctr-logobuilder You'll also need this: https://github.com/Steveice10/bannertool

Credits:
* 3DSGuy for originally converting the CWAV used by this app's banner, years ago(which seems to be originally from the Wii HBC banner audio?).

