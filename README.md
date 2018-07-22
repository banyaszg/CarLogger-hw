# CarLogger-hw
OBD-II CAN logger based on Particle Electron(Photon). With Particle Electron it can monitor 2 CAN buses. So it can handle the Medium Speed CAN bus of Mazda and Ford cars.

# Motivation
My main project is designing a remote surveillance system for my car, which connects to the OBD-II CAN buses and sends notification to my phone. I'm mainly interested in security related information (lock, doors, alarm), and battery power. So the standard OBD communication protocol doesn't cover these signals. I have to find them in the proprietary communication. I designed this device to check whether I can reverse engineer the needed part of the Mazda communication protocol.
This device can also be used as the first version of the surveillance system. It has 3 extension connectors for GPS an other sensors.

# Features
* 2 High-speed CAN transceivers
* Power from the OBD-II port using a DC/DC buck converter
* Use with Particle Photon (1 CAN) or Particle Electron (2 CAN)
* MicroSD card
* Battery monitoring
* With Particle Electron and battery it can turn off the DC/DC converter to save the car's battery
* The CAN transceivers can work from the battery of the Particle Electron
* 3 [Grove](http://wiki.seeedstudio.com/Grove_System/) compatible connectors

# Hardware
* [Schematic (PDF)](CarLogger.PDF)
* [Gerber](Gerber)
* [Drill](NC-Drill)
* [Bill of materials](BOM/Bill%20of%20Materials-CarLogger.xls) (Use Grove connectors instead of JST!)
* The PCB fits into this [case](https://www.aliexpress.com/item/16Pin-OBD2-Connector-J1962m-Handle-Connector-DIY/32782473183.html)

A Particle [Photon](https://docs.particle.io/datasheets/photon-(wifi)/photon-datasheet/) or [Electron](https://docs.particle.io/datasheets/electron-(cellular)/electron-datasheet/) is required.

# Software
* The [CarLogger firmware](https://github.com/banyaszg/CarLogger-sw) is used for logging.
