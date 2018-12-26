## Timing Gates

This project explains the principles of timing gates using household materials.

### Timing Gates

Two gates are connected to the micro:bit so it can detect a car passing through them.

![](https://i.imgur.com/jJGrpgE.png)

As the car passes through the gate `0`, it sends an event to the micro:bit through the `on pin pressed` block. The micro:bit records the time in a variable `t0`.

![](https://i.imgur.com/HhNoFNt.png)

As the car passes through the gate `1`, it sends an event to the micro:bit through the `on pin pressed` block. The micro:bit records the time in a variable `t1`.

![](https://i.imgur.com/BhWGIFe.png)

The rest is a bit of math and physics. The time taken to cross the gates is computed as the difference of t1 - t0. By dividing the distance between the gates by the duration, we get the speed of the car!

![](https://i.imgur.com/Zzytibg.png)

### Materials

- Carboard
- Aluminum foil
- Double-side tape (carpet tape)
- 4 crocodile clips
- A micro:bit board and USB cable

![](https://i.imgur.com/DFME2yL.png)

### blocks

![](https://i.imgur.com/JNIr6Da.png)

### Building the gate

The sensor is made by tapping two strips of foil on the cardboard as close as possible.
Add two strips of double-sided tape on the cardboard. Remove the protective film.

![](https://i.imgur.com/sG70tSs.png)

Lay the Aluminum foil on the double-sided tape. Press firmly on the tape to get a good bonding of the foil.

![](https://i.imgur.com/N76i10K.png)

Pull off the foil that’s not touching the tape strips. That’s all the foil in between and around the tape strips. This clears out the extra foil and makes a gap between the foil on the tape strips. Make sure the gap is just enough so that both foil strips don’t touch each other.

![](https://i.imgur.com/H2wQS3u.png)

Connect a crocodile strip to each foil strip.

![](https://i.imgur.com/WvqfZeX.png)

Connect the crocodile plugs to the `GND` and `P0` pins on the micro:bit.

![](https://i.imgur.com/64xTmMW.png)

The gate is ready to use! Your circuit should look like the picture below:

![](https://i.imgur.com/tD1kurd.png)

### Detecting the car with code

The micro:bit provides an event `on pin pressed` that is raised when a circuit between `GND` and a pin is detected. The circuit conductor could be a wire or even your body! We will attach a foil to the bottom of the car. When it passes over the gate, it connects both foil strips, closes the circuit and triggers the event.

Open the [code editor](https://makecode.microbit.org/) and start a new project and add the following blocks. Notice that we are using pin `P0` here.

![](https://i.imgur.com/PTm8GwZ.png)

Testing the code with our finger, we see a LED column turn on when pressing on both strips.

[https://youtu.be/zi_-NAmdDpY](https://youtu.be/zi_-NAmdDpY)

### Upgrading the car

In this lesson, we picked a random toy car and tapped foil to the bottom. As the car goes through the gate, it will connect both sides of the gate and trigger it. Make sure to add enough foil to get a good connection on the ground.

![](https://i.imgur.com/2LySkGH.png)

By moving the car (slowly) through the gate, you will see that it triggers the `on pin pressed` event.

[https://youtu.be/M3DIUvDPlIA](https://youtu.be/M3DIUvDPlIA)

It doesn’t always work! Why? Sometimes the foil doesn’t touch both strips for long enough time to be detected. This is due to the poor quality of our sensor. To fix this, you would need to use better a sensor, maybe an IR detector or a Hall effect sensor.

### Adding the second gate

Repeat the same process with tape and foil to build the first gate.

![](https://i.imgur.com/EczuaoT.png)

Connect the crocodile plugs to the `GND` and `P1` pins on the micro:bit.

![](https://i.imgur.com/NW9TCAP.png)

### Detecting the second gate

Since the second gate is connected to pin `P1`, we add a second `on pin pressed` event that display 2 columns of LEDs.

![](https://i.imgur.com/3btpPbp.png)

Strolling the car over both gates, you can see how the first gate triggers then the second.

[https://youtu.be/N4bWQcu6yWs](https://youtu.be/N4bWQcu6yWs)

### Computing time

The micro:bit has a clock that measures time precisely. It measures how many seconds the micro:bit has been on. We will record the time where each gate is tripped in variables `t0` and `t1`. We take the different between `t1` and `t0` to compute the duration between the gates.

![](https://i.imgur.com/3x5sNzR.png)

Link: [https://makecode.microbit.org/_6ACEeCPtPY09](https://makecode.microbit.org/_6ACEeCPtPY09)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_6ACEeCPtPY09" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

[https://youtu.be/piyym_ux1EM](https://youtu.be/piyym_ux1EM)

### Computing velocity

Measure the distance between the gates and apply Newton’s laws to compute the velocity (how fast it’s going) of the car.

> v = d / t

We’ll let you try to code this one on your own!



















