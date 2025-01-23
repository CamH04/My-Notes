# Stage 1: Firmware
1.Firmware

Takes firmware data from bios and copies it to RAM

Instruction pointer is put to the start off copied firmware in RAM

Firmware tells CPU to talk to HDD to load MBR

This will be the first ~2MB stored on the HDD disc, this area is called the master boot record (MBR) 

The reason for having a MBR is becuase the Firmware doesnt know about partition tables and file structures