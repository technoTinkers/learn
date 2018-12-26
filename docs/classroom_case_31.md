## Compass

Welcome! This guided tutorial will show you how to program a script that displays which direction the micro:bit is pointing. Let’s get started!

![](https://i.imgur.com/uH9kHQH.png)

Display the direction that the micro:bit is facing using the compass.

### Step 1

Create a loop that will continuously update the reading of the compass.

![](https://i.imgur.com/ZvGUMpi.png)

### Step 2

Store the reading of the micro:bit in a variable called `degrees`.

![](https://i.imgur.com/xvMBxR1.png)

### Step 3

If `degrees` is less than `45` or greater than `315`, then the compass heading is mostly pointing toward **North**. Display `N` on the micro:bit.

![](https://i.imgur.com/BGql1YN.png)

### Step 4

If `degrees` is less than `135`, the micro:bit is mostly pointing **East**. Display `E` on the micro:bit.

![](https://i.imgur.com/RwGe218.png)

### Step 5

If `degrees` is less than `225`, the micro:bit is mostly pointing **South**. Display `S` on the micro:bit.

![](https://i.imgur.com/cAPmeL6.png)

### Step 6

If none of these conditions returned true, then the micro:bit must be pointing **West**. Display `W` on the micro:bit.

![](https://i.imgur.com/BjtZz9M.png)

Link: [https://makecode.microbit.org/_DaaYzF7Xmbfd](https://makecode.microbit.org/_DaaYzF7Xmbfd)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_DaaYzF7Xmbfd" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>






