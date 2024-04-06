# Bouncing-and-Debouncing-Switch

Our task is to control a relay switch with a push-button and understand bouncing and debouncing circuits in electronics.
We are using a relay because it will give a clear picture of on and off devices.

Step -1:Gather the material from the IoT kit:
● 1 x ESP32
● 1 x USB Cable
● 1 x Breadboard
● 4 x Jumper wires
● 1 x Push Button
● 1 x Relay
● 1 x Mosquito Repellant Machine/Lamp/Bulb with holder

Step -2: Let’s do connections:
● Insert pushbutton on the breadboard
● Connect one end of the pushbutton with ESP32 GPIO pin no 22
● Connect another end of the pushbutton with GND of the ESP32

Take the Relay(Black Box), Insert the relay Plug into AC mains.
● Connect relay with ESP32 BOARD
● Connect Black with GND, Red with 3.3V, and Yellow with ESP32 GPIO PIN 18
● Take one device like Mosquito Repellant Machine/Lamp/Bulb with holder and insert them into relay switch.

Step -3: Let’s write the program

Step -4: Output:
Compile and upload the program to ESP32 board using Arduino IDE
● Verify the program by clicking the Tick option
● Upload the program by clicking the arrow option

Press the push button once and keep it for several seconds and then release it and you'll see the light flickering of your connected device.
You will see that you pressed the button once but your lamp/mosquito repellent LED will flicker on and off multiple times.
It is called BOUNCING since it shows multiple stages of 0 and 1. 
Ideally, it should turn on and off once when a button is pressed. Consequently, it will give false signals.
False signals cause a lot of problems with electronics circuits.
To rectify this we focus on Debouncing circuits

To remove this type of issue we have a pre-defined library called ezButton.This library is usually used with pushbuttons and various Switches.
Connections will remain the same as previous circuits.

Go to Tools and select Serial Monitor
Press the push button once and keep it several seconds and then release it and you'll see there is no light flickering.
You will see that you pressed the button once in a result your lamp/mosquito repellent LED will turn on and off once only instead of multiple times
It is called DEBOUNCING since it shows one stage of 0
and 1. 
This is the Ideal solution for the circuit.
