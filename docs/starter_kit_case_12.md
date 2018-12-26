![12](https://i.imgur.com/5RJ1KJn.jpg)     

## Introduction    
---  

Micro:bit has integrated multiple sensors including accelerometer. Today, we are going to use accelerometer to make an level device and display the inclination on NeoPixel ring in bar chart format.   


## Component List      
---  

### Hardware:  

- 1 x [micro:bit Board](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)  
- 1 x Micro-B USB Cable  
- 1 x [micro:bit Breadboard Adapter](http://www.elecfreaks.com/estore/microbit-breadboard-adapter.html)  
- 1 x [Transparent Breadboard - 83 * 55 mm](http://www.elecfreaks.com/estore/transparent-breadboard-83-55-mm.html)  
- 1 x 8 RGB LED NeoPixel Ring  
- 1 x [Breadborad Jumper Wire 65pcs Pack](http://www.elecfreaks.com/estore/breadborad-jumper-wire-65pcs-pack.html)  

**Tips: If you want all components above, you may need [Elecfreaks Micro:bit Starter Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-starter-kit-795.html).**  

![](https://i.imgur.com/W4tseua.jpg)  

### Software:  

[Microsoft Makecode Online Editor](https://makecode.microbit.org/)  


## Major Component Introduction    
---  

**Accelerometer**  

There is an accelerometer on your micro:bit which detects the speed change of micro:bit. It converts analog information into digital form that can be used in micro:bit programs. Output is in milli-g. The device will also detect a small number of standard actions, e.g. shake, tilt and free-fall.  
 
![](https://i.imgur.com/kzqAOK4.jpg)  

The corresponding X, Y, Z axle direction of accelerometer are showed below:   

![](https://i.imgur.com/FQ6zBkH.jpg)  


## Hardware Connection    
---  

Please complete hardware connection according to the picture below.  
![](https://i.imgur.com/NPvcrUo.jpg)  

After connection, you will see:  
![](https://i.imgur.com/SOD2TLb.jpg)   


## Programming      
---  

Open Microsoft Makecode, write your code in the edit area. I would like to suggest you program by yourself first.  

Of course, you can download the whole program from the link below.  

[https://makecode.microbit.org/_R2yHPUecyh2i](https://makecode.microbit.org/_R2yHPUecyh2i)   


## Code Explain    
---  

**show bar graph**  
Display the value with bar chart format just similar to plot bar graph.  

**Acceleration**  
Get the acceleration value (milli g-force) in one of three dimensions, or the combined force in all directions (x, y, and z).  


## Experiment Result    
---  

With the inclination of micro:bit, LED bead on Neopixel ring gradually illuminated one by one. The bigger inclination angle, more LED beads will be illuminated.  

![](https://i.imgur.com/IdpGKQJ.gif)  


## Think     
---    

In this case, we have judged the inclination of one direction(X axle) only. If we want to test the inclination of a flat surface( say XY flat surface), then how to design circuit and program. We look forward to your comments and further discussions with us.   



## FAQ  
---  

   

