[简体中文](https://github.com/Albert-ShaoHua/NOKIA-N900-Recovery/blob/master/README.md)|English

# N900 RecoveryTutorial

#### System
    Linux（centos success）

#### Install
    1、First install 32-bit compatible library for 64 bit system
    2、Download
        （1）link：https://1drv.ms/u/s!AsXYd0VYSC9lgh9OGZYeeDccuSQg?e=6ToF5S
    3、Libusb is the USB driver installation, command: dpkg - I file name
    4、Maemo flash installation, command: dpkg - I file name
    5、Firmware
        （1）Emmc
        （2）Firmware

#### Recovery

    1、Turn off the mobile phone, press and hold the U key on the keyboard, connect the computer with the data cable, and the USB icon will be displayed in the upper right corner to enter recovery
    2、First, brush in the EMMC file
        （1）command：flasher-3.5 -F emmc.bin -f
        （2）display：image(s) flashed successfully in .... (success)
    3、Disconnect, take out the battery, put the battery in again, enter recovery again, and swipe in the firmware file
        （1）flasher-3.5 -F firmware.bin -f -R
        （2）Auto restart successfully