## Coding sequences

Now you know how to wire up LEDs and buzzers, it is about time we mashed them up together. First let's look at something new about breadboards...

### Breadboard side positive and negative strips

You have been using the horizontal rows of five holes that join your components together but there is also a pair of vertical side strips that are often marked as positive (+) and negative (-) and are usually used to create a positive and negative strip all the way down the side of your breadboard. 

![Breadboard.png](images/sequences_breadboardSideStrip.png)

Since we are using switched GPIO pins, we have little use for a positive strip but a negative strip connected to the Raspberry Pi ground makes a lot of sense.

### Wriring up

--- task ---

Wire up a couple of LEDs to GPIO 17 and 23, and a buzzer to GPIO 25. Link the negative side strip to the Raspberry Pi ground (GND) pin and take all negative feeds from there.

![Two LEDs and a buzzer.png](images/sequences_2LEDsAnd1Buzzer.png)

--- /task ---

### Sequence 1

--- task ---

If you saved the Scratch code from the **light show challenge**, that will work with this new set up as long as you used GPIO pins 17, 23 and 25. You will have code that says, `turn LED 25 on`{:class="block3extensions"} or `off`{:class="block3extensions"} but all that does is `set GPIO pin 25 to output high`{:class="block3extensions"} (on) or `low`{:class="block3extensions"} (off), so it will work just the same for an LED or a buzzer.

Open your code and see how it looks... and sounds!

--- /task ---

Just so our code is clear, we'll use the Simple Electronics `LED`{:class="block3extensions"} blocks for our LEDs and the GPIO `set gpio`{:class="block3extensions"} blocks for other components.

--- task ---

If you saved the Scratch code from the **light show challenge**, that will work with this new set up as long as you used GPIO pins 17, 23 and 25. You will have code that says, `turn LED 25 on`{:class="block3extensions"} or `off`{:class="block3extensions"} but all that does is `set GPIO pin 25 to output high`{:class="block3extensions"} (on) or `low`{:class="block3extensions"} (off), so it will work just the same for an LED or a buzzer.

Open your code and see how it looks.

![Two LEDs and a buzzer.png](images/sequences_2LEDsAnd1Buzzer.png)

--- /task ---

