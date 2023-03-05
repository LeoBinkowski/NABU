# NABU title z80 example

This folder contains a bare-bones NABU title for Z80.

The authors are:

- Leo Binkowski
- Tim Ranger
- Bill Bourne
- Trevor Pearce

of the NABU Network of Ottawa Canada, 1982-1984

## How to build

Requires:
- Microsoft Macro-80 Assembler for CP/M (M80.COM) and
- Microsoft Link-80 Linker (L80.COM).

on a CP/M 2.2 or CP/M 3.0 drive where the files in this folder have been copied.

To build the example:

`SUBMIT BUILD.SUB`

This results in an OPEN.COM, OPEN.SYM, and 000110.PAK, which can be loaded using Nabu Network Adapter software into the NABU PC.

000110.PAK is the NABU Main Menu title PAC-MAN, for testing.

## Components

### CP/M Tools

CABUILD.COM - changes a CP/M .COM file into a NABU .PAK segment file.
CABSERVE.COM - allows one NABU PC to emulate a NABU adapter to load NABU segments.

### Source
### OPEN.MAC
The mainline of the example. Initializes the stack, IOS, the video and joystick.

### ARITH.MRO
Macros for Macro-80 Assembler to provide math simple math functionality.

### CLKAT.MRO
Macro for Macro-80 Assembler to provide simple multitasking tied to the TMS9918A's clock

### COMMON.MRO
Common Macros for the NABU Computer, including color definitions and port mappings.

### LINKTAB.EXA
A file to apply as INCLUDE in a Z80 Macro assembler source that will satisfy all IOS routines in the link table.

### LINKTAB.MHO
The NABU IOS Linktable, which maps all of the IOS functions available.

### NABULOGO.MAC
Contains the source to the routines for showing the NABU Logo and messages usually on the home screen of any title.

### PCENG.MAC
Contains the standard english bold game font.

### STRUCT.MRO
A Collection of structured macros specifically for Microsoft Macro-80 that gives IF-ELSE WHILE FOR and CASE statements to assembler programs.
