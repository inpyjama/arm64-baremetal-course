# arm64-baremetal-course
A repo to setup a working environment for experimentation

```
The code provided as part of this repository is ONLY for learning purposes!
```

# TODO: Add course link

# Instructions

1. Create a code space (reuse if already created):
    1. `code` -> `codespaces` -> `+` button!
    2. Wait for codespaces to initialize fully (might take 2-3 minutes)
    3. You should see a working vscode code environment
    4. Don't worry about the dependencies. Toolchains, headers, build-essentials, QEMU environment setup everything is setup for you `:)`
2. Compile the bare-metal kernel for `Raspberry Pi-3b` for a particular assignment/lab-exercise:
    1. Create a new folder e.g. `mkdir section-1-<name>`
    2. Create necessary files and copy over the source code from the files attached in the course's assignment/lecture sections
    3. Once all the files are copied, your directory structure should contain - 
       1. Source - `.c` / `.S` files
       2. Headers - `.h` files
       3. Makefile - `Makefile`
       4. Linker Script `linker.ld`
    4. Run `make` to compile the kernel (You should see `kernel8.img` file being generated)
3. Run the generated image on QEMU
    1. `qemu-system-aarch64 -M raspi3b -kernel kernel8.img -serial null -serial stdio`
    2. `Ctrl + c` to quit QEMU

# Copyright

Copyright © 2024 inpyjama.com. All Rights Reserved.