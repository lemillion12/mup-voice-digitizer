# Voice Digitizer
## Microprocessor And Interfacing Project 2016-2017
## BITS Pilani KK Birla Goa Campus

### Objective
The purpose of this simulation project is to digitize a voice signal and reproduced it with certain modifications by a microprocessor. The signal, which is 6 seconds long, has to be stored and later reproduced with a user defined delay.

### Working
The pre­processed output from the microphone (providing a signal between 0-5 V) is sampled and digitized using an 8­-bit ADC (Analog to Digital Converter) at a rate of 1000 samples per second. The digitized signal is then stored in RAM. The voice stored is reproduced with a delay when the user closes a switch labelled sound
replay. The delay ranging from 0 to 9, is also entered by the user with the help of a key­pad. The keypad includes backspace, enter and the digits 0­ to 9. A seven segment is also provided with the keypad to display the delay value entered by the user. The delay is to be added between samples. So, if the value entered is 5, then delay between two adjacent samples when reproduced is 5ms.

### Files
* code.asm - Assembly language program
* code.DSN - Proteus simulation file

### Components used in simulation
* Microprocessor - 8086
* Clock Generator­ ​- 8284
* EPROM​ ­- 2732 [4KB CHIP]
* RAM -­ 6116 [2KB CHIP]
* Analog To Digital 8 Bit Converter -­ ADC0808
* Digital To Analog 8 Bit Converter -­ DAC0808
* Programmable Peripheral Device ​-­ 8255
* Programmable Interval Timer­ - 8253
* Bi­directional Buffers­​ - 74LS245
* Latches­​ - 74LS373
* 3:8 Decoder ­​- 74HCT138
* Bcd To Seven Segment Decoder­ ​- 7447
* Seven Segment Display (Common Anode)­ - 
* Or Gate­​ - 7408
* Switches­ ​- SWSPDT, SWSPST
* 4X3 Matrix Keypad
* Omnidirectional PCB Mount 9.7mm Condenser Microphone
* ​8 Ohm 0.5 W Speaker
* Blue Led
* Low Power Op Amp­ ​- LM 358
* Audio Power Amplifier - LM386
* 15 MHz crystal

### Addressing

**Memory Addressing:**
* ROM1: 00000h - 00FFFh
* RAM1: 01000h - 01FFFh
* RAM2: 02000h - 02FFFh
* ROM2: FF000h - FFFFFh

**I/O Addressing:**
* 8255(1): 80h - 86h
* 8253: A0h - A6h
* 8255(2): 90h - 96h