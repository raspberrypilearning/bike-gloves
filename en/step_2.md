## Prototype

### Power + 555 “skeleton”

--- task ---

Put the 555 chip in the middle of the breadboard, across the centre gap.

With the notch on the left, the pins are:

```
8  7  6  5
|--|--|--|

|--|--|--|
1  2  3  4
```

![555 chip added to breadboard with Pin 1 in E8 and Pin 8 in F8](images/LED_555-9.png){:width="450px"}

--- /task ---

--- task ---

Connect the 555 power pins:

Pin 1 → ground rail

![A jumper cable connecting A8 to the ground rail](images/LED_555-8.png){:width="450px"}

Pin 8 → positive rail

![A jumper cable connecting G8 to G5 and another jumper cable connecting F5 to the positive rail](images/LED_555-7.png){:width="450px"}

Pin 4 (RESET) → positive rail (so it is always enabled)

![A jumper cable connecting A11 to the positive rail](images/LED_555-6.png){:width="450px"}


At this stage, the 555 chip has power pins wired but nothing else.

--- /task ---

### Build the timing network

--- task ---

Join pins 2 and 6 together (TRIG and THRESH).

![A jumper cable connecting D9 to D13. Another jumper cable connecting E13 to F13. Another jumper cable connects H13 to H10](images/LED_555-5.png){:width="450px"}

--- /task ---

--- task ---

Add two 47 kΩ. resistors:

- The first connects the positive rail to pin 7.

![A kΩ resistor connecting H5 and H9](images/LED_555-4.png){:width="450px"}

- The second connects pin 7 to pins 2 and 6 (the joined pins).

![A kΩ resistor connecting G9 and G13](images/LED_555-3.png){:width="450px"}

--- /task ---

--- task ---

Add the capacitor (10 µF) so that:

- The positive (long) leg connects to joined pins 2 and 6

- The negative (short) leg connects to the GND rail

![A 10uF capacitor with the long leg in J13 and short leg in J15](images/LED_555-2.png){:width="450px"}

The 555 will oscillate, but you will no notice this until it is connected to an LED.

--- /task ---

### Add the LED and resistor

--- task ---

Connect Pin 3 (output) to the 470Ω resistor, which connects to the LED's long leg.

Connect the LED's short leg to the ground rail.

![An LED with the long leg in H14 and short leg in H15](images/LED_555-1.png){:width="450px"}

--- /task ---

--- task ---

Add the 9V battery and connect the power and ground rails:

- Battery positive to the red positive rail

- Battery negative to the blue ground rail

![A 9V battery connected to the power rails](images/LED_555.png){:width="450px"}

--- /task ---

--- no-print ---

<video width="480" height="270" controls>
<source src="images/LED_555.mp4" type="video/mp4">
</video>

--- /no-print ---

The LED should blink once every second.

**Debug**: Unplug the battery and recheck:

- Pin 1 = GND, pin 8 = +9V, pin 4 tied to +9V
- Pins 2 & 6 properly joined
- Timing capacitor legs the correct way round
- LED legs the correct way round.