![alt text](https://xdaforums.com/attachments/68-sem-titulo-png.6405127/ "Banner")
### -WTF is high5-2goya yuri?
We're a new custom ROM project who has plans for giving users a light experience by debloating the devices while giving them newer Android versions, such as Android 5.1 and above, and we're based on CyanogenMod, too.
We're codenamed "yuri" because you should expect the first few builds of the ROM to kill theirselves with kernel panics and because WE'RE PURPLE. Our team is composed by @Aliusta72, @AnUndefinedDeveloper and partially... me, because I designed the wallpaper and this banner and the codename blah blah blah blah blah. Yes, DDLC reference, by the way.

This project only supports the Tab 3 Lite! (SM-T110/SM-T111).
If you try to flash this on any other device (SM-T21x, SM-T113, SM-T116...) the flashing process will be cancelled.

This recovery is needed: https://drive.google.com/file/d/1zp-3kCNGAeI887cmkLJrO4kI4TfvBQCg/view?usp=drive_link
If not used, installation most likely will also halt.

Special credits to notnoelchannel, run4r.ses and etcetera for the base of this project.

### Downloads
To download this ROM, check out the releases tab: https://github.com/a3v9/high5-2goya/releases/tag/Unstable
high5-2goya Yuri — Installation Instructions​
IMPORTANT: These installation instructions are still under examination. They have not yet been fully verified.

Yuri is an extremely experimental Android 5.1.1 ROM for the Samsung Galaxy Tab 3 Lite SM-T110/T111 (goya).

WIP1/First Build:​
The boot animation works, but Android does not currently complete booting. The development team is investigating remaining userspace issues, including mediaserver.


■ 1. Download TWRP
Download this build of TWRP: https://drive.google.com/file/d/1zp-3kCNGAeI887cmkLJrO4kI4TfvBQCg/view?usp=sharing
After getting the .img file, rename it to recovery.img, and using 7Zip, pack it to a .tar file with no compression.
Open Odin3 on your computer.
Select the downloaded TWRP tar image in the PDA/AP slot.
Make sure Auto Reboot is UNCHECKED.
Start the flashing process.
Once Odin finishes, manually reboot your tablet directly into Recovery Mode.
IMPORTANT: Do not allow the tablet to boot into Android between flashing TWRP and entering recovery.

■ 2. Download Yuri's system image
Open the following MediaFire folder:
https://www.mediafire.com/folder/rb58m92zatgfs/300495d4ccf2a100

Download BOTH files:
system.ext4.win
system.ext4.win.md5
IMPORTANT: Do not forget the MD5 checksum file.
Create a dedicated folder with a name you'll be able to differentiate between your firmware and L1teExper1ence, like "yuri-testbuild-backup".
Place both downloaded files inside it.
Keep this folder somewhere accessible from TWRP.
■ 3. Prepare the Yuri backup
In TWRP, open Backup.
Select your preferred storage location.
Back up your current firmware, or at minimum the partitions you want to preserve.
Start the backup.
TWRP will create a directory structure similar to:
TWRP/Backups/(serial number)/(backup name)/
Locate the serial-number directory.
Copy your prepared Yuri folder into that directory.
IMPORTANT: TWRP requires a valid backup structure and associated metadata. The prepared backup must be recognized in TWRP's Restore menu before proceeding.

■ 4. Download and flash Yuri's boot image
Download the attached img file (YuriKernel-CM12.img)
Transfer YuriKernel-CM12.img to your preferred storage location.
In TWRP, select Install.
Choose Install Image.
Locate and select YuriKrrnel-CM12.img.
Select the Boot partition.
Confirm the flash.
Once completed, reboot back into Recovery Mode.
Double-check that you selected the Boot partition.

■ 5. Wipe the existing partitions
In TWRP:
Open Wipe.
Select Advanced Wipe.
Select:
System
Preload
Cache
Dalvik / ART Cache
Data
Confirm the wipe.
WARNING: Make sure your Yuri files and backups are stored somewhere that remains accessible after wiping. External storage is recommended.

■ 6. Restore Yuri
Return to the TWRP main menu.
Open Restore.
Locate the prepared Yuri backup.
Select the System partition.
Swipe to restore.
Wait for the restoration process to finish.
■ 7. Reboot into Yuri
Once the restoration finishes:
Return to the TWRP main menu.
Select Reboot → System.
Allow the device to attempt its first boot.
Congratulations! You've installed Yuri.

■ Recovery-looping? Here's a fix
If you're recovery looping, that means, going back to recovery after following all steps correctly, that means it's a problem with the recovery, because the installation method has been tested and IT WORKS. If you're experiencing this, follow the steps:

METHOD 1
On TWRP, go to Reboot, and simply select Busybox reboot
METHOD 2
Download paziusss's TWRP v2.6.3.0 here: https://xdaforums.com/t/sm-t11x-twrp-2-6-3-0-for-tab3-lite.3060819/ preferrably download the twrp-odin version
Put your tablet in Download Mode, and open Odin3 on your computer
Flash TWRP v2.6.3.0 onto the PDA slot, untick Auto Reboot as always.
Reboot your tablet to recovery,on TWRP, head to Reboot > System
You're now on Yuri!

■ Known limitations
The boot animation works.
Android does not currently complete booting.
mediaserver is constantly crashing.
Other userspace and hardware compatibility issues may remain.
Please report bugs and provide logs to the development team.


WIP2/Second Build and above:​
Android now boots, and everything works, buuut there are some problems:
Literally, everything

Actually I'll stop joking about it, here's the real problem:
Not working is Wi-Fi and pretty much every other service, colors are still inverted, solution should be to disable HWC.

### XDA Thread
https://xdaforums.com/t/t110-t111-5-1-1-wip-rom-high5-2goya-yuri-for-t110-t111.4807400/
