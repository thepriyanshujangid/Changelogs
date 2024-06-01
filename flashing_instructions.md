# CLEAN FLASH

1.) Download the boot , dtbo  and vendor_boot images  from [HERE](https://sourceforge.net/projects/poco-x5-pro-roms/files/evolutionx/android-14/recovery/).  [all files are in zip file so kindly unzip that file.]

2.) Connect To Pc

3.) Reboot to fastboot  ( press  both power_button_key + vol_down_key ) and follow the steps as given below.

	fastboot flash boot boot.img

	fastboot flash vendor_boot  vendor_boot.img

	fastboot flash dtbo dtbo.img 

	fastboot reboot recovery

	Select Wipe Data/factory Reset & Confirm

	Select 'apply Update' From Adb

	adb sideload  Rom_Name.zip

	Select Wipe Data/factory Reset & Confirm

	After Installation Complete, Reboot System.

	( optional ). Reboot to recovery to sideload any add-ons ( e.g magisk, firmware, gapps etc )



# DIRTY FLASH ( Without data format )

1. Reboot to recover by holding power button and volume up simultaneously

2. In the recovery menu select Apply update through ADB

3. adb sideload Rom_name*.zip ( or drag down the rom zip to cmd )

4. After installation complete, Reboot system.

# Change partition slots ( optional )

If your device does not change slot automatically, you can do it manually just follow the given steps.
	adb reboot bootloader

	fastboot getvar current-slot

	fastboot --set-active=b ( for eg. your current active slot is A so you would want your current slot to set be on B )

	fastboot reboot
