![14](https://i.imgur.com/NkZTTdv.jpg)  

## Introduction    
---  

In our blog “Micro:bit Experiment 04: Photocell — Elecfreaks Mirco: bit Starter Kit Course”, we had connected a photocell externally to sense the light. Actually, micro:bit has integrated a light detection device internally. Today we are going to use the internal light sensor to do an experiment. We will light a rainbow LED ring when the light in the outer environment is comparatively dark.     


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

Microsoft Makecode Online Editor  


## Major Component Introduction    
---  

You might be curious how micro:bit senses light without any light sensor. Let’seea paragraph about display on micro:bit website:  

The display is a 5x5 array of LEDs. It is connected to the micro:bit as a 3x9 matrix. Runtime software repeatedly refreshes this matrix at a high speed, such that it is within the user persistence of vision range, and no flicker is detected. This LED matrix is also used to sense ambient light, by repeatedly switching some of the LED drive pins into inputs and sampling the voltage decay time, which is roughly proportional to ambient light levels.  

![](https://i.imgur.com/1JzFZG3.jpg)  

That’s really amazing! Except for its light emitting ability, micro:bit can sense light!Because LEDs are so commonly used as light emitters it is easy to forget that they are fundamentally photodiodes, and as such are light detectors as well.The function may be implemented with no additional hardware cost if incorporated in the LED driver circuit.  


## Hardware Connection    
---  

Please complete hardware connection according to the picture below.  
![](https://i.imgur.com/fKgQRoW.jpg)   

After connection, you will see:  
![](https://i.imgur.com/Hacl6BL.jpg)  


## Programming    
---  

Open Microsoft Makecode, write your code in the edit area. I would like to suggest you program by yourself first.  
Of course, you can download the whole program from the link below.   

[https://makecode.microbit.org/_Ws5gzMYvvM2x](https://makecode.microbit.org/_Ws5gzMYvvM2x)  


## Code Explain    
---  

**Light Level **  
Find the light level (how bright or dark it is) where you are. The light level 0 means darkness and 255 means bright light. The micro:bit measures the light around it by using some of the LEDs on the LED screen.  

**Clear**  
Set the color value of all RGB LED beads to be 0.  

Note:   
Use LED as a light sensor is not sensitive. It requires comparatively brighter light so that light level can change.  


## Experiment Result    
---  

When in darkness, the LED ring will be turned on; while in brightness, the LED ring will be turned off.  

![](https://i.imgur.com/F9B9ySD.gif)  


## Think    
---  

If we want to rotate the rainbow color after the ring was illuminated, then how to design circuit and program? We look forward to your comments and further discussions.  



## FAQ
---

   

