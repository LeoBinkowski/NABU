
To build Miner-2049er:

1. Use JFDOALL2.SUB in the JF directory along with the files in that directory to
   build the JLIB.REL library.

2. Copy JLIB.REL from step 1 to the LB directory and use LBDOALL2.SUB along with
   the files in that directory to build MINER.COM.

Note that there are additional files in the JF directory that are used to build
the 'test' version of MAP (MAP.COM, without the MINER module). Any fixes required
to get them to assemble were also applied, however when changing the required
conditional in the five source files that can be assembled for the test version
or the full version, there are still missing symbols when linking. All of the
missing symbols are found in the MINER source files. I would think that setting
the conditionals as required would obviate the need for anything in the MINER
module, but that isn't the case. Perhaps MAP and MINER are a bit out of sync.

It's an easy enough fix, but I didn't bother. The test module isn't a playable
game, and I doubt anyone will want to use it.


Scott LaBombard
6/23/2023
