## Hot or Cold

Find the hidden micro:bit before the other players!

[https://youtu.be/nbRfNug-RkY](https://youtu.be/nbRfNug-RkY)

### Beacons
In this game, players are looking for a hidden micro:bit that emits a radio signal. Hidden micro:bits are called beacons.

### Setting up the radio
We set the radio group to 1 and all the players use the same group. The micro:bit transmits its serial number (that’s a unique number that identifies it) so that players can tell one beacon apart from another. Also, the power of the antenna is reduced to shorten the range of transmission.

![](https://i.imgur.com/NNnoQGu.png)

### Beacon gotta beam
The beacon just needs to send a radio message every now and then. So, to pace the transmits and give some visual feedback, we add some `||basic:show icon||` blocks to animate the screen.

![](https://i.imgur.com/N5paArS.png)

### Hide the beacons
Download the code to each beacon micro:bit and hide them!

### Hunters
The hunter micro:bit looks for beacons.

### Is the beacon close?
To determine how far away or how close they are, we use the signal strength of each radio packet sent by the beacons. The signal strength ranges from `-128db (weak)` to `-42db (very strong)`.

![](https://i.imgur.com/GGL0SEa.png)

Test and record the signal values as you move around a beacon, moving closer and farther away:

Hot signal value:	_________________
Warm signal value:	_________________
Cold signal value:	_________________

### Hot or cold?
The hunter’s screen will display:

`SmallDiamond`: if the beacon is far (cold).
`Diamond`: if the beacon is relatively close (warm).
`Square`: if the beacon is really close (hot).
Use the `signal` values collected in the previous step to determine when to show each icon.

Here is an example that uses `-95` or less for cold, between `-95` and `-80` for warm, and `-80` or above for hot. You can change these values to account for your room setup or conditions of your hidding place.

To make the program more responsive, add a `||led:stop animation||` to cancel icon animations when a new beacon packet comes in.

![](https://i.imgur.com/6hFBlh3.png)

Download the code and play the game!

### Expand the game: multiple beacons

We’ll making the game more interesting by counting how many beacons the hunting player has seen so far.

#### Remember the beacons

Do you remember that the beacon was configured to transmit its serial number? We can use this information to determine if a beacon is new or if it’s one we’ve seen before.

To do so, we add an `array` variable that will hold all the beacon serial numbers seen so far.

![](https://i.imgur.com/pvlgDJn.png)

Whenever we receive a new packet, we are going to check if the `beacons` array already contains the serial number. If not, we add the serial number at the end of `beacons` and increment the `||game:score||`.

To check if an array contains an certain element, we use the `||arrays:find index of||` block which returns `-1` if the element is not found.

![](https://i.imgur.com/0YyREG5.png)

#### Show my score
To see the current score, we add an `||input:on button pressed||` that displays the score on the screen when the A button is pressed.

![](https://i.imgur.com/f5yIoeF.png)

### All together
The hunter code with all th pieces together looks like this now. Download and try it out with multiple beacons!

![](https://i.imgur.com/uPMY14o.png)

Link：[https://makecode.microbit.org/_cq5AR1hk36Vc](https://makecode.microbit.org/_cq5AR1hk36Vc)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_cq5AR1hk36Vc" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>


This article comes from [Hot or Cold](https://makecode.microbit.org/projects/hot-or-cold).


