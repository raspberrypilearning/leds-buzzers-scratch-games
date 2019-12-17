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

--- task ---

Click on the **Frank** sprite (the process is the same for all sprites so would work for any you choose).

Now pull the code into two parts.
+ the `event`{:class="block3events"} and starting state (initialisation)
+ the cycle of changes (the `forever`{:class="block3control"} loop and everything inside it)

![Frank sprite](images/frankSpriteIdentifier.png)

```blocks3
when flag clicked
go to x: (0) y: (0)
set size to (100) %
set [whirl] effect to (0)

forever
    turn LED (23 v) [on v] ::extension
    change size by (30)
    change [whirl v] effect by (200)
    wait (pick random (0.3) to (1.2)) secs
    turn LED (23 v) [off v] ::extension
    set size to (100) %
    set [whirl] effect to (0)
    wait (pick random (0.3) to (1.2)) secs
end
```

--- /task ---