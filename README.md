# JUST-RG350M-
Stable firmware for RG350M, kernel version 3.12.0 from original firmware with recent 1.16 RetroArch Version.


I just want to create an image for Anbernic rg350m with installed retroarch cores and not beta firmware.

SO to eduardofilo and his RG350_auto_ra_installer (https://github.com/eduardofilo/RG350_auto_ra_installer) as I use it as template for compile retroarch for original firmware.

This version aims to provide a stable experience. While I really enjoyed Adam Image, it was too unstable on my device due to the OpenDingux beta firmware. So, I decided to compile RetroArch for the original stock firmware and package everything into a single image.

Additionally, I prefer the gambatte-dms (link) and reGBA (link) emulators on the RG350M. To complete the setup, I included Simplemenu (link) and a Game Boy theme (link). And voilà!

# Installation

1. Download the image and flash it to an SD card (8GB or larger).
2. Use a second SD card or expand the "SDCARD" partition on the system SD card. Second SD card is recommend and a SDCARD folder structure is provided in downloads.
3. Add your games inside the ROMS folder. For example, Game Boy ROMs should go in /ROMS/GB/. (second sd card should be named "SDCARD"
4. You can modify the .simplemenu configuration to add more systems. Just remember to name the second SD card or the expanded partition and name it "SDCARD" (capital letters). 

# video
This is a mini tour to the system. Enjoy!

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Fjr4lRH9pt0/0.jpg)](https://www.youtube.com/watch?v=Fjr4lRH9pt0)

## Bios

You need to add your bios for better compatibility.

- PSX bios under /.pcsx4all/bios with name SCPH1001.bin
- GB and gbc bios under /.gambatte/bios/ with names gb_bios.bin and gbc_bios.bin
- GBA bios under /.gpsp/ with name gba_bios.bin

you can acess this directories with commander (dingux cmdr) easily, just quit simplemenu once (press start on system selection and select NO in default launcher, then quit session), move the files from your computer to any folder on sd card and then add it to each directory.

## Perks

- Native bilinear filter, on stock you can control a bilinear filter, default is a little sharp but you can press POWER + DPAD UP or DPAD DOWN to change the value. For example with GB and Gambatte core in RA you can use aspect as core provided an use a lot more of the screen real state, but with the dotmatrix video filter pixels dont look good, if you add a little more of bilinear filter you can make it look amazing!
- Stability, Opendingux Beta is super unstable on my device, no matter what, a lot of crashes an freezes, with stock firmware this is not an issue, stability is amazing, I never experience a crash or freeze.
- Native emulators, Gambatte-DMS has a specific version for this device and it works great, I really enjoy the filters and palettes available with this emulators, regba is the same, it can use HW scalers and make GBA look good with amazing performance on this device.
