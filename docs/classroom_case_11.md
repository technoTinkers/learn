## Wallet

Make a micro:bit wallet with this guided tutorial!

![](https://i.imgur.com/ciV3sWw.png)

### Activities

Duration: ~30 minutes

#### Materials

- Paper sheet
- Tape (masking, duct tape, and/or packing tape)
- Scissors
- 1 micro:bit, battery holder and 2 AAA batteries
- Marker or pen

![](https://i.imgur.com/dRyw9dO.png)

#### Duct tape sheet

Let’s start by building a duct tape sheet.

Position the paper sheet on the workbench and place lines of tape over it. Make sure to overlap each layer to avoid seeing gaps of papers. In case of mistake, add tape!

![](https://i.imgur.com/MLLiqch.png)

Cover the entire paper sheet with tape. Don’t hesitate to use various colors or patterns!

![](https://i.imgur.com/ICQMJ3b.png)

Unstick the sheet from the workbench carefully to avoid ripping out the tape and turn it over.

![](https://i.imgur.com/rhZjX7n.png)

Fold the remaining tape sections on the sides towards the center.

![](https://i.imgur.com/uv1CSgY.png)

Great job, your duct tape sheet is ready! Let’s get onto the next step.

![](https://i.imgur.com/QLYjSez.png)

#### Card Hole

We need to cut a hole in the center of the sheet to allow storage of coins and cards inside the wallet.
Gently fold the sheet in half.

![](https://i.imgur.com/4zsy9Lo.png)

Gently foldy the other way.

![](https://i.imgur.com/ZmW2S80.png)

Place the duct tape roll on the inside corner. This will determine the size of the hole.

![](https://i.imgur.com/cN1KZCC.png)

Use your marker and trace around the roll.

![](https://i.imgur.com/QpMnHhc.png)

Use your scissors and cut along the line you’ve just traced while keeping the sheet folded.

![](https://i.imgur.com/YOGU8UZ.png)

Well done! The hole is done and perfectly centered!

![](https://i.imgur.com/evIbMwQ.png)

#### Mounting the micro:bit

We are going to cut a hole for the micro:bit screen and buttons on the front of the wallet.
Place the micro:bit on the back of the sheet.

![](https://i.imgur.com/Izu1i3d.png)

Mark the contour of the micro:bit on the sheet with your marker. Don’t worry about little mistakes.

![](https://i.imgur.com/0zKOWN3.png)

Mark ticks at the location of each corners of the screen as shown on the picture.

![](https://i.imgur.com/ymstbVn.png)

Use the micro:bit as a ruler to trace a line between the ticks.

![](https://i.imgur.com/laIrYhb.png)

Fill the inside square with your marker, you will need to cut it out later.

![](https://i.imgur.com/4XncU6x.png)

Mark the ticks along the button using the same procedure.

![](https://i.imgur.com/GxOJ75f.png)

Fill the button square as well so that you clearly know what to cut or not.

![](https://i.imgur.com/x365heM.png)

Fold the sheet over the center of the darken area and cut out a triangle large enough to squeeze a blade of the scissors.

![](https://i.imgur.com/PV8rsgx.png)

Starting from the small hole, work your way through cutting out the darkened area.

![](https://i.imgur.com/UzODn1O.png)

Eventually, the opening should look like a rectangle with a square in the middle.

![](https://i.imgur.com/lYZRTce.png)

Try mounting the micro:bit and cutting more material as needed.

![](https://i.imgur.com/9Up768n.png)

Put a generous layer of tape on the back of the micro:bit to stick it on the wallet.

![](https://i.imgur.com/lZga9a2.png)

Attach the battery to the micro:bit. You are done for this step!

![](https://i.imgur.com/waRUrOa.png)

#### Folding

The last step is to fold the sheet and tape the sides to get a wallet.
Start form the sheet facing paper up and fold the sheet over the large hole in the center.

![](https://i.imgur.com/urYDR82.png)

Fold another time until the large hole is visible.

![](https://i.imgur.com/ccXPoE3.png)

Apply a layer of tape on the side with the tape overlapping half over the wallet.

![](https://i.imgur.com/42q4zNH.png)

Flip over the wallet carefully.

![](https://i.imgur.com/kLl2MXS.png)

Fold the remaining tape over the wallet and cut the sides with the scissors.
Tuck in the battery in the pocket inside the wallet and make sure the cables are out of the way.

![](https://i.imgur.com/XSIm9n8.png)

Apply the tape on the side using the same procedure.

![](https://i.imgur.com/LssuuuD.png)

That’s it! You have an micro:bit wallet!

![](https://i.imgur.com/npazhiV.png)

#### Protecting those buttons!

The buttons of the micro:bit are left vulnerable to being ripped out.

![](https://i.imgur.com/cUZj5Km.png)

If you plan to make an extensive use of your wallet without using the buttons, you might want to consider to protect the buttons with additional tape.

![](https://i.imgur.com/nQgf9Sv.png)

The wallet is ready, we just have to add some code into the micro:bit to make it alive.

### Code

#### Simple animation

Let’s start by using a combination of forever and show leds to create animation:

![](https://i.imgur.com/evjSH5s.png)

Link: [https://makecode.microbit.org/_43kDbfdftDdm](https://makecode.microbit.org/_43kDbfdftDdm)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_43kDbfdftDdm" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

Download this code to your micro:bit and try it out.

#### Turn off animation in the pocket

If the wallet is in your pocket, you should turn off the LEDs to save energy.

How do we know that the wallet is in the pocket? It is really dark in there… We can use the [light level](https://makecode.microbit.org/reference/input/light-level) to detect this!

Using an [if statement](https://makecode.microbit.org/blocks/logic/if), we can test if the level of light is sufficient to turn on the screen. Otherwise, we turn off the screen for a few second to save energy.

![](https://i.imgur.com/TBOWzLA.png)

Link: [https://makecode.microbit.org/_EHkUqiKdWRq8](https://makecode.microbit.org/_EHkUqiKdWRq8)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_EHkUqiKdWRq8" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### References

The wallet built in this activity is inspired from the duct tape wallet in A Kid’s Guide to Awesome Duct Tape Projects: How to Make Your Own Wallets, Bags, Flowers, Hats, and Much, Much More!
