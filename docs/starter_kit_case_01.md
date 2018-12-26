![1](https://i.imgur.com/GMzHtFZ.jpg)

## Introduction:  
---

LED has wide applications. Most signal lights we saw in our daily life use LED as its major light source. In today’s experiment, we are going to use Micro:bit to make 2 LED beads twinkle alternatively.


## Components List:  
---

### Hardware:  

- 1 x [Micro:bit Board](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)
- 1 x MicroB USB Cable
- 1 x [Microbit Breadboard Adapter](http://www.elecfreaks.com/estore/microbit-breadboard-adapter.html)
- 1 x [Transparent Breadboard - 83 * 55 mm](http://www.elecfreaks.com/estore/transparent-breadboard-83-55-mm.html)
- 2 x LED
- 2 x 100 Ohm Resistors
- 1 x [Breadborad jumper wire 65pcs pack](http://www.elecfreaks.com/estore/breadborad-jumper-wire-65pcs-pack.html)

**Tips: If you want all components above, you may need [Elecfreaks Micro:bit Starter Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-starter-kit-795.html).**

![](https://i.imgur.com/W4tseua.jpg)

### Software:  

[Microsoft Makecode Online Editor](https://makecode.microbit.org/)


## Major Components Introduction  
---

### Micro:bit Breadboard Adapter  

Micro: bit Breadboard Adapter can extend all footers of Micro: bit to breadboard so that we can create circuit on breadboard easily.

![](https://i.imgur.com/dq75zKC.jpg)

This is how Micro: bit Breadboard Adapter is plugged into breadboard. It can be suitable to all kinds of breadboards.

![](https://i.imgur.com/3DHC6U8.jpg)

### LED  

LED is the abbreviation of Light Emitting Diode. It is a kind of semi-conductor diode. It can convert electricity into light. When current passes throught it, it will glow with light.
 
![](https://i.imgur.com/gDwJTlH.jpg)
![](https://i.imgur.com/t8e1q6X.jpg)
 
If you look carefully at the LED you will notice two things. One is that the legs are of different lengths and also that on one side of the LED, instead of it being cylindrical, it is flattened. These are indicators to show you which leg is the Anode (Positive) and which is the Cathode (Negative). The longer leg gets connected to the Positive Supply (3.3v) and the leg with the flattened side goes to Ground.

### Resistance  

Resistance is a component for current control. It can limit the current of the circuit connected. And in our experiment, we use 100Ω resistance. If there is no current limit, it will cause LED damage.

![](https://i.imgur.com/WS9Fk9x.jpg)

Want to know resistance value by color circles? You can read this article: [How to Identify Color Circle Resistance Value](https://www.elecfreaks.com/9158.html).


## Hardware Connection  
---

Connect your components according to the picture below:
![](https://i.imgur.com/6JA8ooG.jpg)
 
After connection, you will see:
![](https://i.imgur.com/ZEP7gfe.jpg)


## Programming  
---

Click to open [Microsoft Makecode](https://makecode.microbit.org/), write the following code in the edit area.

![](https://i.imgur.com/s5sUftj.jpg)

You can see the whole program in the page below. Click “Edit” on the right top corner, and then “download”, you can download your code into Micro:bit.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_aPtRppeup0E5" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


Link of the whole program: https://makecode.microbit.org/_gLbYpW5wK6z7


### Code Explain:

**Forever**
The forever block is a block that loops any other command blocks inserted into it over and over again…forever. It starts from the top and executes your code in order working its way to the bottom and then starts at the top again.

**Digital Write**
The DigitalWrite block enables you to turn a pin on or off. There is a dropdown option for which pin you want to control, and it accepts a variable as the pins state. You use 1 as on and 0 as off. If you prefer, you can also use Boolean states of true and false, but we will use 0 and 1 as our standard throughout this guide.

**Pause**
If you were to just turn pins on and off with the digital write block without a pause, the LED would blink really, really fast. The pause block enables you to slow the micro:bit down and lets you control the timing of things happening. It accepts a number or variable as the number of milliseconds you want the micro:bit to pause. Think of this block as a stoplight for your code!


## Experiment Result  
---

You can see 2 LEDs flashing alternatively. If it is not, go back and check your operations.

![](https://i.imgur.com/xvYjvaQ.gif)


## Think  
---

If we want to control 4 LED beads and make it illuminate by turns, then how shall we design our circuit and make program. We would like to receive your further discussion with us. You can leave your comment below.



## FAQ
---

   

