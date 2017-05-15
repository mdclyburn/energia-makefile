Energia MSP430 Makefile
=======================

The Energia Makefile project has followed a history of being forked from Elpaso's Energia Makefile project (https://github.com/elpaso/energia-makefile) and from Trevortomesh's fork (https://github.com/trevortomesh/energia-makefile). Both the original and the fork appear to be abandoned so I brought the makefile up to working with Energia 1.6.0E18 and published it here.

Instructions
------------
To build an .elf file:

1. Copy makefile to project directory
2. Run:
```sh
export ENERGIADIR=/<path_to>/arduino # only if in a weird place
export ENERGIABOARD=MSP-EXP430FR5969LP # or whatever your target board is
make
```

To compile and upload your .elf file:

1. Run:
```sh
make upload
```
