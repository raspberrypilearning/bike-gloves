## Challenge

### Make the lights blink faster

Bike lights might be more visible if they blink quickly.

If the resistance is halved, the LED will blink twice as fast.

--- task ---

Add a new 47kΩ resistor in parallel with one of the existing 47kΩ resistors.

Bend the new resistor so that its legs are spaced the same.

Solder the legs directly to the exposed legs of the existing resistor.

--- /task ---

### Vary the blink time

Add a dial to change the blink rate.

--- task ---

Add a 50kΩ trimmer potentiometer in parallel with one of the existing 47kΩ resistors.

Connect the middle leg of the potentiometer to one of the resistor's legs. Connect one of the potentiometer's other legs to the other leg of the resistor. Bend the other potentiometer leg out of the way, or trim it off.

--- /task ---

### Save battery: Make the lights only work only in low light

You will mostly need to use your lights when it is darker.

You could make a voltage divider with a light-dependent resistor (LDR) so that **pin 4** can respond to light levels.

--- task ---

Connect one leg of an LDR to **pin 8 (VCC)**.

Connect the other leg of the LDR to **pin 4** and a 47kΩ resistor.

Connect the other leg of the resistor to GND.

--- /task ---
