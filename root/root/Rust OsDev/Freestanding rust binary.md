# Freestanding rust binary
all Rust crates link the standard library, we dont want that bcz its OS specific and we are the ones making the os

`#![no_std]`

Because we dont have the std lib we need to define out own panic function

we also need to disable stack unwinding 

make \_start main and then build: