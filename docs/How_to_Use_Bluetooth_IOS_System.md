# How to Use Bluetooth (IOS System)

![](https://i.imgur.com/qFY5fIV.png)

## Our Goal
---
- Use Bluetooth under IOS system to connect micro:bit. 


## Material
---

- 1 x [micro:bit](https://www.elecfreaks.com/estore/micro-bit-board-with-battery-holder-kit-836.html)
- 1 x IOS System 


## Background Knowledge 
---

- [micro:bit](http://microbit.org/) is a small pocket-sized programmable computer for teenager programming education. It is put forward by British Broadcasting Corporation(BBC) and aims to make programming study and teaching become more easy and funny.

- [IOS](https://en.wikipedia.org/wiki/IOS) is a mobile operating system created and developed by Apple Inc. It was published earlier since the Macworld Convention at Jan. 9th, 2007. It is originally designed for iphone, and later applied to products like iPod touch，iPad and Apple TV，etc..

- [Bluetooth](https://en.wikipedia.org/wiki/Bluetooth) is a wireless technology standard for exchanging data over short distances (using short-wavelength UHF radio waves in the ISM band from 2.4 to 2.485 GHz[3]) from fixed and mobile devices, and building personal area networks (PANs). We can use Bluettoth to connect multiple devices which resolves the difficulty of simultanuous data transmission. 

- [Bittysoftware](http://www.bittysoftware.com/index.html) provides mobile apps and tools for devices like BBC micro:bit.

- [nRF connect](http://www.nordicsemi.com/chi_simple) is a powerful and versatile tool. You can use it to scan, advertise and explore your Bluetooth Low Energy(BLE) devices and communicate with them. 


## Software
---
#### nRf connect

![](https://i.imgur.com/aX7znnU.png)

Search "nRF connect" from your mobile APP store and download it. Here's the interface: 

![](https://i.imgur.com/n9wC36Q.jpg) ![](https://i.imgur.com/nHKuD86.png)

#### Bitty Blue

Search "Bitty Blue" from your mobile APP store and download it. Here's the interface:

![](https://i.imgur.com/I06aGgM.jpg)![](https://i.imgur.com/hmym0Xv.png)


## Programming 
---
### Step 1: Add Package

Click **Advanced** in the code drawer of MakeCode to see more options. 

![](https://i.imgur.com/LjMR5IU.png)

To program for motor:bit, we have to add a package. Find **Add Package** in the bottom of code drawer and click it. This will pop up a dialogue box. Search for "bluetooth" and then click to download this package.

![](https://i.imgur.com/ZNxv964.png)

Note: If you get a hint that some packages will be deleted due to the problem of incompatibility, you can either follow the prompts, or create a new project in the project menu.

### Step 2: Encode

Activate Bluetooth button function when your micro:bit is powered on and started. When connected by Bluetooth, display a string "T" on your micro:bit display. When disconnected, then display a string "F". 

![](https://i.imgur.com/WmMlkNr.png)

Link of the program: [https://makecode.microbit.org/_Dyu4j2A4F23c](https://makecode.microbit.org/_Dyu4j2A4F23c)


## Set Bluetooth Mode
---

To startup micro:bit Bluetooth mode, we need to press the button "A+B" and reset, then micro:bit screen will display a string **`PAIRING MODE！`** and a special character. This character is unique to each micro:bit board. It is a special indentifier for Bluetooth. 
<br></br>
<br></br>
![](https://i.imgur.com/hlt1jqD.jpg) ![](https://i.imgur.com/aqmIAwY.jpg)


## IOS System Paring 
---

- Open nRF connect and find a device similar to "BBC micro:bit[xxxxx]", then click "CONNECT". This will pop up a request for Bluetooth pairing. 

![](https://i.imgur.com/QinTNv6.png) ![](https://i.imgur.com/P2FeWBA.jpg)

- Click pair to complete Bluetooth connection, and then micro:bit screen will display a "√"(tick mark).

![](https://i.imgur.com/pbSFZZ8.jpg)

- Once paired successfully, your micro:bit will restart. 


## Bluetooth Connection
---

Open Bitty Blue, click "Scan" to obtain the paired Bluetooth device. Click on it to complete Bluetooth connection. Then micro:bit will display a string "T" and the APP will enter into its home interface.  

![](https://i.imgur.com/i9mucj8.png) ![](https://i.imgur.com/0KauZdY.png)

![](https://i.imgur.com/8YJdwQG.jpg)

Click the icons in the interface to test its relative functions. 

**Note:** Because we have activated the Bluetooth button function only in the program, so we can only use the test button "Animal Magic" in this case, or the program will go wrong. If you want to test other functions, you need to activate the relative functions in the program.


## Bluetooth Disconnection
---

Exit the APP or shut down Bluetooth switch on your IOS device will disconnect Bluetooth. Once disconnected, micro：bit will display a string "F". 

![](https://i.imgur.com/jcv7YrD.jpg)


## Think
---
How to write your code to test other module function of micro:bit under the Bluetooth mode? 


## FAQ
---

**Q: Why we can't successfully connect after restarting the updated program?**

A: Each time when micro:bit is restarted, we need to forget the paired deviceand then pair again. 

**Q: Why we can't download nRF connect app ?**

A: You can use other similar software for Bluetooth connection. The app we provided here is just for reference. 


## Relative Readings  
---

[Bitty Blue User Guide](http://www.bittysoftware.com/apps/bitty_blue.html)
