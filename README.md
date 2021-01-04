# VirtualWireESP

This is a fork of the [VirtualWire](https://www.airspayce.com/mikem/arduino/VirtualWire/) which is officially superseded by the RadioHead Library.
VirtualWire was originally written for ATmega processors and therefore not supported by Espressif chips.
This project is the **fully** functional port for ESP!
See the VirtualWire [Reference](https://www.airspayce.com/mikem/arduino/VirtualWire/VirtualWire_8h.html#details) for more information.
Tested with the supplied example code on an ESP32 NodeMCU:      
<br>
![NodeMCU example](https://www.elektor.de/media/catalog/product/cache/5562f759999b940b867d7ecf207c58b6/1/6/169034-91f-web.jpg "NodeMCU")

## Caution
I had to redefine
```
#define F_CPU 80000000L
```

in VirtualWirESP.h because my clock speeds where falsly set to 240MHz which caused wrong timings for recieving data.
You might need to readjust this for your personal needs.
