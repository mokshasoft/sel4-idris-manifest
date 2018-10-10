# sel4-idris-manifest - Project to build Idris applications on seL4
Example of Idris applications running on the seL4 microkernel

## Prerequisites
To build this application the seL4 build system and the Idris compiler needs to be setup.
- https://sel4.systems/
- https://www.idris-lang.org/

## Get the Code!

Run the following to get the code:

        mkdir sel4-idris
        cd sel4-idris
        repo init -u https://github.com/mokshasoft/sel4-idris-manifest.git
        repo sync

## Build and run it in QEMU

Run the following to build and run it:

        ../init-build.sh -DPLATFORM=x86_64
        ninja
        ./simulate

After the boot the following should be displayed in the terminal:

        "seL4 <3 Idris"

Quit QEMU with 'Ctrl-a c'
