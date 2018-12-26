## Tele-Potato

Don’t keep the potato too long or you might lose the game!

![](https://i.imgur.com/V5EtA0N.png)

Do you know the “Hot Potato” game? You toss around a potato while a timer counts down and the person holding it when the timer is up loses… It’s super fun.

In this project, we’ll build a similar kind of game but instead we’ll use a virtual potato and the micro:bit radio.

### Teleporting potato?

Instead of passing a real potato around while a real clock counts down, we are going to **send a number** between micro:bits. We can do that using the `||radio:Radio||` blocks. They use the antenna on the micro:bit to send data over radio frequency signals, just like the phones or gadgets around you.

![](https://i.imgur.com/gWNcq6O.png)

Now, what does it mean to have a number represent a potato? Well, we need to **model** the clock as **a number** being tossed around with the potato. We do this so that we can play the game using the radio. So what is so special about this potato clock? It ticks down the time and when it reaches 0, it rings.

To keep track of things, let’s have a variable called **potato**:

- If the value of **potato** is positive, the player has the potato and the **potato** variable represents the **remaining time**.
- If value of **potato** reaches 0, the game is over.
- If the value of **potato** is negative, this means that the player doesn’t have the potato in their hand.

Now that we know what the potato is, we need to come up with the user interactions. This is how will the user play the game:

- press the `A+B` button to start the game and send the first potato.
- when a potato is received, the screen displays some image.
- when the player shakes the micro:bit, they send the potato to other players.

### Let’s get coding!
#### Initialization

Let’s start by creating the potato variable and initializing it to `-1` in `||basic:on start||`. Remember, a negative potato value means you **don’t** have the potato. We use `||radio:radio set group||` to make sure players receive the messages.

![](https://i.imgur.com/ldLEFv0.png)

#### Starting the game
To start the game, we respond to the `A+B` button press and assign a positive number to the **potato** variable. To make the game less predictable, we use the `||math:pick random||` block to generate a value between `10` and `20`.

![](https://i.imgur.com/92vvFzc.png)

#### Sending the potato
Sending the potato is done by shaking the micro:bit. If the **potato** variable is positive, we have the potato and we can send it. After sending it, we set the **potato** variable to `-1` since we don’t have it anymore.

![](https://i.imgur.com/Ffzvfwv.png)

#### Receiving the potato
Receiving the potato is done in the `||radio:on radio received||` block. The **receivedNumber** represents the potato and is stored in the **potato** variable.

![](https://i.imgur.com/Cwu6sbj.png)

#### Ticking the clock
Making the clock tick down is done with a ||loops:forever|| loop.

- If the potato is equal to 0 (potato == 0), KABOOM! you lose!
- If the potato variable is negative (potato < 0), we don’t have the potato so we clear the screen.
- If the potato variable is positive (potato > 0), we display a potato image and decrease the variable by 1.

![](https://i.imgur.com/OJqEevU.png)

#### It’s game time!
Get two or more micro:bits and download the code to them. One player starts the game by pressing A+B to receive the first potato. Good luck!

### Full source

![](https://i.imgur.com/09XeZCj.png)

Link：[https://makecode.microbit.org/_Cv8LfPPMP54D](https://makecode.microbit.org/_Cv8LfPPMP54D)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Cv8LfPPMP54D" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>




