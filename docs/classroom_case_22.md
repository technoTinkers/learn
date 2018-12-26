## Voting Machine

Build a voting machine using many micro:bits!

[https://youtu.be/77HOqf8BaNg](https://youtu.be/77HOqf8BaNg)

In this project, a **voter** program is loaded onto a player’s micro:bit. The player uses the buttons to vote either `yes` or `no` and the vote is sent to a **dashboard** micro:bit using the radio. The dashboard allocates one LED per player and turns it on or off based on the vote.

#### The voter program
Assuming button `A` is for a NO vote and `B` is for YES, the voter program works like this:

#### Transmit a NO vote
When button `A` is pressed, a number `0` is sent via radio and the `X` symbol is shown on the screen.

![](https://i.imgur.com/H0OX3mq.png)

#### Transmit a YES vote
When button `B` is pressed, a number `255` is sent via radio and the `Y` symbol is shown on the screen.

![](https://i.imgur.com/yjXOO8f.png)

#### Set device serial number
In order to track the votes, we tell the radio to also transmit the device serial number.

![](https://i.imgur.com/DgY3RIe.png)

#### Set the radio group
We arbitrarily choose `4` as the group used for the communications.

![](https://i.imgur.com/xDBcAcn.png)

Putting all the parts together, here’s the complete voter program:

![](https://i.imgur.com/9d25lVK.png)

Link: [https://makecode.microbit.org/_XcWH4s7wyhmV](https://makecode.microbit.org/_XcWH4s7wyhmV)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_XcWH4s7wyhmV" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### The dashboard

The dashboard code is in the radio dashboard example.
Download the code from that example into the micro:bit that will be used to display the result.
When the dashboard receives a message from a micro:bit, it find a pixel for that board (and remembers it) and uses the number received as the brightness of the LED.
When a message hasn’t been received by a board for some time, it’s pixel will start to blink. After more time, it will simply turn off.

This article comes from [Voting Machine](https://makecode.microbit.org/projects/voting-machine).

