## Fireflies

Turn your micro:bit into fireflies.

[https://youtu.be/ZGvtnE1Wy6U](https://youtu.be/ZGvtnE1Wy6U)

### How do Fireflies synchronize?
Go to [http://ncase.me/fireflies/](http://ncase.me/fireflies/) and read about the fireflies synchronization phenomenon.

Code the firefly
We want to create virtual fireflies using multiple micro:bits (each micro:bit acts as a firefly). Let’s review some of the key points from the article:

#### “Each firefly has its own individual internal clock…”

A clock in this case is like a counter, so we will start by adding a clock variable to our program.

![](https://i.imgur.com/XJKatWW.png)


#### “…and every time the clock ‘strikes twelve’, it flashes.”
We can use a `||basic:forever||` loop to repeat code that increments the clock. When the clock reaches “noon” (let’s pick 8 as noon), we turn on the screen briefly (by using the game score animation).

![](https://i.imgur.com/vlYr02V.png)

#### When you see a nearby firefly flash, nudge your clock a little bit forward
The micro:bit can send radio messages to a neighbor micro:bit. We can use these messages to simulate the “flashes” of light.

When a firefly flashes, it also sends a number over radio using `||radio:radio send number||`:

![](https://i.imgur.com/LDRmbHc.png)

When a firefly receives a radio packet and it is not sending packet , it increments its clock by one:

![](https://i.imgur.com/05EAk12.png)

### Put it all together

[https://youtu.be/XzZeB4yYnEw](https://youtu.be/XzZeB4yYnEw)

Download this program on as many micro:bits as you can find and try it out in the dark!

Note: We’ve added a `||radio:radio set group||` block to specify which group the firefly will communicate on.

![](https://i.imgur.com/dwFbr6R.png)

Link: [https://makecode.microbit.org/_VckJJgaHgRjr](https://makecode.microbit.org/_VckJJgaHgRjr)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_VckJJgaHgRjr" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>
