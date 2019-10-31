## Making noise with buzzers

As well as LEDs, you can control other electronic components using Scratch 3 on the Raspberry Pi.

Although the `Simple Electronics`{:class="block3extensions"} blocks that you have used so far refer to `turning LEDs on or off`{:class="block3extensions"}, all they are doing is switching the GPIO pin on or off (high or low). We could use them to control other electronic components too but just to make things clear, let's add another Scratch extension.

--- task ---
Add the `Raspberry Pi GPIO` extension in Scratch 3

![GPIO extension.png](images/rpi-buzzer_gpioExtension.png)
--- /task ---

### Connecting a buzzer

A buzzer can be connected just like an LED, but as they are a little more robust, you won't be needing a resistor to protect them.

Just like the LED, most buzzers need to have the positive power supply going to the longer, positive leg to work.

Set up your buzzer circuit as shown below:

![Buzzer circuit](images/buzzer_circuit.png)

### Coding a buzzer

--- task ---
Now you can sound the buzzer by using the code below:

```blocks3
when flag clicked
forever
set gpio (17 v) to output [high v] ::extension
wait (1) secs
set gpio (17 v) to output [low v] ::extension
wait (1) secs
```

Or even control it with your button

```blocks3
when gpio (2 v) is [high v] ::hat extension
set gpio (17 v) to output [high v] ::extension

when gpio (2 v) is [low v] ::hat extension
set gpio (17 v) to output [low v] ::extension
```
--- /task ---
