# UEFI

## UEFI-Apps

### uefi shell

shellx64.efi; https://ftp.spline.inf.fu-berlin.de/mirrors/archlinux/iso/

https://wiki.archlinux.org/index.php/Unified_Extensible_Firmware_Interface

edk2-shell, uefi-shell-git

### Memtest 86
https://www.memtest86.com/memtest86.html

### GNU-EFI
https://sourceforge.net/projects/gnu-efi/
https://git.code.sf.net/p/gnu-efi/code
https://wiki.osdev.org/GNU-EFI

shows efifb resolutions

### nyan-load
https://github.com/ohnx/nyan-load

### goomse-cat
https://github.com/astr0n8t/goomse-cat

## Other ressources

### DUET

### uefi-example
https://github.com/tqh/uefi-example

### UEFITool
https://github.com/LongSoft/UEFITool

## Issues

UEFI GOP - graphics output protocol ; https://www.win-raid.com/t892f16-AMD-and-Nvidia-GOP-update-No-requests-DIY.html

## UEFI qemu
ed2k-ovmf
$ cp /usr/share/edk2-ovmf/x64/OVMF_VARS.fd my_uefi_vars.fd

-drive if=pflash,format=raw,readonly,file=/usr/share/edk2-ovmf/x64/OVMF_CODE.fd \
-drive if=pflash,format=raw,file=my_uefi_vars.fd

$ qemu-system-x86_64 -enable-kvm -m 1G -drive if=pflash,format=raw,readonly,file=/usr/share/edk2-ovmf/x64/OVMF_CODE.fd -drive if=pflash,format=raw,file=my_uefi_vars.fd
