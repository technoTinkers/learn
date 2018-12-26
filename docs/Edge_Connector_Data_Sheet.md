
# Edge Connector Data Sheet
---
- A detailed data sheet all about the pins and signals of the edge connecto.

![](https://i.imgur.com/ppEvX0Y.jpg)
## Overview
---
- The edge connector on the micro:bit board brings out all the key signals and circuits that you would need in order to build attachments to the micro:bit. 5 of the pads are large rings with 4mm through plated holes suitable for attaching standard banana plugs, or for clipping crocodile clips to. 3 of these are connected to GPIO pins that are also capable of analog, PWM and touch sensing. The 3V and GND rings are useful for providing a small amount of power to external circuits, or (carefully) back powering the micro:bit from an external power supply.

- The smaller strips spaced at 1.27mm on the edge connector have additional signals, some of which are used by the micro:bit, and others that are free for you to use. There are a number of external PCB connectors for purchase with an 80w 1.27mm pitch that can be used to easily access these extra pins. For these narrow pins, they are only connected on the front of the device, the narrow pins on the back are unconnected.

## Pins and Signals
---
- This table shows various data about each of the pins on the micro:bit edge connector.

![](https://i.imgur.com/auRKA92.png)




## Notes
---
![](https://i.imgur.com/6tdNMJG.jpg)

1. RINGs for 0, 1, 2, 3V and GND are also connected to the respective reverse side rings on the edge connector.
2. The 3V and GND rings have guard strips either side of the big rings, to avoid any degradation of device performance due to slipping crocodile clip connections. Care should be taken on rings 0, 1 and 2 to avoid shorting crocodile clips against adjacent pins, which could cause some slight interference with the pattern currently displayed on the LED matrix, or introduce some innaccuracies in the light sensing readings.
3. The DAL DynamicPWM driver (and the underlying nrF51 timer peripherals) dictate that PWM can only be active on 3 pins simultaneously. Any attempt to allocate a 4th pin for PWM use, will disable one of the existing PWM pins.
4. Digital input pins are by default configured with internal pull down resistors when the pins are configured by the DAL.
5. Functions in brackets should be used with caution, as other features of the device may become unstable, degraded or non operational, if their normal use is not disabled in the software first.
6. The source file for the pinout table is held in CSV format. You can load this into a spreadsheet and sort and filter it in any way that makes sense to you. There is also a zipped Python script in this folder that you can download to re-generate the markdown table version of the pinmap used on this page, from the .csv file.
7. The pin marked ‘ACCESSIBILITY’ is used to enable/disable an on-board accessibility mode, and should not be used for anything else (even though it can be used as a GPIO for testing). Future versions of the official micro:bit editors may remove the ability to write to this pin.

## Uncoupling Default Functionality
---
- Pins that are marked with brackets around functions, require the default functionality for that pin to be disabled, before other functions can be used.

---

- pins: P3, P4, P6, P7, P9, P10

These pins are coupled to the LED matrix display, and also it’s associated ambient light sensing mode. To disable the display driver feature (which will automatically disable the light sensing feature) call the DAL function display.enable(false).Note also that the LED 3x9 matrix connects LEDs with associated resistors across these pins, so you should take that into account when designing circuits to use these pins for other purposes.

---

- pins: P5, P11

These pins are assigned to the two on-board buttons. In their default setup with all the standard high level languages, there is a global uBit instance containing: `uBit.buttonA`, `uBit.buttonB` and `uBit.buttonAB`.
Buttons are hooked into the system timer in their constructor for regular debouncing. However, if you want to completely remove this feature and use the physical pins for other purposes, you can delete `uBit.buttonA`, it will call the C++ destructor and de-register the button instance from the system timer, effectively disabling all DAL activity with that pin. It is then possible to use a `MicroBitPin` instance around the physical pin name to control it directly without interference from the DAL.

*Be aware though, that there are 10K external pullup resistors fitted to the micro:bit board.*

---

- pins: P19, P20

These pins are allocated to the I2C bus, which is used by both the onboard motion sensor. It is strongly suggested that you avoid using these pins for any function other than I2C.

It is possible to disable the DAL services that use these pins as the I2C bus, but the motion sensor device will still be connected to the bus, and may try to interpret the signals as data payloads, which could create some undesirable side effects on the SDA and interrupt pins. There are 4K7 pullups fitted to both pins on the board, so the best use for these two signals is to add other I2C devices.

The main reason you might choose to use these pins for other purposes would be if you were designing your own micro:bit variant without any I2C devices, and then it would free up two more pins for other purposes.


## Power Supply Capabilities
---

The power supply capabilities and parameters, which better define how you can use the GND and 3V rings.
 
1. The maximum number of pins configured as high-drive (5mA) at any one time is 3 pins.

2. A common way that the maximum pin voltages can be exceeded, is to attach an inductive load such as a speaker, motor, or piezo sounder directly to the pin. These devices often have significant back-EMF when energised, and will generate voltages that exceed the maximum specifications of the GPIO pins, and may cause premature device failure.

3. The pin marked `‘ACCESSIBILITY’` is used to enable/disable an on-board accessibility mode, and should not be used for anything else (even though it can be used as a GPIO for testing). Future versions of the official micro:bit editors may remove the ability to write to this pin.

4. The BBC suggest in the safety guide, that the maximum current you can draw from the whole edge connector at any one time is 90mA. This is set based on the 30mA budget for on board peripherals, and the fact that the on board regulator of the KL26 when powered from USB is rated at a maximum of 120mA.

