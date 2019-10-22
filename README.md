# NetTv IPTV box easy hack 

This is a simple guide to install stock(ish) android tv firmware to NetTv devices. You will be able to use the android platform into your televison after sucessfully flashing the <b>proper</b> firmware. NetTv interface is basically a custom or limited software that runs on the top of any Android TV Box. It requires device disassemble to find the correct model number.

The below procedure can also be applied to fix any bricked device. You may require to short NAND pins if your device won't boot.

<b>Disclaimer: This is a non-proper guide to install android tv firmware to your NetTv box. It is soley done for educational purposes. I'm not responsible for any physical damage or bricking of your devices that you might encounter. Please proceed on your own risk. thank you
</b>

<hr>

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

![Screenshot from 2019-10-01 19-30-52](https://user-images.githubusercontent.com/43197293/65968537-0ce9ac00-e483-11e9-9c01-7d9d746ca94f.png)
1. Remove phillips screw hidden under four soft pads.

![IMG_20190815_114509__01](https://user-images.githubusercontent.com/43197293/66922432-cc735c00-f046-11e9-94fe-32286bb61841.jpg)

2. Note the device model number. In the above image the device is using Amlogic S905X. Your device name may vary, in case of different name X, search model X in google and its specs or chipset.

![usb](https://user-images.githubusercontent.com/43197293/67307640-858ad800-f518-11e9-8744-b66b5f14a983.png)

4. Change language on USB burning tool by nagivating to top right second tab, click and choose english language. Load the fimrware image file by clicking file>import image. The tool will verify the file and click START when completed. In the configuration, choose normal erase and erase bootloader option. <b>Please find the correct fimrware image to continue. The file extension should be .IMG</b>

3. Hold device reset button for few seconds (7) which is usually located behind SPDIF port or sometimes AV port. Use toothpick to hold reset pin and connect Type A male connector from your device USB port (use bootable USB port) to your PC USB port. Plug the power cord to the device.

4. Once the device is detected on USB burning tool, the device ID is shown and the flashing procedure will continue.

5. Wait for flashing or download system procedire to 100% and burned successfully text is shown (this might usually take 3 to 5 minutes).

6. The firmware update is completed. The device may take few minutes to start fresh new boot in Android TV platform.

<hr>

## Contribution

You can modify the content, optimize the guide by sending pull requests.


