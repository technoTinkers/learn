![9](https://i.imgur.com/nCSnCEt.jpg)  

## Introduction  
---

Buzzer is a kind of electronic sound receiver with integrated structure. It is widely used as a voice device in electronic products like computers, printers, copying machines, alarm apparatus, electronic toys, auto electronic devices, telephones, etc..In this experiment, we are going to use Micro:bit to drive buzzer and make its sound circulate between high frequency and low frequency just like alarm song. And we will present its sound frequency on Micro:bit screen with bar chart format. 


## Component List  
---  

### Hardware：

- 1 x [micro:bit Board](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)  
- 1 x Micro-B USB Cable  
- 1 x [microbit Breadboard Adapter](http://www.elecfreaks.com/estore/microbit-breadboard-adapter.html)  
- 1 x [Transparent Breadboard - 83 * 55 mm](http://www.elecfreaks.com/estore/transparent-breadboard-83-55-mm.html)  
- 1 x Mini Speaker (Buzzer)  
- 1 x TIP 120 NPN Transistor  
- 1 x 100 Ohm Resistors  
- 1 x [Breadborad Jumper Wire 65pcs Pack](http://www.elecfreaks.com/estore/breadborad-jumper-wire-65pcs-pack.html)  

**Tips: If you want all components above, you will need [Elecfreaks micro:bit Starter Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-starter-kit-795.html).**  

![](https://i.imgur.com/W4tseua.jpg)  


## Software:  

[Microsoft Makecode Online Editor](https://makecode.microbit.org/)  


## Major Component Introduction    
---  

### Buzzer  

Buzzer is a kind of voice device. It is made of vibration device and resonance device. According to the difference of control method, we can divide buzzer into active type and passive type.   

![](https://i.imgur.com/KfDVHIk.jpg)   

Here’s the working principle of active buzzer:   
Because active buzzer has integrated amplify sampling circuit and resonance system, when DC power input pass through active buzzer, it will make resonance device generate sound signal. We can see the schematic diagram below for the working principle of active buzzer:  

![](https://i.imgur.com/spNnKiB.jpg)     

The working principle of passive buzzer is: When square wave signal pass through the buzzer, its resonance device will transform the square wave signal input into sound signal output. Below is the schematic diagram for the working principle of passive buzzer:   

![](https://i.imgur.com/kNHyjjl.jpg)   
 
Note: In this experiment, we use passive buzzer only.   

### Transistor  

Transistor is a kind of semi-conductor component for current control. It is used to amplify the weak signal to signal with larger frequency.  

![](https://i.imgur.com/LEvAFS5.jpg)  

If we input PWM signal produced by Micro:bit into buzzer directly, the buzzer will send out feeble voice. This is because the drive current of I/O port is usually too weak to directly drive components like buzzer. At this time, we have to use transistor to amplify the current of PMW signal so that the buzzer can alarm properly. Here is the circuit diagram for a typical application of using transistor to drive buzzer:  

![](https://i.imgur.com/ZhQ3fhv.jpg)  


## Hardware Connection  
---  

Please complete connection according to the picture below.
![](https://i.imgur.com/YTNuh7H.jpg)

After connection, you will see:
![](https://i.imgur.com/iYiZM7O.jpg)  


## Programming
---

Please open Microsoft Makecode, write your code in the edit area. I would like to suggest you to program by yourself first. 

Of course, you can see the whole program in the link below. Just click “Edit” on the right top corner of the interface to edit your program, and then click “Download” to download your code into Micro:bit directly.

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_9k7bPrCdue1Y" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


## Code Explain
---

**Analog Set Period**

Configure the period of Pulse Width Modulation (PWM) on the specified analog pin. Before you call this function, you should set the specified pin as analog.

Under brick “on start”, set two variables: variable “f” is for audio frequency, variable “item” for frequency change intervals. 

![](https://i.imgur.com/Jwr97SA.jpg)

Under brick “forever”, “analog write pin P0 to 512” indicates to make “P0” output square wave.

![](https://i.imgur.com/40bHXlV.jpg)

Variable “T” is for square wave period. We all know that “ period=1s/frequency” and time unit in  “Analog Set Period” is “us”. So we get “T=1000000/f”. 

![](https://i.imgur.com/uIUqFVh.jpg)

Every circulation makes “f” change “item”, “f” changes among 20Hz to 6000Hz.

![](https://i.imgur.com/TNh0ZHb.jpg)


## Experiment Result  
---  

The sound sent out by buzzer changes between high frequency and low frequency. And we can see the bar chart of frequency on Micro:bit screen.

![](https://i.imgur.com/2AJXtVY.gif)

 
## Think     
---  

If we want to make a high temperature alarming device with temperature sensor and buzzer, then how can we design circuit and program? We look forward to your feedback and further discussion.   



## FAQ  
---  

   

