## Rock Paper Scissors

Make the Rock-Paper-Scissors game on your micro:bit and challenge your friends.

![](https://i.imgur.com/9MHnzYj.png)

Duration: ~20 minutes.

### Materials

- micro:bit, battery holder and 2 AAA batteries
- Roll of duct tape (maybe 2 rolls if you want another color)
- Velcro

### Activities

#### Setting

##### Step 1 - Cut the pieces of tape

Cut 2 Pieces of Duct Tape about 9-10 inches long. Press the sticky sides together to form one piece of tape (this is tricky!). This makes the band of your wrist cuff.

![](https://i.imgur.com/NwUoy2N.png)

##### Step 2 - Attach the micro:bit and battery pack

Mount the micro:bit in the center of your wrist cuff band by looping a piece of duct tape around in a circle.

![](https://i.imgur.com/Fvg8pL7.png)

Attach the battery pack to the micro:bit and tape it on the wrist cuff band on the opposite side from the micro:bit.

##### Step 3 - Add the wrist fasteners the micro:bit

Attach Velcro tabs at the ends of the wrist cuff as fasteners. You may need to try it on your wrist to adjust the size.

![](https://i.imgur.com/Ggn8v4M.png)

##### Step 4 - Decorate it!

Decorate the wrist cuff with stickers, glitter, markers, etc.

![](https://i.imgur.com/NmTjyry.png)

#### Code

##### Step 1

We want the micro:bit to choose rock, paper, or scissors when you shake it. Place a `on shake` block so when you shake the micro:bit, it will run part of a program.

![](https://i.imgur.com/r5M1BnM.png)

##### Step 2

Add a `tool` variable to store a random number computed with `pick random`.

When you shake the micro:bit, it should pick a random number from `0` to `2` and store it in the variable `tool`. (This variable is named `tool` because rock, paper, and scissors are the tools you use to challenge your friends!)

![](https://i.imgur.com/G1wQf6H.png)

In a later step, each of the possible numbers (0, 1, or 2) is matched to its own picture. The picture is shown on the LEDs when its number is picked.

##### Step 3

Place an `if` block under the `pick random` and check whether `tool` is equal to `0`.

![](https://i.imgur.com/zbXw2Ni.png)

##### Step 4

In the `if` block, place a `show leds` block that shows a picture of a piece of paper.

![](https://i.imgur.com/0EC4a7K.png)

##### Step 5

Add an `else if` block to the `if` block and check whether `tool` is equal to `1`.
Click on the gearwheel icon to open up the `if` editor; then drag and drop an `else if` block in the `if` editor.

![](https://i.imgur.com/YVoe1rF.png)

##### Step 6

Place a `show leds` block under the else if and draw a rock image on the screen.

![](https://i.imgur.com/UZXLDn4.png)

##### Step 7

Add a `show leds` block with a picture of scissors to the `else` part.
You don’t need to check if `tool` is `2` because `2` is the only number left out of `0`, `1`, and `2`. That’s why you can use an `else` instead of an `else if`.

![](https://i.imgur.com/sj8uE4R.png)

Link of the whole program: [https://makecode.microbit.org/_3kHLRkXR85s2](https://makecode.microbit.org/_3kHLRkXR85s2)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_fFfPbhbwWimT" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>



