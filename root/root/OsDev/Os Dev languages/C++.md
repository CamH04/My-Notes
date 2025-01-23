# C++
C++ expects a stack pointer before the program is executed, that is a big problem as the boot loader wont set it. That means we have to set it yourself. In AlbaOS this is done in as follows:

loader.s :

sets stack pointer and then jumps to kernel.cpp

For this ^ to work we will need to use a linker (.ld file) because they are different languages (ASM and C++). These files are combined to create the kernel.bin file

The kernel.bin is put into the boot directory of the partition as well as putting a menu entry for it into the GRUB .CFG so the boot loader can be pointed to the kernel.