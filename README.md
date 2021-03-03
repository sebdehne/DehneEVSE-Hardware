# EvChargingStationHardware

KiCad design files of a controller board for Type-2 charging (IEC 61851) of EVs. It is based on [Arduino Nano 33 IoT](https://store.arduino.cc/arduino-nano-33-iot). See [EvChargingStationFirmware](https://github.com/sebdehne/EvChargingStationFirmware) for firmware.

Hardware features:
- Control Pilot (CP) circuit (borrowed from [OpenEVSE](https://github.com/OpenEVSE/OpenEVSE_PLUS)).
- Proximity Pilot (PP) support for Socket outlets.
- Reads charging power by measuring both voltage and current on all three phases.

Not implemented features:
- No ground fault detection included. Use an external Type-B GFCI
- No driver for motorised interlock (to lock the charging cable in the type-2 socket)

## Changelog

### Revision 1.3 (wip)

- Voltage divider on non-inverting input @ U3 is now 3.3V based  
- Change the Proximity Pilot: R2 is now 1k and is moved down to D1 (which is removed)
- Proper termination of 2nd channel for U3 LF353P op-amp

### Revision 1.2

- Connected available pins on Mains-connector J1 to GND for PE connection
- Fixed several unconnected traces
- Made drill holes for 3.5mm mini-jack (J3, J4 & J5) connectors round
