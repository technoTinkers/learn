![4](https://i.imgur.com/MwngMAi.jpg)

## Introduction  
---

Photocell is a kind of special resistance based on internal photoelectric effect. Its resistant value is opposite to the brightness of light. Brighter light leads to lower resistant value. Usually photocell is the core component of a photoswitch. In the following experiment, we are going to use photocell to control the brightness of 5*5 LED screen on micro:bit.


## Component List  
---

### Hardware:

- 1 x [micro:bit Board](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)
- 1 x Micro-B USB Cable
- 1 x [micro:bit Breadboard Adapter](http://www.elecfreaks.com/estore/microbit-breadboard-adapter.html)
- 1 x [Transparent Breadboard - 83 * 55 mm](http://www.elecfreaks.com/estore/transparent-breadboard-83-55-mm.html)
- 1 x Photocell
- 1 x 10k Ohm Resistors
- 1 x [Breadborad jumper wire 65pcs pack](http://www.elecfreaks.com/estore/breadborad-jumper-wire-65pcs-pack.html)

**Tips: If you want to buy all components above, then you will need [Elecfreaks micro:bit Starter Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-starter-kit-795.html).**

![](https://i.imgur.com/W4tseua.jpg)

### Software:

[Microsoft Makecode Online Editor](https://makecode.microbit.org/)


## Introduction of Major Components  
---

### Photocell

Photocell is a kind of special resistance made of semi-conductor materials like Cds or CdSe. It is based on internal photoelectric effect. Brighter light, lower resistant value. As with the increase intensity of light, its resistant value swiftly decreased. The minimum light resistant value can reach under 1KΩ. Photocell is very sensitive to light. When there is no light, its resistant value arrives maximum. Its dark resistant value usually can reach 1.5MΩ at max.  

![](https://i.imgur.com/jS03zGQ.jpg)


## Hardware Connection  
---

Please complete hardware connection according to the picture below.

![](https://i.imgur.com/FtQDhiS.jpg)

A bleeder circuit will be formed when photocell and 10KΩ resistance connect inserial.

After connection, you can see:

![](https://i.imgur.com/TMd3Fq8.jpg)


## Programming  
---

Open Microsoft Makecode, write code in editor window. I would like to suggest you to try programming by yourself first.

Of course, you can see the whole program in the link below. Just click “Edit” on the right top corner, then click “download” to download the whole code into micro:bit. 

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_iqDLctEkHFj1" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

Link of the whole program: [https://makecode.microbit.org/_iqDLctEkHFj1](https://makecode.microbit.org/_iqDLctEkHFj1)


## Code Explain  
---

**set**

This is assignment operation. set a to 1 equals to “a=1”. We use an equals sign to make a variable store the number or string you say.
When you use the equals sign to store something in a variable, the equals sign is called an assignment operator, and what you store is called a value.

**analog read**

Read an analog signal (0 through 1023) from the pin you say.

**show icon**

Shows the selected icon on the LED screen

**Clear Screen**

Turn off all the LED lights on the LED screen.

**If else**

In Lesson 2, we have talked about the usage of “if” sentence. In sentence of “ if else”, when the format value is false(or 0), then it will implement “else” brick program before running program in sequence. Here is the flow chart: 

![](https://i.imgur.com/E5Xi2Uu.jpg)

In this experiment, micro:bit read analog voltage of Pin0 port as the reference value of brightness.

![](https://i.imgur.com/Tck85NO.jpg)

In brick “ forever” , scan analog voltage of Pin0 in circulation. Once the voltage lower than reference value minus 2( it shows intensity of light increase, resistant value of photocell decrease), then it tells the light has been turned off. 

![](https://i.imgur.com/K8tmDxV.jpg)

In program, calibrationVal-2 is for adjusting sensitivity. Lower value, higher sensitivity. However, it is not suitable for all kinds of light environment. You have to adjust this parameter until it can adapt to the present light condition. 


## Experiment Result
---

Turn on light, 5*5 LED screen on micro:bit become empty. Turn off light, LED screen displays a sign of heart.

![](https://i.imgur.com/1Xu4lBR.gif)

**Note:**
After resetting micro:bit, it will calibrate the reference value according to the present brightness. So, in order to make the program run properly, we must start micro:bit program on the condition that the light is turned on . 


## Think
---

If we want to use photocell to control a LED bead, then how to design circuit and program? We look forward to your further discussions or comments.


## FAQ
---

   

