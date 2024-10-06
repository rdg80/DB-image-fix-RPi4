# DB-image-fix-RPi4

This is a tutorial on how to fix an old image that was put out back in 2021? And seemed to work fine back then, but was having issues loading now.  This might not work for everyone, but this is how I got it to work in my use case.  Hope this helps, enjoy!

Error:
start4.elf: is not compatible

Main Outline - Steps to fix image

I. Get Image on to SD card
	A. Use disk/card imager of choice (Raspberry Pi Imager, Win32DiskImager, balenaEtcher)
II. Get image to boot without errors
	A. Replace fixup4.dat and start4.elf files
		1. Find known good working files
		2. Replace old files with the known good working files
	B. (Checkpoint) Splashscreen intro video should now play when booting up RPi4 with SD card image
III. Add additional files to image - in order to made further modifications
	A. Add ssh and wpa_supplicat.conf files
		1. Edit the wpa_supplicat.conf to match your internal network credentials
  B. The ssh file automatically enables ssh - so you can login using a terminal emulator
IV. Use a terminal emulator to connect to RPi4
	A. Run the specific "update" commands
  B. Reboot
V. Plug in gamepad and configure
	A. After gamepad is configured you should be able to navigate through the menus
VI. Fixing the Reboot and Shutdown options (in menus)
	A. Login to your RPi again, using terminal emulator
		1. Run chmod commands to grant privledges for the Reboot and Shutdown options


Oops that did not format properly, I'll have to fix the outline later

[More updates to come...] 

Last updated: Oct 6, 2024
