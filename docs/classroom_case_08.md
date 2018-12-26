## Hack your headphones

Build your own micro:bit music player using headphones.

![](https://i.imgur.com/2bhw6Gq.png)

Duration: ~15 minutes.

### Materials

- micro:bit, battery holder and 2 AAA batteries
- Headphones
- Crocodile clips

No crocodile clips!?!?! Use wires or aluminium foil!

### Activities

Did you know you could attach your headhpones to the micro:bit to generate sounds?

#### Step 1

![](https://i.imgur.com/6ltCp4R.png)

Using the 1st crocodile clip, connect the end of the crocodile clip onto GND pin on the micro:bit.

#### Step 2

![](https://i.imgur.com/umFmgVC.png)
![](https://i.imgur.com/XqZM9Zj.png)

Using the 2nd crocodile clip, connect the end of the crocodile clip onto the 0 pin on the micro:bit.

#### Step 3

![](https://i.imgur.com/wtBxTrW.png)

Using the 1st crocodile clip, connect the second end of the crocodile clip onto based of the headphone jack. The base of your headphone jack is considered the ground so it is connected to the GND of the micro:bit.

#### Step 4

![](https://i.imgur.com/ueGMdF1.png)
![](https://i.imgur.com/GHs8QJS.png)

Using the 2nd crocodile clip, connect the second end of the crocodile clip onto the tip of the headphone jack. The tip of your headphone jack feeds into the right speaker on the headphone. You connect from the micro:bit pin 0 to the tip of the right side of your headphone. Use the tip of the headphone jack to play sounds.

#### Step 5

![](https://i.imgur.com/Cmarujh.png)

You hacked your headphones!

### Code

Have you ever tried to making beat box sounds based on the light level? Let’s try making a beatbox with code!

Let’s start by adding a variable where you can store data. Then rename the variable to “light”. Then set the value of the variable to the block `light level` from the Input drawer. This will gets the `light level` from 0 (dark) to 255 (bright). The light is measured by using various LEDs from the screen. Modify your code so that your code looks like this.

![](https://i.imgur.com/SvSpJNF.png)

Link: [https://makecode.microbit.org/_C656hCHCwAiF](https://makecode.microbit.org/_C656hCHCwAiF)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_C656hCHCwAiF" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

We want to play music on button pressed in order to register an event handler that will execute whenever when you run a script and click `on button pressed` on the simulator. We must start by opening the Input drawer and adding on button pressed A. Then add a block `rest` to plays nothing for a `1/16` beat. Modify your code so that your code looks like this.

![](https://i.imgur.com/i2EpcRw.png)

Link: [https://makecode.microbit.org/_5zP1puK2D5sL](https://makecode.microbit.org/_5zP1puK2D5sL)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_5zP1puK2D5sL" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

We click on the Logic drawer then insert a `if do` that will conditionally run code depending on whether the Boolean condition is true or false. Then insert the variable `light` into the first part of the inequality. The variable “light” will appear in the Variables drawer. Finally, we insert 25. Modify your code so that your code looks like this. If the `light level` is `less than` 25, play `ring tone C`. If this conditions is not true, play `ring tone A`.

![](https://i.imgur.com/skDhw87.png)

Link: [https://makecode.microbit.org/_KbVhzqDssHmc](https://makecode.microbit.org/_KbVhzqDssHmc)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_KbVhzqDssHmc" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

We click on the Logic drawer then insert a `less than` sign into the first `if` conditional that will conditionally run code depending on whether the Boolean condition is true or false. Continue this logic to continue with these conditional statements. Click on the Logic drawer. Then we want to add additional conditional statements by clicking on the gear to the left of the `if`. Add 05 `else if` and 01 `else` inside the `if do` block structure. If the `light level` is `less than` 50, play `ring tone D`. If the `light level` is `less than` 100, play `ring tone E`. If the `light level` is `less than` 150, play `ring tone F`. If the `light level` is `less than` 180, play `ring tone G`. If these conditions are not true, `ring tone A`.

![](https://i.imgur.com/yoA9L45.png)

Link: [https://makecode.microbit.org/_6qecgRgKC1fh](https://makecode.microbit.org/_6qecgRgKC1fh)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_6qecgRgKC1fh" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

click **Download** and run your code on the micro:bit.
