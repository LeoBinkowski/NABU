
Here are the updated sources. To build:

1. Use JFDOALL2.SUB in the JF directory along with the files in that directory to
   build the JLIB.REL library.*

2. Copy JLIB.REL to the LB directory and use LBDOALL2.SUB along with the files in
   that directory to build MINER.COM.


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


I did look at the code a bit more, and determined that the catwalk table will never
contain data due to the missing bit of code. Consequently, the game will not be
playable. The missing code is only responsible for the catwalk table, all the other
tables (ladders, slides, etc...) have their own unique table functions, and I have
verified that all of them appear to be intact. This explains why BB can't walk onto
the catwalk, and why I was able to climb the ladder on the right of the first screen
(and it further explains why BB stops when at the top of ladder).

Scott LaBombard
6/23/2023
