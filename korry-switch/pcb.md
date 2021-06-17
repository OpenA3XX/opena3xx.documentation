---
description: How to get the PCB for the Korry Switch.
---

# PCB

## Understanding What It Does

I want to start with a short explanation of what the PCB actually does, and why we have decided to choose this method of design.

![Front of the PCB](../.gitbook/assets/korry_pcb2%20%282%29.png)

The unit itself contains a switch \(locking or non-locking\), 2 LED's and 2 resistors.  
So, why does such a simple circuit need a PCB? Can't we just put the components in the 3D printed unit, solder a resistor to the LED leg and then solder some wires?

![Back of the PCB](../.gitbook/assets/korry_pcb3.png)

Well, yes you can do that. And that was part of the design for those that really can't \(or don't want to\) use the PCB.  
The PCB gives the whole unit some stability and structure. The base of the 3D printed outer shell sits between the PCB and the switch & LED's. This gives a base for the switch when it is pressed and pressure applied. It also holds the components in exact alignment, and most importantly, it removes the need for soldering wires inside the unit, it makes it neat and compact, and completley modular.  
Using the pin headers on the PCB means you can easily swap out units and reconnect them without the need for soldering. This makes things easier, but also prevents accidental damage to units with the soldering iron when working in tight spaces.

The LED's have a common **CATHODE**.  
The switches have 2 functions. One is _'Press to make'_ and the other is _'Press to break'_.  
We are using the _'Press to make'_ function, which means that when the switch is closed, it completes the circuit and turns the switch 'On'. The other function does the opposite, and you should check with a multimeter which pins are which on the swtich. I personally break the legs off the switch that we don't need to avoid confusion at a later date. If you don't want to do this, the PCB has holes for these legs.

![](../.gitbook/assets/img_5354.jpg)

The LED's are placed on either side of the switch, and they are deliberatly square as they are 'directional' and will throw their light in a straight line, helping to avoid light bleed across the unit.  
Each LED then lights up it's respective 'Top' or 'Bottom' display when illuminated.  
There are 5 pins on the board \(see below for the [wiring diagram](pcb.md#wiring-diagram)\), and this enables the switch and each LED to be connected individually.

It's cheap, well designed, reliable and easy to get your own made. You can even get the small resistors already soldered to the board at the factory if you don't want to do those yourself.  
We believe that this is a great way to start with the OpenA3XX project and give yourself some added confidence to take on some of the bigger projects, like the MCDU for example.

![](../.gitbook/assets/1.png)

## How To Order Your Own

## Wiring Diagram

![Korry PCB Wiring Diagram](../.gitbook/assets/capture.jpg)

