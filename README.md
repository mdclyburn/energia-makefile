Energia MSP430 Makefile
-----------------------

This project was forked from Elpaso's Energia Makefile project (https://github.com/elpaso) as it appears to have been abandoned for
a number of years. His original notes can be found at the bottom of this
readme.

INSTRUCTIONS
------------
To build an elf file:
(Assuming you are running linux)
```
1. Download Energia:
  http://energia.nu/download/

2. Extract energia file to a directory of your choice.

3. cd to the energia-makefile directory  

4. Place the .ino file that you want to compile in the energia-makefile dir

4. export ENERGIADIR=/YOUR PATH/energia

   export ENERGIABOARD=lpmsp430g2553 (or whatever your taraget)

   make

5. Get elf file.
```

To compile and upload your .elf file:

```
1. run sudo /YOUR PATH/YOUR ENERGIA VERSION/hardware/tools/msp430/bin/mspdebug

2. in the debugger, type 'erase'

3. in the debugger, type 'prog yourFile.elf'

4. in the debugger, type 'run'
```

================================================================================
Elpaso's Original Notes:
-----------------------

Energia MSP430 Makefile
-----------------------

I'm the kind of programmer that hates complicated IDEs, moreover I can't suffer Java(TM), for this reason I tend to use Makefiles to compile MCU code, this is what I've been doing with Arduino during the last years.

Yesterday I received this new Launchpad board and the very first thing I've done was to write a Makefile to compile and upload programs to the board.

This Makefile is freely adapted from the good job done by Tim Marston at http://ed.am/dev/make/arduino-mk

Makefile for c code
-------------------

Makefile.c is a makefile to compile c programs, it doesn't use energia stuff.
