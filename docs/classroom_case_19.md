## Mood Radio

![](https://i.imgur.com/wkP2X5J.png)

This project uses the radio to share your mood with other micro:bits. When you press `A`, your friends will see a **smiley** face. When you press `B`, they will see a frowny face.

### Sending a smiley
The micro:bit can’t understand mood but it is pretty good with numbers. In fact, it can send numbers between micro:bits using the radio antenna, just like a phone can send text messages.

Let’s add blocks that send a number when button `A` is pressed. We assume that `0` is the “mood code” to send for smiley.

![](https://i.imgur.com/dlZ8JkU.png)

### Receiving a smiley
We add a `||radio:on radio received||` block that will run code whenever a new “mood” message comes in. The `receivedNumber` variable contains the numeric value that was sent. Since we’ve decided that `0` is **smiley**, we add a conditional `||logic:if then||` statement to show this icon.

![](https://i.imgur.com/39sPdHn.png)

### Sending a frowny
Adding another mood to our messaging app done in a similar way. We decide that the “mood code” of `1` means **frowny**. We can add a `B` button event that sends that code.

![](https://i.imgur.com/Il7ZAB3.png)

If the `||radio:on radio received||` block, we add another conditional `||logic:if then||` statement to handle the **frowny** “mood code”.

![](https://i.imgur.com/nTRQbWo.png)

Link: [https://makecode.microbit.org/_PUz53eRJLKWR](https://makecode.microbit.org/_PUz53eRJLKWR)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_PUz53eRJLKWR" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

That’s it. Download your code to multiple micro:bits and try it out!

### Challenges

Try adding a new code and use the `||input:on shake||` event to send it.

### Full sources

![](https://i.imgur.com/WxB66i2.png)

Link: [https://makecode.microbit.org/_9L65tCd0EF71](https://makecode.microbit.org/_9L65tCd0EF71)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_9L65tCd0EF71" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


