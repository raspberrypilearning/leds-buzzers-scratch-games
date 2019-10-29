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

![LED to 3.3v GPIO pin](images/lightShow_LEDto3.3v.png)

--- /task ---

--- hints ---

--- hint ---

When the `program starts`{:class="crumblebasic"}, it should `wait`{:class="crumblecontrol"} a couple of seconds and then turn both motors `FORWARD`{:class="crumbleinputoutput"}, then `wait`{:class="crumblecontrol"} until the buggy has travelled about 30cm. Then, the motors should turn right until they have turned 180° (a half turn), then both motors should turn `FORWARD`{:class="crumbleinputoutput"} until the buggy is back in its starting position. Then, both motors should `STOP`{:class="crumbleinputoutput"}.

--- /hint ---

--- hint ---

You will need to use the blocks below to create the 'there and back again' code.

Can you rearrange them and alter the wait times to make the code work?

![There and back challenge code parsons problem](images/thereAndBack_thereAndBackCode__parsons.png)

--- /hint ---

--- hint ---

The code below works for the example buggy. You might need to alter the wait times and speeds for your buggy.

![There and back challenge code solution](images/thereAndBack_thereAndBackCode_Solution.png)

Click the green **Play** button to see if it works.

--- /hint ---

--- /hints ---
