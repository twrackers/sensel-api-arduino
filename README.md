# ALPHA RELEASE. Documentation to be added.

# Sensel API Arduino

The Sensel API Arduino allows users to communicate with Sensel devices from Arduino boards. 

This fork of the original repository refactors the arrangement of the files and adds supporting files to match the updated Arduino IDE, version 1.8.19. It has not yet been tested with the newer Arduino 2.2+ IDE. Source files have also had corrections applied so that sketches calling this library will now compile.

## Getting Started

To get started with the Sensel API for Arduino, you will need to have a Sensel device, like a Sensel Morph, and a Hacker Cable which connects the Sensel device to your Arduino board serial communication.  

## Serial Interface

The Sensel Hacker Cable should be connected to a Hardware Serial on the Arduino Board. While it is possible to use a Software Serial, the signal is unreliable at higher speeds so occasional frames will need to be dropped if improper data is sent.

Arduino-type devices which do have hardware serial (usually called **Serial1** in the code) include:

* Arduino MEGA 2560
* Arduino Micro
* Arduino R4 Minima
* Arduino R4 WiFi
* Arduino DUE
* Adafruit Itsy Bitsy 32u4, 5V 16MHz version (tested)
* Adafruit Itsy Bitsy 32u4, 3V 8MHz version
