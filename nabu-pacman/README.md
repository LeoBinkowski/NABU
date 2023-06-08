# NABU PAC-MAN Z80 Source code

This is the official Source Code to NABU PAC-MAN 

The authors are:

- Leo Binkowski
- Laura Schening

of the NABU Network of Ottawa Canada, 1982-1984

## How to build

Requires:
- Microsoft Macro-80 Assembler for CP/M (M80.COM)
- Microsoft LIB-80 Library Manager for CP/M (LIB80.COM)
- Phoenix Software Assoc. Linker for CP/M (PLINK-II.COM)

on a CP/M 2.2 or CP/M 3.0 drive where the files in this folder have been copied.

To build the example:

`SUBMIT DOALL.SUB`

This results in an PACMAN.COM, which can be converted using CABUILD.COM to software loadable on a NABU PC

000110.PAK is the NABU Main Menu title PAC-MAN, for testing.

## Components

### CP/M Tools

CABUILD.COM - changes a CP/M .COM file into a NABU .PAK segment file.
CABSERVE.COM - allows one NABU PC to emulate a NABU adapter to load NABU segments.
PLINK-II.COM - Allows code larger than 32K to be linked.


