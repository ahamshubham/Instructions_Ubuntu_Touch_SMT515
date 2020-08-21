My device details:
Device Model Number: SM-T515NZKDINU
Linux Kernel Version: 4.4.111-17420370

Instructions for SM-T515:

1) Download these files using the links given in the post: https://forum.xda-developers.com/galaxy-tab-a/development/ubports-ubuntu-touch-sm-t510-t515-t4146417:
	a) Halium arm32 GSI file
	b) Ubports Patched Kernel
	c) (Optional) SamsungUSBTethering zip

2) Copy all the above files to your External SD Card and insert this SD card in the device (tablet)

3) Flash STOCK Android 9.0 Pie on your device (tablet) and install TWRP:
	a) For installing TWRP, use the following post: https://forum.xda-developers.com/galaxy-tab-a/development/recovery-twrp-3-3-1-2019-galaxy-tab-10-1-t3934805. The instructions for installing TWRP as given in this post are:
		i) Unlock bootloader (See the end of my comment)
		ii) Hold Vol Up & Vol Down buttons during restart to enter Download mode
		iii) Install TWRP to AP with Odin
		iv) Hold Power & Vol Up buttons during restart to enter TWRP recovery
		v) On TWRP: Swipe to allow modifications
		vi) On TWRP: Wipe -> Advanced Wipe -> Select all except SD card
		vii) On TWRP: Reboot -> Recovery

4) On TWRP: Go to Install -> Install Image -> (Flash halium-boot.img. Partition to flash image is BOOT). DON'T REBOOT. PRESS BACK.

5) On TWRP: Go to Install -> (Flash ubports_GSI_installer_V1-arm32.zip. Don't check any check boxes)

6) (Optional) On TWRP: Goto Install -> (Flash samsung-usb-tethering.zip)

7) Reboot

8) Ubuntu Touch will open. The password is: phablet

Unlocking Bootloader (Check this post: https://www.getdroidtips.com/oem-unlocking/):
1) Enable Developer Mode in Device Settings
2) Enable OEM Unlocking Option in Developer options after connecting to WiFi and setting the year in the phone to the year 2019
3) Get into Device Unlock Mode: Press (Volume Up Key + Volume Down Key + Insert USB Cable in the phone) while restarting the phone
4) Unlock bootloader. (Very Important!!) DON'T LET THE DEVICE BOOT INTO THE ANDROID OS AFTER UNLOCKING DEVICE BOOTLOADER
