![10](https://i.imgur.com/8KZyoCy.jpg)

## Introduction  
---  

Motor is a kind of device which can transfer electric energy into kinetic energy according to the law in electromagnetic induction. In this experiment, we are going to use a switch to control the start and stop of a motor.   


## Component List  
---  

### Hardware:  

- 1 x [micro:bit Board](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)  
- 1 x Micro-B USB Cable  
- 1 x [micro:bit Breadboard Adapter](http://www.elecfreaks.com/estore/microbit-breadboard-adapter.html)  
- 1 x [Transparent Breadboard - 83 * 55 mm](http://www.elecfreaks.com/estore/transparent-breadboard-83-55-mm.html)  
- 1 x 5V Miniature Motors  
- 1 x TIP 120 NPN Transistor  
- 1 x 1N4007 Diodes  
- 1 x 100 Ohm Resistors  
- 1 x [Breadborad Jumper Wire 65pcs Pack](http://www.elecfreaks.com/estore/breadborad-jumper-wire-65pcs-pack.html)  
- 2 x Alligator Clip Wires  

**Tips: If you want all components above, you may need [Elecfreaks Micro:bit Starter Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-starter-kit-795.html).**  

![](https://i.imgur.com/W4tseua.jpg)  

### Software:  

[Microsoft Makecode Online Editor ](https://makecode.microbit.org/)  


## Major Component Introduction  
---  

### Motor  

Motor is a kind of device that can transfer electric energy into kinetic energy according to the law of electromagnetic induction. Motor has a lot of categories. In our experiment, the motor we use is DC motor. When we supply DC voltage to the two terminals of motor, it will rotate. The higher the voltage, the faster it rotates.  

![](https://i.imgur.com/JesPIk4.jpg)  

### Diodes  

Diode is a kind of component with two polarities: one is for positive and the other is negative. It allows current move from the positive end to the negative end only. We can regard it as an electronic check valve.   
For common diode, we can judge from the color of tube for its polarity. The terminal with white color is negative polar.  

![](https://i.imgur.com/b1g3bBJ.jpg)   

### Alligator Clip Wires  

Similar to the usage of jumper cable, alligator clip wire is used when some components are not suitable to use jumper cable for connection.    

![](https://i.imgur.com/EfkdKmY.jpg)  

In this experiment, we use alligator clip wire to connect our motor.   

![](https://i.imgur.com/Oj1aUaf.jpg)  


## Hardware Connection      
---  

Please complete hardware connection according to the picture below.  

![](https://i.imgur.com/2MZA7bj.jpg)  

The drive current on Micro:bit IO port is too feeble to connect motor directly. At this time, we have to use a triode to amplify the current of IO port.  The circuit diagram of using triode to amplify current on IO port is very similar to the circuit diagram of our last chapter “Micro:bit Experiment 09:Buzzer —— Elecfreaks Mirco: bit Starter Kit Course”. The only difference is the motor has two diodes on its both terminals. And the diode in this circuit is called Freewheel Diode.   

Within the motor, there has a coil. When current flow through the coil, it will produce induced electromotive force on the both terminals. When current disappeared, the induced electromotive force will generate backward voltage to the components in the circuit. It might damage these components. Freewheel diode connects the two terminals of the coil in anti-parallel. When we cut off the power supply of the inductance coil, the induced electromotive force will not disappear immediately. And the residual force will release by diode.   This is a typical design of protection.     

Below is the partial circuit diagram of the usage of triode in amplifying the IO port current.   

![](https://i.imgur.com/e4YL3hx.jpg)  

After connection, you will see:   

![](https://i.imgur.com/RwH4uNp.jpg)   


## Programming    
---  

Please open Microsoft Makecode, write your code in the edit area. I would like to suggest you program by yourself first.   

Of course, you can download the whole program from the link below.  

Link of the whole program: https://makecode.microbit.org/_Kid26LToz2mU  


## Code Explain    
---  

In the software aspect, this experiment do not have new knowledge points. The thing we have to pay special attention to is P1 port connect button. Under brick “on start”, we have to set P1 to be up mode, or it can not recognize button signal properly.   

![](https://i.imgur.com/7lkYPlA.jpg)  


## Experiment Result  
---  

Press down the button, the motor starts rotate. Press again, it will stop move.   
Attention: The voltage of micro:bit power source is low. It is 3V only. Press down the button, the motor may not start. If this happened, please stir the fan blade of the motor so that it can move properly.   

![](https://i.imgur.com/UeWUgLi.gif)  


## Think  
---  

If we want to use potentiometer to control the motor speed, then how to design circuit and program. We look forward to your comments and further discussions with us.     



## FAQ  
---  

   

