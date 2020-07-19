# Neotron Compute

Neotron is a family of 1980's style home computers, powered by ARM Cortex-M processors, with a ROM written in Rust, and a fully open-source design.

## Components

### BIOS

The Neotron BIOS is a similar concept to the IBM PC BIOS, or the BIOS used on CP/M systems. It boots the system and provides hardware abstraction.

### OS

The Neotron OS runs on all Neotron machines. It expects to access RAM starting at `0x2000_0000`, and gets all other information about the system from the BIOS.

### Shell

The Neotron Shell is a cross between `COMMAND.COM` on MS-DOS, and the BASIC interpreter you get on something like a Commodore 64 or ZX Spectrum.

### Applications

The Neotron Shell can ask the OS to load an application, which will then run. A well-behaved application should run on any system running the Neotron OS, provided it has enough RAM available. You can also get (perfectly valid) badly-behaved applications which reach out and touch the hardware directly - like MS-DOS, there's no memory protection here!

## Developers

* [thejpster](https://github.com/thejpster)
* [segfault](https://github.com/IGBC)
