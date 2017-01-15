# AVR-Makefile
A makefile that I use for my projects, rewritten line by line so that I understand it. Simple yet complete, as long as debugging and simulation are not required.

This makefile supports the following:
* `make` or `make build`: Build and link C (`*.c`) and ASM (`*.S`) files in the current directory
* `make program`: Upload hex and eeprom files to the device using avrdude and selected programmer type
* `make fuses`: Burn fuses using avrdude
* `make clean`: Remove all compiled object and dependency files

An EEPROM file (`*.eep`) will also be generated and uploaded, containing any preloaded EEPROM variable set with the EEMEM attribute.

All object, hex, eeprom, and dependency files are placed in a "builds" subfolder.
