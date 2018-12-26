## Rock Paper Scissors Teams

Massively multi-player rock paper scissors!

[https://youtu.be/8ztOmdZi5Pw](https://youtu.be/8ztOmdZi5Pw)


Playing rock paper scissors is usually a two player game… but it works with many more players too! When playing with more than two players, it becomes a team game: all players shake at the same time, then the number of rock, paper, scissors is tallied between all the players. The team with the most players wins the game.

Starting with the basic version of the RPS game, we are going to change the code so that the micro:bit counts and displays the number of players on the same team. The micro:bit will use radio communication to send its status and receive the status of the other boards.

Let’s get started!

### Starting blocks
Let’s start out with the code from the original game. The basic version picks one of the tools in a `||input:on shake||` event and displays an icon accordingly. Take a peek at the code below to refresh your memory.

![](https://i.imgur.com/Q7JjY6R.png)

#### Step 1: Refactoring the rendering
**Refactoring** is a funny word used in coding which pretty much means `reorganizing`. In this case, we are going to move the code that displays the rock/paper/scissor icon into its own `||basic:forever||` loop.

![](https://i.imgur.com/w7LMIyt.png)

#### Step 2: Send status via radio
We send the value of `tool` over the radio to the other micro:bit in the `||basic:forever||` loop. Since a radio packet may or may not arrive, it’s a good idea to keep sending them.

We also set the radio group and send the device serial number (a number that uniquely identifies a micro:bit) as we will need that later.

![](https://i.imgur.com/tyDhhhT.png)

#### Step 3: the team roster

All players are constantly broadcasting to the other players which tool they picked. Let’s add the code that receives this status and counts it.

We’ll add an Array variable that contains all the players on the same team as the current player. This array, named `players`, is like your team roster: it contains the list of micro:bit serial numbers that are using the same tool as you.

![](https://i.imgur.com/QxLIdYy.png)

#### Step 4: Receiving a message (part 1)
In an `||radio:on radio received||` event, we receive the status from another micro:bit. Click on the **gearwheel** to add the `serial` parameter as we will need it to identify who sent that packet.

We compute three values from the data received:

- match a boolean value indicating whether or not the tool of the other micro:bit matches our current tool
- player_index the position in the array of the other board’s serial number. It will be -1 if it is not in the array
- found a boolean value indicating whether or not the micro:bit serial number is part of the players array

![](https://i.imgur.com/07pzeRs.png)

#### Step 5: Receiving a message (part 2)
There are two cases that we need to handle when looking at `match` and `found`:

- **if** we have a `match` and the player is `not found` in the list, then we add it to `players`.
- **if** we don’t have a `match` and the player is `found` in the list, then we `remove` it from players

We turn the two rules above into two `||logic:if then||` statements where the serial number is added or removed.

![](https://i.imgur.com/3wfDMaU.png)

#### Step 6: Reseting the team
What if some of the other players leave the game? They would stop broadcasting their status but would still stay in our list of players. To avoid this problem, we reset the `players` array each time we shake:

![](https://i.imgur.com/rJfPhDf.png)

#### Step 7: Showing team score
The team score is the number of players in that team… which is really just the length of the players array. We add a `show number` block in the `forever` loop to display it.

![](https://i.imgur.com/OReG1xk.png)

#### The final code
Now, it’s time to glue together all the pieces of our program. Go carefully through all the steps and assemble the various features. Eventually, it should look like the following program here. Download and play it with your friendssss!

![](https://i.imgur.com/kUTa2dv.png)

Link: [https://makecode.microbit.org/_1RFcTjPuVV9D](https://makecode.microbit.org/_1RFcTjPuVV9D)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_1RFcTjPuVV9D" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

