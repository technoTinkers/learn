
# Troubleshooting downloads with WebUSB
---
- Having issues pairing your micro:bit with [ WebUSB ](https://makecode.microbit.org/device/usb/webusb)？Let’s try to figure out why!

## Step 1: Check your cable
---

Make sure that your micro:bit is connected to your computer with a micro USB cable. You should see a **MICROBIT** drive appear in Windows Explorer when it’s connected.。

![](https://i.imgur.com/Squ6KpH.png)

**If you can see the MICROBIT drive go to step 2.**

If you can’t see the drive:

- Make sure that the USB cable is working.

    Does the cable work on another computer? If not, find a different cable to use. Some cables may only provide a power connection and don’t actually transfer data.

- Try another USB port on your computer.

Is the cable good but you still can’t see the MICROBIT drive? Hmm, you might have a problem with your micro:bit.If you are our cutomers, please feel free to contact us.

## Step 2: Check your firmware version
---

It’s possible that the firmware version on the micro:bit needs an update. Let’s check:

1.Go to the MICROBIT drive.

2.Open the DETAILS.TXT file.


![](https://i.imgur.com/GB7LQBv.jpg)

3.Look for a line in the file that says the version number. It should say Version: ... 

![](https://i.imgur.com/CU5Ajdd.jpg)

If the version is **0234, 0241, 0243** you NEED to update the[firmware](https://makecode.microbit.org/device/firmware) on your micro:bit.Go to **Step 3** and follow the upgrade instructions.

If the version is **0249, 0250** or higher, you have the right firmware go to step 4.

## Step 3: Upgrade the firmware
---

1.Put your micro:bit into **MAINTENANCE Mode**. To do this, unplug the USB cable from the micro:bit and then re-connect the USB cable while you hold down the reset button. Once you insert the cable, you can release the reset button. You should now see a **MAINTENANCE** drive instead of the **MICROBIT** drive like before. Also, a yellow LED light will stay on next to the reset button.

![](https://i.imgur.com/02zBjkk.gif)

2.[Download the firmware ZIP file](https://github.com/ARMmbed/DAPLink/releases/download/v0250/0250_release_package_682d8303.zip) .

3.Find the **0250-kl26z-microbit-0x8000.hex** in the downloaded zip file **0250-release-package-682d8303.zip** .

4.Drag and drop that file onto the **MAINTENANCE** drive.

5.The yellow LED will flash while the HEX file is copying. When the copy finishes, the LED will go off and the micro:bit resets. The **MAINTENANCE** drive now changes back to **MICROBIT**.

6.The upgrade is complete! You can open the DETAILS.TXT file to check and see that the firmware version changed to the match the version of the HEX file you copied.

If you want to know more about connecting the board, MAINTENANCE Mode, and upgrading the firmware, read about it in the[Firmware support page](https://support.microbit.org/support/solutions/articles/19000019131-how-to-upgrade-the-firmware-on-the-micro-bit) 

## Step 4: Check your browser version
---

WebUSB is a fairly new feature and may require you to update your browser. Check that your browser version matches one of these:

- Chrome 65+ for Android, Chrome OS, Linux, macOS and Windows 10.

## Step 5: Pair device
---

Once you’ve updated the firmware, open the **Chrome Browser**, go to the editor and click on **Pair Device** in the gearwheel menu.See [ WebUSB ](https://makecode.microbit.org/device/usb/webusb) for pairing instructions.

Enjoy fast downloads!
