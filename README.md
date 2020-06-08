# MiniNetPad  First post 8 June 2020

This project is licensed under CERN Open Hardware Licence v.1.2 http://ohwr.org/cernohl

Project designed with KiCad Ver 5.1.2

Zip file with design files: MiniNetPad_V0.01a.zip

Schematic file: MiniNetPad_V0.01a.SCH.pdf

BOM file: MiniNetPad_V0.01a.BOM.pdf

Bare board can be odered from OSH Park. https://oshpark.com/shared_projects/rFaZbuVc with project name MiniNetPad_V0.kicad_pcb or use source project to make files and order from whoever you want.

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

Please, take time and study the schematic before building MiniNetPad.

Bare Board

![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad_Pics/01_board_of_top.jpg?raw=true "boardtop")

Building the board.

  I use LOW TEMP solder paste to give a bit more space for the top end temperature. I use a modified toaster oven for reflow.
  
  I do reflow twice.
  
  First round. Apply paste for the higher pin density chips and problem items then place the chips and items, then reflow.
      After reflow fix any solder bridges.
      
  Second round. Apply paste for resistors, capacitors, leds, etc, then add parts and reflow again.
    
  It takes me about 4 hours to hand build a board. Take it slow and be carefull.

Items not done with reflow, hand soldered after reflows.

  SWD Jack, PowerJack, 3V Select Switch, 16 and 20 pin jacks, RJ45 Jack, Buzzer, Buzzer Pot, Reset Switch, TFT Jack.

Config solder jumpers on bottom of board.

![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad_Pics/07_board_bottom_pads.jpg?raw=true "boardBottomjumpers")

The flash chip can be configured 2 ways - Arduino or CircuitPython

![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad_Pics/11_Flash_Config_Options.jpg?raw=true "flashConfig")

The MiniNetPad uses Arduino ZERO firmware when using Arduino IDE so you flash the board like you would flash an Adruino ZERO.

For MiniNetPad when programing with Arduino IDE, use Arduino Zero (Native USB Port) for board type.

3D printed PLA case was designed with Alibre 2018 CAD,

  Original source file MiniNetPadCaseV01a.AD_PRT and stl file MiniNetPadCaseV01a.stl posted.

Software test program uses TestMiniNetPadV01a.ino

![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad_Pics/15_arduino_testcode.jpg?raw=true "testcode")

If you wish to run CircuitPython.

  Check circuitpython_notes directory for info on installing circuitpython.
  
  I have only test circuit python blink program using the mu-editor, a lot more testing is needed.

There is 2 additional IO boards that plug into the expansion pins.

Source files about the boards is in the ExpansionBoards diretory.

  A small prototype board.

![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad_Pics/17_expansion_protoboard.jpg?raw=true "expansion_protoboard")

MiniProtoBoardV01a bare board can be odered from OSH Park. https://oshpark.com/shared_projects/MGMJdXwL with project name MiniProtoBoardV01a.kicad_pcb
  or use source project to make files and order from whoever you wnat.


  A Tboard that plugs into a breadboard.
  
![alt text](https://github.com/Sd4Projects/MiniNetPad/blob/master/MiniNetPad_Pics/18_expansion_tboard.jpg?raw=true "expansion_tboard")

tExpJackV01a bare board can be odered from OSH Park. https://oshpark.com/shared_projects/LmE7I2u6 with project name tExpJackV01a.kicad_pcb
  or use source project to make files and order from whoever you wnat.

Until more info is added here, check the MiniNetPad_Pics directory.
