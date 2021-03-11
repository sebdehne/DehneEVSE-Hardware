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

### Bill of Materials (BOM)

| Reference             | Part                           |
| --------------------- | ------------------------------:|
| C1, C2                | 1uf                            | 
| C3                    | 2.2uf/50V                      |
| D1, D2, D4, D5, D6    | 1N4148                         |
| D3                    | TVS-P6KE16CA                   |
| J1                    | Wago 256-408                   |
| J3, J4, J5            | FC68131 3.5mm jack             | 
| K1                    | G5NB-1A Relay 5VDC             |
| L1                    | 18uH                           |
| PS1                   | NMA0512SC                      |
| Q1                    | PN2222A                        |
| R1, R2, R6            | 1k                             |
| R3                    | 330                            |
| R4, R5                | 120k                           |
| R7                    | 180k                           |
| R10, R12, R14         | 100k                           |
| R9, R11, R13, R15-R20 | 10k                            |
| T1, T2, T3            | VB_05-1-12                     |
| U1                    | Arduino Nano 33 IoT            |
| U2                    | NMA0512SC DC/DC 5V -> -12,+12V |
| U3                    | LT1498IN8                      |
| U4, U5, U6            | MCP6291-e_p-nd                 |
















