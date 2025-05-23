---
layout: post
title: Eurorack 555 Synth
date: 2025-03-8
categories: electronics
tags: diy electronics
---
This is a synth made with a 555 timer that uses CV and Gate. CV goes from 1 to 5 volts and gate is sensitive to anything above 0.5 volts. 

This Eurorack 555 timer does not track with the 1V OCT standard but it does sound decent. The CV is controlled trough a vactrol and the Gate is controlled trough a transistor. 

Note: The pulldown resistor may not be needed on the base of the transistor for gate depending on your hardware/sequencer.

Realistically there should be diodes implemeted near audio jack inputs to protect your hardware so please use at your own risk. For me, with the arturia beatstep, I did not use the pulldown resistor and felt confortable not using diodes due to my hardwares circut protection.

![Alt text 2](https://32bitwave.github.io/32bitcoffee/images/Euro555Pic.JPG) 

![Alt text 2](https://32bitwave.github.io/32bitcoffee/images/555withCVandGate.png) 

![Alt text 2](https://32bitwave.github.io/32bitcoffee/images/555withCVandGate2.png) 

Bill of materials:
* 1 to 3 X Breadboard
* 2 X 10uf Capacitors (Be aware of polarity!)
* 5 X 1K Resistors
* 1 X LED
* 1 X 555 Timer IC
* 1 X 10K Potentiometer
* 1 X 2N2222 Transistor
* 1 X Photoresistor (Play around with the values!)
* 3 X Audio Jacks
* 3 X Audio Cables
* 1 X 9V battery (any power supply 9V to 12V)
* 1 X Set of wires for breadboard
