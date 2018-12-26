![](https://i.imgur.com/krV05be.jpg)
## Goal
---


- Make an auto window.

## Materials
---

- 1 x [Smart home Kit](https://www.elecfreaks.com/estore)
- 1 x corrugated board

## Background
---
### What is an auto window ? 
-  Noise pollution is a common problem in our life. When the value of noise higher than 70dB, it is will impact our health. We will design a smart window and door using micro:bit.

### Auto window operation
- Using micro:bit detect wether the the value of noise higher than 70dB and control servo to closing the door and the window.

![](https://i.imgur.com/g674G7D.png)

## Practical operation
---
Materials: corrugated board and cutter

![](https://i.imgur.com/PuJE7uj.jpg)

Build as below picture：

Front side：

![](https://i.imgur.com/sPzbv3R.jpg)

Back side：

![](https://i.imgur.com/hvyJ9Ow.jpg)

Paste devices as below piture:

![](https://i.imgur.com/oSZrVnY.jpg)


## Hardware connect
---
![](https://i.imgur.com/hOlsKaR.png)






## Software
---
[makecode](https://makecode.microbit.org/#)

[Edge Connector Data Sheet](https://www.elecfreaks.com/learn-cn/Edge_Connector_Data_Sheet/)



## Programming
---
### Step 1
Go to MakeCode page, click Advanced in the code block and click on Extensions.

![](https://i.imgur.com/2qCyzQ7.png)

We need to add a new codebase for programming of smart home. Finding “Add Package” in the bottom of code block and click it. Then a message box will show up, search “smart home"， and download this new codebase.

![](https://i.imgur.com/QR2s7LD.png)

Note：If there is a hint says some codebase will be deleted because of incompatibility. Don't worry. You could go ahead as the hint or build a new item in item menu bar.


### Step 2

Drag on start on from Basic, snap into servo write pin, set P1 to 0.


![](https://i.imgur.com/cAwF1Yb.png)

### Step 3

Snap set item to into forever, assignment value of noise to noise variables.

![](https://i.imgur.com/V2ptpb6.png)

### Step 4

If value of noise > 70dB, snap into servo write pin,set P1 to 0 and the window be closed.

![](https://i.imgur.com/RGf9xF5.png)

### Step 5
If value of noise < 70dB，snap into servo write pin,set P1 to 100 and the window be opened.

![](https://i.imgur.com/5VmbsGn.png)
### Programming

Make code：[https://makecode.microbit.org/_PyELU94qWPYD](https://makecode.microbit.org/_PyELU94qWPYD)

You also could directly download program visit website as below:

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_PyELU94qWPYD" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>  
---

## Result
---
micro:bit driving servo open the window when value of noise > 70dB.

Front side：
![](https://i.imgur.com/2JsAZKA.jpg)

Back side：
![](https://i.imgur.com/rGIkINB.jpg)

## Think
---
How to know wether open the window on room temperature.

## Questions
---


## More information   
---

