# Microbit Learning Menu

The goal of this project was to allow students to demonstrate their computer science knowledge while exploring various aspects of the BBC Microbit. In addition to the device itself, we also used alligator clips, speakers, LEDs, NeoPixels, standard 9-gram servos, continuous rotation servos, cardboard, and tin foil.

[![YouTube video of our BBC MicroBit projects](http://img.youtube.com/vi/ceZ3xELcZFQ/0.jpg)](http://www.youtube.com/watch?v=ceZ3xELcZFQ)

## Simulation Preparation

A few days prior to actually working with the device, students researched the Microbit and it's built-in sensors. They went to microbit.org and started using the block-based editor (and the Javascript editor) and previewing their result with the simulated Microbit. For simple starter activities, students displayed "Hello World" on the matrix, created a countdown time, and created a simple counting app in which A button increase the count and B button decreased the count.

## Microbit 1: Countdown Game (required)
Create a timer variable and set it to 5 (or 9).

Create a score variable (or two) and set it to 0.

Countdown from 5 to 0, displaying the timer on the "screen"

When the timer is zero or less, say who wins... either player A or player B.

Upload your HEX file here when finished.

## Microbit 2: Bouncing Of The Walls (required)
Create a variable and set it to be a sprite at x 2, y 2

The sprite automatically moves forward and bounces off the walls at random angles.

A and B buttons MUST do something, but you get to decide what the A and B buttons do. Ideas:

-	A starts/resumes the animation and B pauses the animation
-	A increases the speed and B decreases the speed.
-	When A and B are pressed at the same time, the sprite moves back to the center.

### Complete 5 or more of the following:
-	[MakeCode Light Sensor Face](https://github.com/20hz20khz/microbit-learning-menu#makecode-light-sensor-face)
-	[MakeCode Robot Arm](https://github.com/20hz20khz/microbit-learning-menu#makecode-robot-arm)
-	[MakeCode Make A Song ](https://github.com/20hz20khz/microbit-learning-menu#makecode-make-a-song)
-	[MakeCode Musical Instrument ](https://github.com/20hz20khz/microbit-learning-menu#makecode-musical-instrument)
-	[MakeCode Blink 3 LEDs ](https://github.com/20hz20khz/microbit-learning-menu#makecode-blink-3-leds)
-	[MakeCode Fade 2 LEDs ](https://github.com/20hz20khz/microbit-learning-menu#makecode-fade-2-leds)
-	[MakeCode Gyroscope Game ](https://github.com/20hz20khz/microbit-learning-menu#makecode-gyroscope-game)
-	[MakeCode Jumping Game ](https://github.com/20hz20khz/microbit-learning-menu#makecode-jumping-game)
-	[MakeCode Running Game ](https://github.com/20hz20khz/microbit-learning-menu#makecode-running-game)
-	[MakeCode DDR Game ](https://github.com/20hz20khz/microbit-learning-menu#makecode-ddr-game)
-	[MakeCode RC Car ](https://github.com/20hz20khz/microbit-learning-menu#makecode-rc-car)
-	[MakeCode Droid ](https://github.com/20hz20khz/microbit-learning-menu#makecode-droid)
-	[MicroPython Speak ](https://github.com/20hz20khz/microbit-learning-menu#micropython-speak)
-	[MicroPython Sing ](https://github.com/20hz20khz/microbit-learning-menu#micropython-sing)
-	[MicroPython NeoPixel ](https://github.com/20hz20khz/microbit-learning-menu#micropython-neopixel)

## MakeCode Light Sensor Face

Using the built-in light sensor (built into the LEDs), show a happy face if it is bright and a sad face if it is dark.

## MakeCode Robot Arm

Control a standard 9-gram servo with the A and B buttons.

## MakeCode Make A Song

Create a musical instrument. Attach a speaker.
Create a variable and set it to false.
Have a forever loop that plays your sounds (8 or more notes) if a variable is set to true.
When the A button is pressed, set the variable to true.
When the B button is pressed, set the variable to false.

## MakeCode Musical Instrument

Create a musical instrument. Attach a speaker.
When the A button is pressed, play a Low A note.
When the B button is pressed, loop through these notes: C, D, E, G, A.
There are multiple ways that the B button could work...
-	The B button could randomly play either C, D, E, G, A
-	The B button could play C on the 1st press, then D on the 2nd press, etc

## MakeCode Blink 3 LEDs

Get 3 external LEDs.
When A is held down blink two LEDs like this 1-2-1-2-1-2-1-2.
When B is held down blink three LEDs like this 1-2-3-1-2-3-1-2-3.

## MakeCode Fade 2 LEDs

Get 2 external LEDs.
You will use a variable and loops to adjust the LED from 0 (off) to 1023 (full).
Gradually fade the LEDs from 0 up to 1023 down to 0 up to 1023 down to 0 up to 1023, etc.
The 2 LEDs should be out of sync with each other so that one is at 0 while the other is at 1023.

## MakeCode Gyroscope Game

Here is a demo video: https://drive.google.com/open?id=1y9LoEznvtpbSR08ZVglxIcYm-guvGtxg
-	Create a player sprite
-	Change the players x and y location based on the pitch and roll of the microbit
-	Divide the pitch by 60 and roll by 60 to decrease the sensitivity
-	Use a brief pause (from the Basic section) to control the pause's speed

Once you have the basic player controls.....
-	Create an enemy sprite
-	Set the enemy sprite's "blink" setting to 100
-	Create a SECOND forever loop
-	If enemy touches player then game over
-	Either move the enemy randomly or have them move towards the player
-	Use a pause (from the Basic section) to control the enemy's speed.

## MakeCode Jumping Game

Create 2 tin foil buttons so that the players can jump on them.

On start...
-	Setup this game with a countdown timer that starts at 9
-	Create a loop that will display the countdown timer until time is up
-	Display the winner... "A" or "B"

Forever...
-	While the player hasn't pressed A pause 1ms.
-	While the player has pressed A pause 1ms.
-	Give the player A a point

Forever...
-	While the player hasn't pressed B pause 1ms.
-	While the player has pressed B pause 1ms.
-	Give the player B a point

## MakeCode Running Game

Make 2 tin foil buttons so that the player can step on them.
Create a points variable and a timer variable. Set the timer to 9. Display the timer as it counts down. When the timer reaches 0, display the points.

Forever...
-	While the player hasn't pressed A pause 1ms
-	While the player has pressed A pause 1ms
-	Give the player a point
-	While the player hasn't pressed B pause 1ms
-	While the player has pressed B pause 1ms.
-	Give the player a point

## MakeCode DDR Game

Create a Dance Dance Revolution game with 3 tin foil buttons.
Randomly display Left, Right, or Up.
Wait until the player presses that button, then randomly display another.
If the player waits too long, then game over.

## MakeCode RC Car

Connect your microbit to 2 continuous rotation servos.
Either...
-	Use bluetooth to control the microbit's servos from iPad, iPhone, etc.
-	Use a 2nd microbit to send radio signals to control the RC car.

## MakeCode Droid

Combine the light sensor face, create a song, and servo arm projects to create a droid that "talks" and moves it's arms when the light level changes.

## MicroPython Speak

Add a speaker. Use the MicroPython editor.
Make your Microbit speak.
[http://microbit-micropython.readthedocs.io/en/latest/tutorials/speech.html#say-something](http://microbit-micropython.readthedocs.io/en/latest/tutorials/speech.html#say-something) (ignore the diagram that shows the wrong way to connect a speaker)
*You can't just turn in one of the examples from that site.
**Turn in the .PY file, NOT the .HEX file.

## MicroPython Sing

Attach a speaker. Use the MicroPython code editor.
Make your MicroBit sing.
[http://microbit-micropython.readthedocs.io/en/latest/tutorials/speech.html#sing-a-song-of-micro-bit](http://microbit-micropython.readthedocs.io/en/latest/tutorials/speech.html#sing-a-song-of-micro-bit)
*You can't turn in an example from that website.
**Turn in the .PY file, NOT the .HEX file.

## MicroPython NeoPixel

Use the MicroPython editor.
Connect a NeoPixel.
Each time you press the A button, the NeoPixel switches to a random color.
[http://microbit-micropython.readthedocs.io/en/latest/neopixel.html](http://microbit-micropython.readthedocs.io/en/latest/neopixel.html)
**Turn in the .PY file, NOT the .HEX file.
