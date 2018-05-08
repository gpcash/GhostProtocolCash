GhostProtocolCash integration/staging tree
================================

http://http://www.ghostprotocal.org/
```
Copyright (c) 2009-2013 Bitcoin Developers
Copyright (c) 2011-2012 PPCoin Developers
Copyright (c) 2013 NovaCoin Developers
Copyright (c) 2018-2023 GhostProtocolCash Developers
```
What is GhostProtocolCash?
----------------

GhostProtocolCash is a lite version of Bitcoin using scrypt as algorithm and a PoS-based cryptocurrency using proof-of-stake technology.
 - Algo: Scrypt
 - Type: Hybrid (PoW/Pos)
 - Nama: GhostProtocolCash
 - Short: GPC
 - Address Start: G
 - Supply Coins: 100,000,000 GPC
 - Premine : 20% (20,000,000 GPC)
 - Coin maturity: 80 block
 - Target block: 2 min
 - Diff Adjust: 1 min
 - Confirmations: 10 blocks
 - Stake Reward: 10% (~365 days)
 - Minimum Coin Age to Stake: 12 hours

For more information, as well as an immediately useable, binary version of
the GhostProtocolCash client sofware, see https://github.com/gpcash/GhostProtocolCash/releases

Block Explorer
--------------
http://gpc.pointto.us.

License
-------

GhostProtocolCash is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the GhostProtocolCash
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
[mailing list](http://sourceforge.net/mailarchive/forum.php?forum_name=bitcoin-development).

The patch will be accepted if there is broad conSENsus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of GhostProtocolCash.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test GhostProtocolCash-qt.pro
    make -f Makefile.test
    ./GhostProtocolCash-qt_test
