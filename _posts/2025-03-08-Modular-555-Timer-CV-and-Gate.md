---
layout: post
title: Eurorack 555 Synth
date: 2025-03-8
categories: electronics
tags: diy electronics
---
Transistors in the simplest terms amplify or switch electrical signals. In these examples, a BJT 2N2222 transistor will be used to switch on and off power to an LED.

Micro-controllers (like an Arduino, Pi, CV/Gate) use transistors to control things they normally cannot due to high amp or voltage demand and keep you micro-controller safe.

How it works:
* A low power source, such as an Arduino pin or low voltage, is applied to the "Base"
* Electricity flows from "Collector" to "Emitter"

Always check or google the datasheet for the transistor you decide to use. The Base, Collector, and Emitter can be different depending on the trasistor and is not always consistent. Sometimes the Base is not the middle leg!

![Alt text 2](https://32bitwave.github.io/32bitcoffee/images/BJTexample.png) 

Bill of materials:
* 1 X Breadboard
* 1 X 1K Resistors
* 1 X LED
* 1 X 2N2222 Transistor
* 1 X 9V battery (any power supply 5V to 12V)
* 1 X Set of wires for breadboard
* 1 X Button

This is how it will look on the breadboard. When you hit the button, the transistor "allows" the circut to complete and electricity to flow.
![Alt text 2](https://32bitwave.github.io/32bitcoffee/images/tinkercadTransistor2n2222.png) 

Arduino Example:

Bill of materials:
* 1 X Breadboard
* 1 X 1K Resistor (for base)
* 1 X 470 ohm resistor (for LED)
* 1 X LED
* 1 X 2N2222 Transistor
* 1 X 9V battery (any power supply 5V to 12V)
* 1 X Set of wires for breadboard
* 1 X Button
* 1 X Arduino

![Alt text 2](https://32bitwave.github.io/32bitcoffee/images/arduinoTransistor.png)

Code:

      void setup()
      {
            pinMode(9, OUTPUT);
      }
      
      void loop()
      {
            // turn the LED on (HIGH is the voltage level)
            digitalWrite(9, HIGH);
            delay(1000); // Wait for 1000 millisecond(s)
            // turn the LED off by making the voltage LOW
            digitalWrite(9, LOW);
            delay(1000); // Wait for 1000 millisecond(s)
      }
