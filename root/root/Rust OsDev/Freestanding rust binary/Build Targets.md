# Build Targets
**My specific target:**

`cargo build --target albaos.json`  
 

**Run in qemu**

`qemu-system-x86_64 -drive format=raw,file="target/albaos/debug/bootimage-albaos.bin"`

had to build for a non default env so i had to build for a ARM env as an example

 `cargo build --target thumbv7em-none-eabihf`

could build it for host with ore linker commands 

`cargo rustc -- -C link-arg=-nostartfiles`