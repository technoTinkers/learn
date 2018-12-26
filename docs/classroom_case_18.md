## States of Matter

Make a states of matter experiment that responds to your micro:bit wand or micro:bit’s movement!

[https://youtu.be/Hdsy93yaQC0](https://youtu.be/Hdsy93yaQC0)

### Duration

The activity is approx 30-45 min based on familiarity with the coding concepts

### Materials

- Cardboard
- Aluminum Foil
- Permanent Markers (Red and Black)
- 1 micro:bit, battery holder and 2 AAA batteries
- 4 Crocodile clips
- Activities

Turn a piece of cardboard into a detector of temperature and atmospheric temperature! 

[https://youtu.be/Hdsy93yaQC0](https://youtu.be/Hdsy93yaQC0)

- Fold the foil squares and place them around the cardboard.
- Connect each piece of foil to the appropriate pin on the micro:bit.

That’s it!

### Code

Have you ever tried to represent the states of matter? Let’s try to visually represent various states of matter based on atmospheric temperatures!

#### Step 1: Variables.

In order for States of Matter to follow the rules for determining the atmospheric temperature, we need to add variables that will store data. Then we will assign (set) the value of the variables. We want to name the two (2) variables as follows: “atmos_temperature” and “temperature”. Set the value of the variables to 100. Modify your code so that it looks like this.

![](https://i.imgur.com/ARXb2Ra.png)

#### Step 2: Detect a solid.

We want to detect when the solid state occurs. On Pin 2 Pressed, you want to represent an atmospheric temperature of 0 and scroll the message “SOLID”. We want to set atmos_temperature to 0 and show the string: “SOLID”. Modify your code to look like this:

![](https://i.imgur.com/A29CA6M.png)

#### Step 3: Detect a liquid.

We want to detect when the liquid state happens. On Pin 1 Pressed, you want to represent an atmospheric temperature of 80 and scroll the message “LIQUID”. We want to set atmos_temperature to 80 and show the string: “LIQUID”. Modify your code to look like this:

![](https://i.imgur.com/uYM3S1d.png)

#### Step 4: Detect a gas.

We want to detect when matter will be a gas. On Pin 0 Pressed, you want to represent an atmospheric temperature of 80 and scroll the message “GAS”. We want to set atmos_temperature to 250 and show the string: “GAS”. Modify your code to look like this:

![](https://i.imgur.com/9pGmKYq.png)

- click Download to see if the code works as expected.

#### Step 5: Increase temperature.

We want to display a change of temperature on shake. When you shake the states of matter experiment, there will be a show icon to represent an increase in temperature. Modify your code to add the shake event:

![](https://i.imgur.com/FqU5oOK.png)

- click Download to see if the code works as expected.

#### Step 6: Display temperature change.

We want to conditionally run code depending on whether a Boolean condition is true or false. We want to display certain icons to reflect the temperature being changed on shake. We will create two condition statements. After displaying an icon, the icon will be cleared from the screen with clear screen. Then we will pause program execution for 100 milliseconds. This function is helpful to slow down the program’s execution.

The first condition statement follows this logic: - change the temperature by 20 if the temperature is less than the atmospheric temperature. - change the temperature by -20 if the temperature is not less than the atmos_temperature.

The second condition follows this logic: - show icon with a symbol of a solid if the temperature is less than 32 degrees. - show icon with a symbol of a liquid (umbrella) if the temperature is less than 212 degrees. - show icon with a symbol of a gas if the temperature is greater than or equal to 212 degrees.

![](https://i.imgur.com/rY5AuPD.png)

Link: [https://makecode.microbit.org/_HEq9m0LsjE2g](https://makecode.microbit.org/_HEq9m0LsjE2g)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_HEq9m0LsjE2g" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>






