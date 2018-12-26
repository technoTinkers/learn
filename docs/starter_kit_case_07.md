![7](https://i.imgur.com/fMCJitN.jpg)

## Introduction    
---  

Temperature sensor is a kind of sensor that can feel temperature and transfer it into output data. Temperature sensor is the core component of temperature gauges and instruments. It has multiple categories. In this experiment, we are going to learn analog temperature sensor--TMP36 and display its data on the screen of Micro:bit.  


## Components List  
---  

### Hardware：  

1 x [micro:bit Board](http://www.elecfreaks.com/estore/bbc-micro-bit-board-for-coding-programming.html)  
1 x Micro-B USB Cable  
1 x [microbit Breadboard Adapter](http://www.elecfreaks.com/estore/microbit-breadboard-adapter.html)  
1 x [Transparent Breadboard - 83 * 55 mm](http://www.elecfreaks.com/estore/transparent-breadboard-83-55-mm.html)  
1 x TMP36 Temperature Sensor  
1 x [Breadborad Jumper Wire 65pcs Pack](http://www.elecfreaks.com/estore/breadborad-jumper-wire-65pcs-pack.html)  

**Tips: If you want all components above, you may need [Elecfreaks Micro:bit Starter Kit](http://www.elecfreaks.com/estore/elecfreaks-micro-bit-starter-kit-795.html).**  

![](https://i.imgur.com/W4tseua.jpg)  

### Software:  

[Microsoft Makecode Online Editor](https://makecode.microbit.org/)  


## Major Components Introduction  
---  

### TMP36  

TMP36 is a kind of analog temperature sensor. Its output voltage and temperature forms a linear relationship. That means higher temperature will have bigger output voltage.  

![](https://i.imgur.com/SDoXRcM.jpg)  

**Note:**  
When we look at the front side marked “TMP36”, the left footer of the core is VCC, middle is Vout, and the right footer is GND. You can’t connect it wrong or the components connected might be damaged.   

![](https://i.imgur.com/P6ZkUDh.jpg)  

Here’s the curve chart for output voltage of TMP36 changing with temperature:  

![](https://i.imgur.com/5R7izFc.jpg)  
![](https://i.imgur.com/U2c4qdp.jpg)  
 
We can know from the above chart that the temperature formula is:  

Temperature（℃）=(Output Voltage（mV）-500)/10  


## Hardware Connection  
---

Please complete hardware connection according to the picture below.  
![](https://i.imgur.com/HnUeLBR.jpg)  

After connection, you will see:  
![](https://i.imgur.com/IAor80B.jpg)  


## Programming  
---  

Open Microsoft Makecode, write your code in the edit area. I would like to suggest that you program by yourself first.  
Of course, you can see the whole program in the link below directly. Just click “Edit” on the top right corner of the interface, then click “Download” on the bottom right corner to download code into Micro:bit directly.   

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_7MLCRdhek0mJ" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  

Link of the whole program: [https://makecode.microbit.org/_Csja8Y2koEyi](https://makecode.microbit.org/_Csja8Y2koEyi)


## Code Explain  
---  

**map**  

Remaps the specified value from one range to another. This function maps the value of **from low** to the value of **to low**, the value of **from high** to the value of **to high**, and intermediate values to intermediate values.  
This function does not constrain values to the ranges, because out-of-range values are sometimes intended and useful. If you need to limit a range, you can use the **Math.clamp** function before or after calling this function.  

![](https://i.imgur.com/oCPoKPs.jpg)   

In our program, we have to use brick **Map** to transfer the read-out analog data into voltage(mV).   
If **analog read** value is 0 to 1023, so **from low** is 0, **from high** is 1023.  
The basic voltage of Micro:bit is 3.3V, i.e. 3300Mv. So **to low** is 0, **to high** is 3300.  

![](https://i.imgur.com/b8aM1qv.jpg)  

Temperature（℃）=(Output Voltage（mV）-500)/10  
Then according to the formula above to calculate temperature value.   


## Experiment Result
---

micro:bit screen displays the present temperature value. 
![](https://i.imgur.com/b0w5PkN.gif)


## Think  
---

In this experiment, Micro:bit displays the centigrade temperature. If we want to display the Fahrenheit temperature, then how to design circuit and program? We look forward to your comments or further discussion with us.


## FAQ
---

   

