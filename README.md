# ZIN-70 Quad Nixie Display
 
### Important Notes

This is a four tube display built using Millclock ZIN-70 Nixie Tubes. This can be used to drive a clock, or just as a numeric display.

Please note that if you decide to use this display as a clock, it does not include a colon.

Current iteration: Version 2

### Components and Requirements

Supply:
* Any* 12V 500mA (or better) supply. DC 5.5mm Male Plug

Mechanical and Connectors:
* 1x Same Sky `PJ-063AH` DC 5.5mm Female Connector 
* 1x C&K Switches `DP62J12S202HQ` DPDT Slide Switch (Power Switch)
* 2x Same Sky `TS04-66-85-BK-100-SMT` SPST Button (Hour and Minute buttons)
* 2x Keystone Elec. `1291-66 ` 9V Battery connector

Tubes:
* 4x Millclock `ZIN-70` Nixie Tubes (Z5680M Pinout) - 170V ~5mA each
* 1x NE-2 5mm "Daytime" Indicator (I used a yellow phosphor Mercury/Argon tube)
* 1x NE-2 5mm "Nighttime" Indicator (I used a blue phosphor Mercury/Argon Tube)

Passives:
* 4x 6.8kR 1206(in) SMD Current-Limiting Power Resistors (Nixie Tubes)
    - (or 5K if you wish to run at a bit higher current)
* 8x 1kR 1206(in) SMD Current-Limiting Signal Resistors (Outputs)
* 4x 200kR 1206(in) SMD Current-Limiting Power Resistors (Indicator Swapper)
* 2x 100nF 1206(in) SMD Decoupling Capacitors
* 2x 1uF 1206(in) SMD Filter Capacitors
* 2x 10k 1206(in) SMD Filter Resistors

HV Boost Supply:
* 1x Omnixie `NCH8200HV` (12V to 170V 30mA)
    - Custom footprint. Only compatible with NCH8200V.

Driver:
* 1x Murata `OKI-78SR-5/1.5-W36-C` 12-5V DC-DC Converter 
    - Custom footprint for this device. Swap or remove as required
* 1x Murata `OKI-78SR-12/1.0-W36-C` 18-12V DC-DC Converter 
    - Custom footprint for this device. Swap or remove as required
* 1x WaveShare `RP2040-Tiny` devboard 
    - Custom footprint. Please swap for your driver. Only compatible with 23-pin 2.54mm pitch RP2040 tinies.
    - Buy directly from waveshare if you want to avoid incompatibility.

Registers and Other:
* 2x Microchip Tech. `HV5122` PQFP-44 32bit HV Registers (220V 100mA Drains)
    - Custom symbol/package configured. 
* 4x TO-92 NPN Transistor (any with E B C pinout) such as 2N2222
    - Faster transistors better!
* 2x >0.5A Through-hole Diode - 1N400X series intended, equivalent works.

