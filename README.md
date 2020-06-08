# MiniNetPad  First post 8 June 2020

This project is licensed under CERN Open Hardware Licence v.1.2 http://ohwr.org/cernohl

Project designed with KiCad Ver 5.1.2
Zip file with design files: MiniNetPad_V0.01a.zip

Schematic file: MiniNetPad_V0.01a.SCH.pdf
BOM file: MiniNetPad_V0.01a.BOM.pdf

Bare board can be odered from OSH Park. https://oshpark.com/shared_projects/rFaZbuVc with project name MiniNetPad_V0.kicad_pcb
  or use source project to make files and order from whoever you wnat.

MiniNetPad features.
 1. Uses Arduino ZERO boot firmware.
 2. CPU is an ATSAMD21G18A.
 3. Has a RT6222 buck based power supply, so wider range of power can be used.
 4. Has a 10/100 network interface W5500 and supporting builtin 802.3af PoE LTC4267.
 5. Support for external RA8875(Adafruit) with 7 inch TFT and touch screen.
 6. Has MicroSD slot.
 7. Has RTC Clock DS3231 chip with battery backup.
 8. 2 Meg of flash memory GD25Q16C.
 9. 1 NEO pixel.
10. MCP23008 I/O.
11. ADS1115 AtoD.
12. MCP4725 DtoA.
13. Buzzer.
14. One 16 pin and one 20 pin external jacks.

Finished Board Top View
![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad.jpg?raw=true "finishedboard")

This project is an alpha level work in progress at this point in time. I expect changes to come.
