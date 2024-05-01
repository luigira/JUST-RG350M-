# JUST-RG350M-
Stable firmware for RG350M, kernel version 3.12.0 from original firmware with recent 1.16 RetroArch Version.


I just want to create an image for Anbernic rg350m with installed retroarch cores and not beta firmware.

SO to eduardofilo and his RG350_auto_ra_installer (https://github.com/eduardofilo/RG350_auto_ra_installer) as I use it as template for compile retroarch for original firmware.

This version aims for a relaible experience, I really enjoyed Adam Image but it was super unstable on my device bc of the OpenDingux beta firmware, so I decided to compile retroarch for original stock firmware and put all togheter on an image.

Also I prefer the gambatte-dms (https://github.com/bardeci/gambatte-dms) and reGBA (https://github.com/jdgleaver/ReGBA) emuators on the 350M so I aim for it, I complement it all with Simplemenu (https://github.com/fgl82/simplemenu) and a Gameboy theme (https://github.com/Yarkiebrown/GameBoy-Theme) and voila!

You can download the img and put it on an sd card (8gb or more) and added a second sd card or expand the "sdcard" partition on the system sd card and add your games under roms folder then gb for example (SDCARD/ROMS/GB/), you can modify section groups on .simplemenu to add more systems. Just remember to name the second sdcard or the extended partition as "SDCARD".

This is a mini tour to the system. Enjoy!

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/Fjr4lRH9pt0/0.jpg)](https://www.youtube.com/watch?v=Fjr4lRH9pt0)

##Bios

You need to add your bios for better compatibility.

psx bios under /.pcsx4all/bios with name SCPH1001.bin
gb and gbc bios under /.gambatte/bios/ with names gb_bios.bin and gbc_bios.bin
gba bios under /.gpsp/ with name gba_bios.bin

you can acess this directories with commander (dingux cmdr) easily, just quit simplemenu once, move the files from your computer to any folder on sd card and then add it to each directory.

##Perks

- Native bilinear filter, on stock you can control a bilinear filter, default is a little sharp but you can press POWER + DPAD UP or DPAD DOWN to change the value. For example with GB and Gambatte core in RA you can use aspect as core provided an use a lot more of the screen real state, but with the dotmatrix vide filter pixels dont look good, if you add a little more of bilinear filter you can make it look amazing!
- Stability, Opendingux Beta is super inestabe on my device, no matter what, a lot of crashes an freezes, with stock firmware this is not an issue, stability is amazing, I neve experience a crash or freeze.
- Native emulators, Gambatte-DMS has a specific version for this device and it works great, I really enjoy the filters and paletes available with this emulators, regba is the same, it can use HW scalers and make GBA look good with amazing performance on this device.
