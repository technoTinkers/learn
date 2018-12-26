## Introduction
---
Octopus BME280 Pressure Sensor is an electric brick, which has integrated temperature sensor, air pressure sensor and humidity sensor onboard. We can use it to measure humidity, temperature and air pressure, or even to calculate the altitude according to the measured air pressure.    


## Features 
---
- Low power consumption and small size. 
- 3mm standard positioning hole. 
- Rated 3.3v power supply, which is enough to support micro:bit.
- Support I2C and SPI protocol. 


## Parameters
---
Item | Parameter 
:-: | :-: 
Product Name |Octopus BME280 Pressure Sensor
Version No.|V1.0
SKU| EF04087
Working Voltage |DC 1.2V-3.6V
Connectors |IIC（slave mode 3.4MHz）or SPI（3-wire or 4-wire slave mode 10MHz）
Relative Humidity Range |0%～100%, response time > 1s
Humidity Tolerance |±2%；Humidity Hysteresis: ±1%；Resolution Rate: 0.8%
Air Pressure Measure Range |300～1100hPa
Air Pressure Tolerance |±1hPa, Resolution Rate: 0.18Pa
Temperature Measure Range|0℃～65℃
Temperature Tolerance |±0.5℃; Max: ±1℃; Resolution Rate: 0.1℃
Size |31 x 23 mm


## Dimensions 
---
![](https://i.imgur.com/ZCHyqrg.png)


## Wire Connection
---
![](https://i.imgur.com/TGFmmNb.png)


## Quick Start 
---  
### Hardware Connection 
Connect the sensor to I2C connector on octopus:bit using a jumper cable.
Insert micro:bit into the edge slot of octopus:bit. 

### Programming  

Click to open [Makecode](https://makecode.microbit.org/), write your code to read air pressure values and display it on the micro:bit screen.
Link of the whole program: [https://makecode.microbit.org/_cPih8ybrDXuz](https://makecode.microbit.org/_cPih8ybrDXuz)

You can also download it from the page below.
<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_cPih8ybrDXuz" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Result  
Air pressure values are scrolling on the micro:bit screen with unit mb.

## FAQ
---
