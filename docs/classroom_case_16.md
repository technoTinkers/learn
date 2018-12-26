## Plant Watering

Water your plants automatically!

[https://youtu.be/7eC_VjH1eP0](https://youtu.be/7eC_VjH1eP0)

## Materials
---
- 1 micro:bit with battery pack and batteries
- 2 long nails or silver
- 2 crocodile clips
- 1 micro servo + 3 female-to-croc clips
- 1 ice cream wooden stick
- 2 elastics
- 1 clear tape roll
- 1 straw
- 1 pair of scissors

## Activities
---

### Setting

#### The pump

Follow the instructions in the video to build a mini water-pump using a micro:bit and a servo.

[https://youtu.be/jANCdtkJAKY](https://youtu.be/jANCdtkJAKY)

#### The soil moisture sensor

Use the instructions of the soil moisture project to make a soil moisture sensor and upload the code to your micro:bit.

The final wiring should look like this:

![](https://i.imgur.com/kMxxo8N.png)

### Code

Let’s add code so that when the soil moisture level is low, the servo waters the plant.

From the soil moisture project, we know that the moisture is low when the `reading` is roughly less than `500`. We can use this number to add an if `reading < 500` in the code to decect a dry condition.

![](https://i.imgur.com/mlhYN7K.png)

The servo is connected to pin **P2** so we can use the `||pins:servo write||` block to change the angle of the servo. We want the angle to change to `0`, wait until the water pours off, and then move the angle back to `80`.

![](https://i.imgur.com/745Fnpl.png)

Insert the code above in the `||basic:forever||` loop of the soil moisture code.

![](https://i.imgur.com/IdqqSuW.png)

Link: [https://makecode.microbit.org/_W1AgrH069TyE](https://makecode.microbit.org/_W1AgrH069TyE)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_W1AgrH069TyE" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

Here’s a video showing the micro:bit watering a plant.

[https://youtu.be/7eC_VjH1eP0](https://youtu.be/7eC_VjH1eP0)


