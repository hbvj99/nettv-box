# NetTv IPTV box easy hack 

This is a simple guide to install Android TV OS skin/bypass restrictions on NetTv devices. You will be able to use the Android platform into your television after successfully flashing the <b>proper</b> firmware. NetTv interface is basically a custom or limited software that runs on the top of any Android TV OS skin Box. It requires a device disassemble to find the correct model number.

The below procedure can also be applied to fix any bricked device. You may require to short NAND pins if your device won't boot. Most of the firmware are available pre-rooted.

> <b>Disclaimer: This is a non-proper guide to install android tv firmware to your NetTv box. It is solely done for educational purposes. I'm not responsible for any physical damage or bricking of the devices that you might encounter. Please proceed on your own risk. thank you
</b>

View updated guide in a [blog](https://vijaypathak.com.np/2019/11/nettv-box-hack.html)

# Method 1 : Custom Firmware

## How it works?
- Understand your device model number, chipset, specs
- Download correct firmware
- Understand the flashing procedure
- Install Android

## Requirement
- USB 2.0 Type A Male to Male connector
- USB burning tool for Amglogic <a href="https://androiddatahost.com/5yaux" target="_blank">chipset</a>, for Rockchip  <a href="https://androiddatahost.com/5yaux" target="_blank">device</a>. Visit <a href="https://androidmtk.com/category/drivers" target="_blank">here</a> for different chipset
- Firmware for Vianet devices model Amglogic <a href="https://drive.google.com/open?id=1vujacdrzMZI5kcKKqBUzBYT9eidP9g-s" target="_blank">S905x</a> 1GB RAM/4GBROM, get older worldlink firmware for model MXQ <a href="http://firmware.mxqproject.com/index.php/2018/04/04/mxq-4k-rockchip-3229-android-nougat-firmware-update-files/" target="_blank">RK3229</a> 1GB RAM
- Windows 7 or plus

## Procedure (for Vianet Amlogic S905X)

1. Remove Phillips screw hidden under four soft pads.

![Screenshot from 2019-10-01 19-30-52](https://user-images.githubusercontent.com/43197293/65968537-0ce9ac00-e483-11e9-9c01-7d9d746ca94f.png)

2. Note the device model number. In the below image, the device is using Amlogic S905X. Your device name may vary, in case of different name X, search model X in google and its specs or chipset.

![IMG_20190815_114509__01](https://user-images.githubusercontent.com/43197293/66922432-cc735c00-f046-11e9-94fe-32286bb61841.jpg)

![usb](https://user-images.githubusercontent.com/43197293/67307640-858ad800-f518-11e9-8744-b66b5f14a983.png)

3. Change language on USB burning tool by navigating to the top right second tab, click and choose the English language. Load the firmware image file by clicking file>import image. The tool will verify the file and click START when completed. In the configuration, choose normal erase and erase bootloader option. <b>Please find the correct firmware image to continue. The file extension should be .IMG</b>

4. Hold the device reset button for few seconds (7) which is usually located behind SPDIF port or sometimes AV port. Use a toothpick to hold reset pin and connect Type-A male connector from your device USB port (use bootable USB port) to your PC USB port. Plug the power cord to the device.

5. Once the device is detected on the USB burning tool, the device ID is shown and the flashing procedure will continue.

6. Wait for flashing or download system procedure to 100% and burned successfully text is shown (this might usually take 3 to 5 minutes).

7. The firmware update is completed. The device may take a few minutes to start a fresh new boot in Android TV platform.
<hr>

## Images after fresh install

![IMG_20190815_132345-01](https://user-images.githubusercontent.com/43197293/67455257-d7cd1580-f64c-11e9-8702-e0ad8d79a925.jpeg)
![IMG_20190815_132430-01](https://user-images.githubusercontent.com/43197293/67455258-d7cd1580-f64c-11e9-8341-73aabab508f5.jpeg)
![IMG_20190815_132921-01](https://user-images.githubusercontent.com/43197293/67455259-d865ac00-f64c-11e9-8707-d4697a377c04.jpeg)
![IMG_20190815_143723-01](https://user-images.githubusercontent.com/43197293/67455260-d865ac00-f64c-11e9-97fe-28fb19f8025c.jpeg)
![IMG_20190815_143933-01](https://user-images.githubusercontent.com/43197293/67455261-d8fe4280-f64c-11e9-90a0-2e26dff3d147.jpeg)
![IMG_20190815_144527-01](https://user-images.githubusercontent.com/43197293/67455263-d8fe4280-f64c-11e9-8720-1433ebc6f303.jpeg)


# Method 2: Install on the top of offical NetTv

## Process

[Method 1](#method-1--custom-firmware) is fairly limited and you need to disassemble your device before proceeding, mostly it's done for testing purposes since your official NetTv services won't work after.

This is the solid alternative, let me explain. We are going to bypass and access the hidden [Google play store](https://play.google.com/) to install other Android apps. This is relatively easy and we aren't modifying firmware this time so we can install updates from ISPs in future without a problem. 

> We can do this because NeTv devices are simply an Android TV OS skin limited by third party software and we are going to bypass this.

Steps to follow;
1. First, grab the USB mouse and keyboard and attach both to the device backside USB ports. Disconnect the LAN Ethernet port from the device and connect to your wifi by navigating to net tv settings>network.
2. Next, press Win(Windows logo key)+b from the keyboard, a browser will appear.
3. Goto ```https://play.google.com/store/apps``` in browser URL and try to install an app, you will be redirected to Google sign-in page.
4. After signing, install a [tv launcher](https://play.google.com/store/apps/details?id=ca.dstudio.atvlauncher.free) from play store, after installing press home key from remote and select the new launcher as default.
5. Make sure you download some apps externally from the browser (we're going to download youtube for android tv app since it is incompatible in play store), the default storage location is internal>Download.
6. Now you can open play store app and install various apps as you may like, but as I have noticed some firmware versions have disabled installing external apps from storage. We're going to enable this since most of the devices come pre-rooted.
7. We're going to install a [terminal](https://play.google.com/store/apps/details?id=jackpal.androidterm) from play store first and open.
8. Next, enable superuser by typing ```su``` as a command.
9. We are going to enable unknown source apps by typing command ```settings put global install_non_market_apps 1``` This is important for users who cannot access Android settings and manually enable.
10. Install apps by typing command: ```pm install /storage/emulated/0/Download/your_app_name.apk``` Follow this command to install different apps.

### Image

![IMG_20200603_181154__01](https://user-images.githubusercontent.com/43197293/83907736-a5a89800-a785-11ea-8cbf-7a5f5ec4e26d.jpg)

> Note, you need to connect LAN Ethernet port to access official Live TV. Likewise, remove LAN Ethernet port and connect through wifi to run apps that require active internet connection.

That's it. Your apps will now be available in launcher apps. Please feel free to comment down below if you have any questions?


## Contribution

YYou can modify the content, optimize the guide by sending pull [requests](https://github.com/hbvj99/nettv-box/pulls).

