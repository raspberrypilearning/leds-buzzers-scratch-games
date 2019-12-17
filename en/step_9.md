## Scratch games with LEDs and buzzers

The last thing you're going to do in this project is make a two-player Scratch game.

The game will be a simple race game but the players can only move at certain times indicated by two LEDs and a buzzer. If a player tries to move when the red LED is lit, they will jump backwards!

--- no-print ---

![Scratch game](images/scratchGame_final.gif)

--- /no-print ---

--- print-only ---

![Scratch game](images/scratchGame_final.png)

--- /print-only ---

Let's start with the LED and buzzer hardware circuits.

--- task ---

You'll need to start off with a red LED wired to GPIO 17, a yellow LED wired to GPIO 23 and a buzzer wired to GPIO 25. Of course, it makes no difference if you choose different colours or different GPIO pin numbers but the example code will always refer to these pin numbers.

![2 LEDs and 1 buzzer](images/scratchGame_2LEDsAnd1Buzzer.png)

This is the exact same setup you had earlier in **Coding sequences**.

--- /task ---

Next step is to get a **backdrop** and two **sprites**.

--- task ---

Click on the **choose a backdrop** button and choose a background that works for two characters to race across. 

![Choose a backdrop](images/scratchGame_chooseBackdropButton.png)

This example uses **Basketball 1**.

![Basketball 1 backdrop](images/scratchGame_basketballBackdrop.png)

--- /task ---

--- task ---

Next, click on the **choose a sprite** button and choose two sprites to race across your stage. Having two characters that are similar widths will make things easier but using sprites you like is important too.

![Choose a sprite](images/scratchGame_chooseSpriteButton.png)

This example uses **Ben** and **Jordyn**. They are very similar which makes things easier.

![Ben and Jordyn sprites](images/scratchGame_benAndJordynSprites.png)

--- /task ---

### The game structure

To make your player move, you simply have to press that sprite's **move** key, **a** for Ben and **l** for Jordyn. The letters at opposite ends of the keyboard.

The red LED indicates that you are not allowed to move. If a player has their **move** button pressed when the red light is lit, their sprite will jump backwards.

The yellow LED indicates that you **are** allowed to move. Pressing a player's **move** light when the yellow LED is lit will make their sprite move slowly forwards.

The buzzer will sound as a warning just before the yellow turns off and the red LED turns on. As soon as a player hears the buzzer they should stop pressing their **move** button.

You will write the code for when the LEDs and buzzer turn on and off in the stage's workspace.

--- task ---

For this project, you will need both the `Raspberry Pi GPIO` and `Raspberry Pi Simple Electronics` extensions, so add those right away if they are not already loaded.

--- /task ---

--- task ---

Select the stage.

Start wth the `when flag clicked`{:class="block3events"} and then add blocks to make sure that the yellow LED and buzzer start by being off, and the red LED starts on.

+ red LED = LED 17
+ yellow LED = LED 23
+ buzzer = GPIO 25

```blocks3
when flag clicked
set gpio (25 v) to output [low v] ::extension
turn LED (23 v) [off v] ::extension
turn LED (17 v) [on v] ::extension
```


--- /task ---