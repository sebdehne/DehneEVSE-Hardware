# DehneEVSE

KiCad design files of a controller board for Type-2 charging (IEC 61851) of EVs. It is based 
on [Arduino Nano 33 IoT](https://store.arduino.cc/arduino-nano-33-iot). 
See [EvChargingStationFirmware](https://github.com/sebdehne/EvChargingStationFirmware) for firmware.

See [Schematic](Media/schematic.pdf) and [3d-view](Media/PCB-3d-view.png).

Hardware features:
- Control Pilot (CP) circuit.
- Proximity Pilot (PP) support for Socket outlets.
- Reads charging power by measuring both voltage and current on all three phases.

Not implemented features:
- No ground fault detection included. Use an external Type-B GFCI
- No driver for motorised interlock (to lock the charging cable in the type-2 socket)

