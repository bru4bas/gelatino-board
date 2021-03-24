# gelatino-board
Arduino meets iCE40 FPGA

This project is meant to be a low-cost FPGA development board, targeting education (Verilog and FPGA) and hobbist users and employing exclusively open-source software and hardware.

It is based on the iCE40LP384 FPGA from Lattice Semiconductor, embedded together with a ATMega328 Arduino-like hardware. Both MCU and FPGA can work together in the Arduino compatible board, and shall be programmed using the traditional Arduino IDE, with extensions. FPGA programming is carried out by the ATMega MCU itself, with an extension of the Arduino standard bootloader -- transfering data to the Flash serial memory, that is shared by both devices.

The main ideas of the project are:
  * Low-lost -- use the cheapest possible components
  * Relative simplicity of production, even hand-made -- avoid smaller IC packages (like BGA)
  * Open-source software only: Arduino environment (avr-gcc, avrdude, ...) and icestorm framework (yosys, icestorm, nextpnr, ...)

Up to now, the project roadmap is
  [x] Preliminary electronic design
  [x] Preliminary bill-of-materials (components from lcsc.com)
  [x] Initial PCB design
  [ ] Conclusion of electronic design and final BOM
  [ ] Building and testing a prototype
  [ ] Changing the Arduino Bootloader for providing FPGA Flash memory programming
  [ ] Coding a extension for the Arduino IDE to deal with Verilog files
  
  Everyone interested in joining this project is welcome!
  
  Many thanks to FPGA WARS, for most of electronic design was inspired from -- mainly the board Alhambra II -- and the amazing projects Yosys and IceStorm.
  
