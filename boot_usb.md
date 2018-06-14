hardware
Pi 3B v1.2
usb pendrive: sandisk Ultra fit usb 3.1 flash drive

At PC
flash 2018-04-18-raspbian-stretch.img to USB pendrive using etcher-electron-1.4.4-x86_64.AppImage
sudo gparted to read uuid of thumbdrive\rootfs partition

At Pi
boot Pi from SDCARD
insert above USB, make sure detected
copy above uuid to /boot/cmdline.txt, refer https://www.raspberrypi.org/forums/viewtopic.php?t=205374
remove SDCARD
sudo reboot 
