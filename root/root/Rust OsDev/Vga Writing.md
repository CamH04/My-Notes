# Vga Writing
Read and write to 0xb8000 

BUFFER STRUCTURE

Bits     Byte     What It Does

0-7      1             Code page 437 Representation Number (high ASCII or OEM font)  
8-11     2             Foreground Colour  
12-14   2             Backround Colour  
15        2              Will the character blink

COLOURS

| Number | Color | Number + Bright Bit | Bright Color |
| --- | --- | --- | --- |
| 0x0 | Black | 0x8 | Dark Gray |
| 0x1 | Blue | 0x9 | Light Blue |
| 0x2 | Green | 0xa | Light Green |
| 0x3 | Cyan | 0xb | Light Cyan |
| 0x4 | Red | 0xc | Light Red |
| 0x5 | Magenta | 0xd | Pink |
| 0x6 | Brown | 0xe | Yellow |
| 0x7 | Light Gray | 0xf | White |

full colour is held as 1 byte