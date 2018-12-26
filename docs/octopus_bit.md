## Introduction
---

ELECFREAKS Octopus:bit is a kind of breakout boards for micro:bit. It can lead out GPIO port, serial port, IIC port, and SPI port on the micro:bit board. The biggest feature of Octopus:bit is that it can switch electric level for some GPIO ports, which makes micro:bit available to be adapted to 5V sensors.

![](https://i.imgur.com/wcgxnG0.png)


## Shipping List
---

1 x ELECFREAKS Octopus:bit


## Hardware
---

### Features

- Input voltage: 3.3V（powered by the edge connector of micro:bit）
- Extend all of GPIO ports(P0~P16, P19~P20).
- Beneath each I/O port, there are pins for VCC and GND. These pins are differentiated by different colors, which enable you to connect your extension module easily. The spread of pins is fully compatible with Octopus series' products.  
- With a voltage boosting module, you can shift the working voltage of P8, P9, P11~P16 between 3.3V and 5V through the voltage switch. 
- Lead out serial port, I2C port and SPI port, among which I2C can connect 3 channels of I2C devices and SPI can connect 2 channels of SPI devices. 
- Available for direct serial port communication between two breakout boards. 


### Application

It is suitable for all conditions that require micro:bit GPIO such as programming education, smart device creation, and so on.  

### Pins & Connectors

![](https://i.imgur.com/wCWdoag.jpg)


## More Details
---
 
#### Standard GVS Port 

![](https://i.imgur.com/gk3dN4E.png)

Among the standard GVS ports, the working voltage of the yellow part（P0~P7， P10）is 3.3V, while the working voltage of the blue part（P8, P9, P11~P16）can be shifted between 3.3V and 5V through a voltage switch. 
Beneath each I/O port, there are pins for VCC and GND. These pins are differentiated by different colors, which enable you to connect your extension module easily. The spread of pins is fully compatible with Octopus series' products.

#### Voltage Switch 

![](https://i.imgur.com/JoxT6k2.png)

Sliding this switch, we can change the voltage of the blue IO ports（P8, P9, P11~P16）between 3.3V and 5V.

You can see its working range in the below: 

![](https://i.imgur.com/GHPffMl.png)

#### Serial Port

![](https://i.imgur.com/8aVYsja.png)

The working voltage of serial port is available to be shifted between 3.3V and 5V through the voltage switch. 
Connect TX to P8，RX to P12. The left pins are bidirectional serial port, which can run both input and output. The right female header is a one-way output serial port. 

**Note** : To use this port, we have to initialize it according to the program in the below:   

![](https://i.imgur.com/1gnuYd5.png)  


## Dimension     
---  

![](https://i.imgur.com/ZYrWREG.jpg)  


## Software  
---  

### Example 1 Music Broadcast  

#### Hardware Connection   
Connect passive buzzer module to PO.

![](https://i.imgur.com/Zc6ChwR.jpg)

#### Code Example    

![](https://i.imgur.com/0MBprkk.png)  

You can download the whole program from the link here: [https://makecode.microbit.org/_fAmC3WERHdR2](https://makecode.microbit.org/_fAmC3WERHdR2)  

Download the whole program into your micro:bit, the buzzer will play Happy Birthday again and again in round.    


## Relative Cases  
---   

[Music Machine](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_01_Music_Machine/)  
[Smart Light ](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_02_Smart_Light/)  
[Electro-Theremin](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_03_Electro_Theremin/)  
[Simple Alarm Box](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_04_Simple_Alarm_Box/)  
[Plant Monitoring Device](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_05_Plant_Monitoring_Device/)  
[Intruder Detection](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_06_Intruder_Detection/)  
[Fish Feeder](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_07_Fish_Feeder/)  
[Motion Detector](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_08_Motion_Detector/)  
[Lie Detector](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_09_Lie_Detector/)  
[PADDLEBALLSUPERSMASHEM](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_10_PADDLEBALLSUPERSMASHEM/)  
[Avoid Asteroids](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_11_Avoid_Asteroids/)  
[Remote Control Everything ](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_12_Remote_Control_Everything/)  
[micro:bit Car](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_13_Micro_bit_Car/)  
[Flipping Pancakes](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_14_Flipping_Pancakes/)  
[Maze Runner](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_15_Maze_Runner/)  
[QUICK MATHS](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_16_QUICK_MATHS/)  
[Pitch Perfect](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_17_Pitch_Perfect/)  
[Finger Dexterity](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_18_Finger_Dexterity/)  
[Electric Spirit Level](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_19_Electric_Spirit_Level/)   
[Space Shooter](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_20_Space_Shooter/)  
[Flappy Bird](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_21_Flappy_Bird/)  
[Wire Transmission](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_22_Wire_Transmission/)  
[Snake Game](https://www.elecfreaks.com/learn-en/Micro_bit_Tinker_Kit_Case_23_Snake_Game/)   


## Relative Components
---


### [BBC micro:bit](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)

[![](https://i.imgur.com/nKomLk2.png)](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)


### [Octopus Bricks Series](http://www.elecfreaks.com/estore/octopus-bricks-sensor)

[![](https://i.imgur.com/m1Xdqvg.png)](http://www.elecfreaks.com/estore/octopus-bricks-sensor)

### [ElecFreaks Micro:bit Tinker Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-tinker-kit.html)

[![](https://i.imgur.com/pkfhaWF.jpg)](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-tinker-kit.html)
