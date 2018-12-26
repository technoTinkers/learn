## The Watch

Build your own micro:bit watch from an old pair of jeans and T-shirt!

![](https://i.imgur.com/RnUOmT3.png)


### Materials

- micro:bit, battery holder and 2 AAA batteries
- Old T-shirt
- Old Jeans
- Velcro with sticky back – 5cm x 5cm
- Double-sided tape – 22cm x 5cm. You can find carpet tape in your local hardware shop
- Ruler and pen
- Scissors


### Activities

### The Watch - Make

Make a watch for your micro:bit.

Duration: ~30 minutes

#### Materials

- micro:bit, battery holder and 2 AAA batteries
- Old T-shirt
- Old Jeans
- Velcro with sticky back – 5cm x 5cm
- Double-sided tape – 22cm x 5cm. You can find carpet tape in your local hardware shop
- Ruler and pen
- Scissors

#### Steps

##### Step 1

![](https://i.imgur.com/BWWBDEU.png)

Using the ruler and pen, mark a rectangle of more or less 26cm x 5cm on the T-shirt. Don’t worry if you don’t get it quite right, we’ll tidy things up later on.

##### Step 2

![](https://i.imgur.com/7zeidiA.png)

Cut the rectangle using the scissors. Don’t worry about the quality of the cut, we’ll trim it later on.

##### Step 3

![](https://i.imgur.com/SbyrBnr.png)

Cut a piece of cloth from the pair of jeans. Cut straight by the seam.

![](https://i.imgur.com/xmyzfYB.png)

##### Step 4

![](https://i.imgur.com/RlOGe6B.png)

Using the ruler and pen, mark a rectangle of 22cm x 5cm (adults should use 24cm x 5cm) on the jeans cloth.

##### Step 5

![](https://i.imgur.com/4LdJFTw.png)

Stretch the cloth using your hands and apply the double-side tape on the rectangle marked on the jeans. You might need the help of a friend to achieve this step. Don’t worry if the tape is larger than the rectangle, we will trim it later. Make sure to apply pressure to the tape to secure it firmly.

##### Step 6

![](https://i.imgur.com/jHYb0wu.png)

Using the scissors, cut the rectangle of jeans.

##### Step 7

![](https://i.imgur.com/Wiz0YFf.png)

Peal the tape protective layer from the rectangle.

##### Step 8

![](https://i.imgur.com/o8qd9KA.png)

Place the micro:bit pins on the tape at more or less 7 cm from the left border. Then lower the micro:bit on the tape and press gently.

##### Step 9

![](https://i.imgur.com/Ayz7NKs.png)

Connect the battery holder and place it on the right of the micro:bit. Tuck the cables away on the tape to protect them.

##### Step 10

![](https://i.imgur.com/1iqWr3b.png)

Stick the T-shirt rectangle from the top of the micro:bit, over the battery cables.

##### Step 11

![](https://i.imgur.com/Eizvz4d.png)

Use your fingers to push the T-shirt cloth under the micro:bit to give access to the micro-USB plug.

##### Step 12

![](https://i.imgur.com/tDKSbvq.png)

Place the T-shirt over the battery holder and stick it up to the end.

##### Step 13

![](https://i.imgur.com/X83yK2m.png)

Turn over the watch and cut the extra T-shirt material.

##### Step 14

![](https://i.imgur.com/FXGd7aJ.png)

Stick the T-shirt cloth on the other side of the watch. Lift the micro:bit pins to slide the cloth under and leave them free from the tape.

##### Step 15

![](https://i.imgur.com/IBTiAoH.png)

Turn over the watch and cut left over T-shirt cloth.

##### Step 16

![](https://i.imgur.com/9wRaKOv.png)

Cut a 5cm x 5cm square of Velcro loops.

##### Step 17

![](https://i.imgur.com/6Fk7bWM.png)

Cut a 5cm x 5cm square of Velcro hooks.

##### Step 18

![](https://i.imgur.com/kuXfq5Q.png)

Stick the Velcro hooks on the right side of the battery holder on the T-shirt cloth.

##### Step 19

![](https://i.imgur.com/SyWC5Qi.png)

Stick the Velcro loops on the other end on the jeans fabric.

##### Step 20

Trim any leftover fabric, threads or tape.

##### Step 21

![](https://i.imgur.com/kNVZnJL.png)

Your watch is ready! We’ll now add code to the micro:bit to make it keep time for real!

### Code  

Let’s make a counter for your watch to remember all the motions you make when you walk or move your arm.

Duration: ~5 minutes

#### Make a count variable

We need a variable to keep track of how many motions you make.

- Go into **Basic** in the toolbox and pull an `on start` on to the workspace.
- Ok, in **Variables** click on `Make a Variable`. Name the variable as `motions`. Drag out a `set to` block and change the name with the dropdown to `motions`. Place the variable into the `on start` block.
- Let’s show that there are no motions counted yet. Get a `show number` from **Basic** and put it after the variable. Now, change the `0` to the `motions` variable from the **Variables** category in the toolbox.

![](https://i.imgur.com/Fd9IRN8.png)

Link: [https://makecode.microbit.org/_KgsJbE2e35up](https://makecode.microbit.org/_KgsJbE2e35up)

#### Count your movements

Ok, now we’ll count and show all of your movements.

- Get an `on shake` block from **Input** and place it in the workspace.
- To count each of your movements, get a `change by` and place it in the `on shake`. Change the variable from `item` to  `motions`.
- Grab another `show number` and put it at the bottom of the `on shake`. Find `motions` again back over in **Variables** and replace the `0` with it.

![](https://i.imgur.com/ERw27X6.png)

Link: [https://makecode.microbit.org/_H92U8JYPAgrU](https://makecode.microbit.org/_H92U8JYPAgrU)

#### Reset!

If we want to start over from zero, then we need to have a way to reset the motion count. Let’s use one of the buttons to do it.

- Go over to Input and get an `on button pressed`. Place a `set to` inside. Change the variable name to `motions`.
- Grab another `show number` and change the `0` to the a `motions` variable.

![](https://i.imgur.com/aERnT2G.png)

Link: [https://makecode.microbit.org/_WLoMUXMqwJkD](https://makecode.microbit.org/_WLoMUXMqwJkD)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_WLoMUXMqwJkD" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

#### Finished!

Yeah! You’re ready to count your movements. Press the `Download` button to move the code to the micro:bit. Walk around, move you arm, and watch it count! Press the **A** button if you want to start over.

#### More watch coding projects

Are you up for a bigger challenge? How about making your watch turn into a countdown timer or even a real digital watch? Take a look at some other coding projects for the micro:bit watch:

- Countdown timer
- Digital watch

### Acknowledgements

Artistic design by Melinda Hoeneisen.
