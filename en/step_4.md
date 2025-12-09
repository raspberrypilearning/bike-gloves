## Challenge

### Blink faster

Bike lights might be more visible is they blink quickly.

If the resistance is halved, the LED will blink twice as fast!

--- task ---

Add a new 47 kΩ resistor in parallel with one of the existing 47 kΩ resistors.

Bend the new resistor so its legs are spaced the same.

Solder the legs directly to the exposed legs of the existing resistor.

--- /task ---

### Vary the blink time

Turn a dial to change the blink rate.

--- task ---

Add a 50 kΩ trim potentiometer in parallel with one of the existing 47 kΩ resistors.

Connect the middle leg of the potentiometer to one of the resistor's legs.
Connect one of the potentiometer's other legs to the other leg of the resistor.

Bend the other potentiometer leg out of the way, or trim it off.

--- /task ---

### Save battery - only work only in low light

Your bike light will mostly be needed later in the day, when it is darker.

Makes a voltage divider, so Pin 4 can sense light levels.

--- task ---

- Connect one leg of an LDR to Pin 1 (VCC).

- Connect the other leg Pin 4 AND to a 47 kΩ resistor.

- Connect the other leg of the resistor to GND.

--- /task ---
