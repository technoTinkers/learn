## Magic Button Trick

Build a magic trick that uses the micro:bit’s compass to detect a nearby magnet!
This is a simple magic trick you can perform to amaze your friends! When you move the sticky labels on your micro:bit’s A and B button, you appear to make the buttons really switch over. To see the trick performed watch the video below.

[https://youtu.be/-9KvmPopov8](https://youtu.be/-9KvmPopov8)

### How the trick works  

The **magic** here is really in the code. This trick uses a magnet, hidden in your hand, to tell the micro:bit to swap over the buttons. When the magnet is near the micro:bit, the **A** button starts working like the **B** button and the **B** button starts working like the **A** button. Tricky!

### What you need

The only things you need for this trick are your micro:bit and any magnet that is small enough to fit in your hand, even a fridge magnet will work.

![](https://i.imgur.com/Z4rx7XY.png)

### Step 1: Getting the buttons to display A and B

Before we code the trick itself, we need to get the buttons working as you would expect them to such that pressing button A displays ‘A’ and pressing button B displays ‘B’:

![](https://i.imgur.com/EzjTIKQ.png)

### Step 2: Measuring magnetic force

We will use the micro:bit’s compass to detect the magnet. A compass tells us which direction we are pointing to by detecting the Earth’s magnetic field, but it can also detect any other magnet nearby. We will use that to check if our magnet is next to the micro:bit by using the `magnetic force` block found in the **Input** menu’s … **More** section. Since we only want to measure the strength we change the drop down to select `strength`:

![](https://i.imgur.com/YzekMGN.png)

### Step 3: Checking if the magnetic is nearby

Now we can measure the magnetic force near the micro:bit. We can check if the value we measure is so big that it means there must be a strong magnet nearby.

If you’ve ever played with magnets you know they have two ends, often called a North and South ‘pole’. Depending on which end of the magnet is pointing at the micro:bit, the magnetic force measurement will either be a negative number (like, -100) or a positive number (like, 100). We just want to know if the strength is at least 100. We don’t care if its negative or positive so we also use the `absolute of` block from the **Math** menu to tell our code to ignore the negative sign and just treat -100 as if its 100.

So, in the code below, we will check if the absolute value of our magnetic field strength reading is more than 100 and save the result of that check in a new variable called `isSwitched`:

![](https://i.imgur.com/208su2R.png)

### Step 4: Running our ‘magnet nearby’ check all the time

At the moment, our code to detect a magnet being nearby will only run once. We need to put it into a `forever` loop so that it keeps running again and again, checking for the magnet to come near to the micro:bit. We should also make sure `isSwitched` is set to `false` when our program starts.

![](https://i.imgur.com/IPBcbFA.png)

### Step 5: Swapping the buttons when we know the magnet is nearby

Now we can check the value of our variable `isSwitched` whenever we want and we will know that the magnet is nearby if it’s value is `true`. Let’s use that to change how the buttons work and complete the code for our trick. We will add an `if then else` block to each button’s code and check if we should swap over what’s displayed for each button if `isSwitched` is equal to `true`:

![](https://i.imgur.com/RwV1Ldk.png)

Link of the whole program: [https://makecode.microbit.org/_Lc4b87PtL9ih](https://makecode.microbit.org/_Lc4b87PtL9ih)

<div style="position:relative;height:0;padding-bottom:70%;overflow:hidden;"><iframe style="position:absolute;top:0;left:0;width:100%;height:100%;" src="https://makecode.microbit.org/#pub:_Lc4b87PtL9ih" frameborder="0" sandbox="allow-popups allow-forms allow-scripts allow-same-origin"></iframe></div>

### Step 6: Practice your technique

Now you just need to program your own micro:bit and practice the trick a few times before performing for your friends. Try asking your friends to click the buttons after you have switched the labels and the trick won’t work for them because they don’t have a hidden magnet in their hand!

Remember, that as we are using micro:bit’s compass, it will need to be [calibrated](https://support.microbit.org/support/solutions/articles/19000008874-calibrating-the-micro-bit-compass-what-does-it-mean-when-the-micro-bit-says-draw-a-circle-or-tilt) each time we flash the program or run it for the first time.

### About the authors

This project was contributed by Brian and Jasmine Norman, aka @MicroMonstersUK. You can checkout their [MicroMonsters](https://www.youtube.com/channel/UCK2DviDexh_Er2QYZerZyZQ) tutorials channel on YouTube for more projects.
