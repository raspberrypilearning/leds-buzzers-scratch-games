## Challenge: Light show!

Add more LEDs to your breadboard, connect them to your Pi and code a spectacular light show!

--- no-print ---

![LED light show](images/lightShow_completedTask.gif)

--- /no-print ---

--- print-only ---

![LED light show](images/lightShow_completedTask.png)

--- /print-only ---

Add new LEDs in the same way that you added the first one.

--- task ---

Connect another LED using the **3.3v** GPIO pin.

![LED to 3.3v GPIO pin](images/lightShow_LEDto3.3v.png)

--- /task ---

--- task ---

If the LED turns on then you know it is working and connected the correct way round, so move the jumper cable from the **3.3v** pin to a numbered GPIO pin.

![LED to GPIO pin 23](images/lightShow_LEDtoGPIO23.png)

--- /task ---

--- task ---

Do the same to add a third LED, and even a fourth if you like.

![Three LEDs](images/lightShow_3LEDs.png)

--- /task ---

With the three LEDs wired up and ready to go it's time for you to write some code to get all the lights working in any way that you like.

The example shows the LEDs connected to GPIO pins 17, 23 and 25 but you could use any pins that you like, just make sure your coding uses the same pins that you have used.

![Light show challenge code solution](images/lightShow_lightShowCode_Solution.png)

--- hints ---

--- hint ---

`when flag clicked`{:class="block3events"}, carry on `forever`{:class="block3control"} turning `LED 17`{:class="block3extension"}, `LED 23`{:class="block3extension"} and `LED 25`{:class="block3extension"} `on and off`{:class="block3extension"}.

This challenge is very open, the order you light them, whether they all go together or on some random sequence, how you set the timing are all up to you.

--- /hint ---

--- hint ---

You will probably use the blocks below to create the LED light show code.

![Light show challenge code parsons problem](images/lightShow_lightShowCode__parsons.png)

You might also want to use the `random number`{:class="block3operators"} block.

![Light show challenge code parsons problem](images/lightShow_randomNumber.png)

--- /hint ---

--- hint ---

The code below are some possible examples but what you come up with is up to you. You might want to think about the result you want and try to make that heppen with code, or you could approach it from the other side, playing with the code and seeing what the results look like. 

Always try and understand why the result look the way it does. 

![Light show challenge code solution](images/lightShow_lightShowCode_Solution.png)

--- /hint ---

--- /hints ---
