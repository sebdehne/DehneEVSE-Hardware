# EvChargingStationHardware

KiCad design files of a controller board for Type-2 charging (IEC 61851) of EVs. It is based on [Arduino Nano 33 IoT](https://store.arduino.cc/arduino-nano-33-iot).

Hardware features:
- Control Pilot (CP) circuit (borrowed from [OpenEVSE](https://github.com/OpenEVSE/OpenEVSE_PLUS)).
- Proximity Pilot (PP) support for Socket outlets.
- Reads charging power by measuring both voltage and current on all three phases.

Not implemented features:
- No ground fault detection included. Use an external Type-B GFCI
- No driver for motorised interlock (to lock the charging cable in the type-2 socket)

