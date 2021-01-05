[简体中文](https://github.com/Albert-ShaoHua/NOKIA-N900-Recovery/blob/master/README.md)|English

# N900刷机教程

#### 系统要求
    Linux（centos测试成功，其他暂未测试）

#### 安装刷机工具/下载固件
    1、64位系统先安装32位兼容库（自行百度，不超过5条命令，很简单。）
    2、下载地址
        （1）链接：https://pan.baidu.com/s/18iG2z38xoIEkIgCOmErQZQ
        （2）提取码：xmea
    3、libusb是usb驱动全部安装，命令：dpkg -i 文件名（下载地址见2）
    4、Maemo flasher安装，命令：dpkg -i 文件名（下载地址见2）
    5、固件下载
        （1）Emmc（下载地址见2）
        （2）Firmware（下载地址见2）

#### 刷机

    1、手机关机，按住键盘上的u键，在用数据线连接电脑，右上角显示usb图标，进入刷机模式
    2、首先刷入emmc文件
        （1）命令：flasher-3.5 -F emmc.bin -f
        （2）显示：image(s) flashed successfully in .... (刷入成功)
    3、断开连接，取出电池，重新将电池放入再次进入刷机模式，刷入firmware文件
        （1）flasher-3.5 -F firmware.bin -f -R
        （2）刷机成功自动重启