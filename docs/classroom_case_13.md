## Countdown Timer

Let’s make a countdown timer and see the seconds tick by on your micro:bit watch.

Duration: ~10 minutes

### Make the time variable

We need a variable to keep track of how many seconds are left on the watch.

- Go into **Basic** in the toolbox and pull an `on start` on to the workspace.
- Ok, in **Variables** click on `Make a Variable`. Name the variable as `seconds`. Drag out a `set to` block and change the name with the dropdown to `seconds`. Place the variable into the `on start` block.

![](https://i.imgur.com/XfqaMWJ.png)

### Set the time with buttons

There has to be a way to set the time on your watch. We’ll use the buttons to set the amount of time by adding both 10 seconds and single seconds. We’ll use one button for adding `10` seconds and another button for adding just `1 `second.

#### Set seconds by ten

We’ll use button `A` to add `10` seconds to our time count. The time count of `seconds` will increase by `10` each time the button is pressed.

- In **Input**, find an `on button pressed` an put it somewhere on the workspace.
- Get an `if then` block from **Logic** and put it in the `on button pressed`.
- From the same **Logic** category, get a **0 < 0** and relpace the `false` condition with it.
- Change the left `0` in the condtion to the `seconds` variable. Change `0` on the right to `50`. This limits time to just one minute.
- In the `then` section, put a `change by` there. Select the `seconds` variable name from the dropdown and change the `0` on the right to `10`.
- Add a `show number` below the `change by`. Change the value to the `seconds` variable. Then, put a `clear screen` under that.

![](https://i.imgur.com/bf79m2g.png)

Link: [https://makecode.microbit.org/_d9WXoCP9E7ya](https://makecode.microbit.org/_d9WXoCP9E7ya)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_d9WXoCP9E7ya" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

#### Set seconds by one

Now, we’ll use the `B` button to add just `1` second the time count. The time count in `seconds` will only increase by `1` when this button is pressed.

- In **Input**, find an `on button pressed` an put it somewhere on the workspace.
- Get an `if then` block from **Logic** and put it in the `on button pressed`.
- From the same **Logic** category, get a **0 < 0** and relpace the `false` condition with it.
- Change the left `0` in the condtion to the `seconds` variable. Change `0` on the right to `60`. Again, this limits the time to just one minute.
- In the `then` section, put a `change by` there. Select the `seconds` variable name from the dropdown.
- Add a `show number` below the `change by`. Change the value to the `seconds` variable. Then, put a `clear screen` under that.

![](https://i.imgur.com/B9KBpLv.png)

Link: [https://makecode.microbit.org/_eE2V3q11h8t4](https://makecode.microbit.org/_eE2V3q11h8t4)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_eE2V3q11h8t4" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

#### Shake off the time

Ok, now we’ll get the timer going and show how many seconds are left. This will happen when the watch is shaken!

- Get an `on shake` block and place it in the workspace.
- Pull out a `while` from **Loops** and put it in the `on shake`. Replace the `true` condition with the `0 < 0 `conditon from **Logic**. Make the `<` go to `>`. Change the `0` on the left to the `seconds` variable.
- Take out another `show number` and put it inside the `while`. Change the `0` to the `seconds` variable. Put a `pause` under that and set the time to `1000` milliseconds. This means our timer will count down by **1000** milliseconds, which is actually one second, each time through the loop.
- To change the number of seconds left, get a `change by `and place it below the `pause`. Find the `0 - 0` block in **Math** and put it in the `change by`. Set the `0` on the right of the minus to be a `1`.

![](https://i.imgur.com/NsPGdv8.png)

#### Be alarming!

Add a few `show icon` blocks at the bottom of the `while` to make an alarm to show that the time is up! We have some diamonds and the ‘X’ symbol for ours right now.

![](https://i.imgur.com/cbFPxjn.png)

Link: [https://makecode.microbit.org/_72ch5T95a56j](https://makecode.microbit.org/_72ch5T95a56j)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_72ch5T95a56j" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

#### All Done!

Nice! You’ve got your timer coded now. Go press the `Download` button and put your code on the micro:bit. When you shake it, it counts down from the time you have set.

At first, there are zero seconds set. To add ten seconds to the count, press the **A** button. To increase the count by one second, press the **B** button.

