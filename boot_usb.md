hardware
Pi 3B v1.2
usb pendrive: SanDisk 16GB Ultra Fit USB 3.1 Flash Drive - SDCZ430-016G-G46 

At PC
flash 2018-04-18-raspbian-stretch.img to USB pendrive using etcher-electron-1.4.4-x86_64.AppImage
sudo gparted to read uuid of thumbdrive\rootfs partition

At Pi
boot Pi from SDCARD
insert above USB, make sure detected
copy above uuid to /boot/cmdline.txt, refer https://www.raspberrypi.org/forums/viewtopic.php?t=205374
remove SDCARD
sudo reboot 

Backup USB image
  sudo fdisk -l
  sudo dd if=/dev/sdd of=usb.img status=progress bs=4M
