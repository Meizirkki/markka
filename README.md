Markka - The virtual currency of finns!
================================

Copyright (c) 2009-2013 Bitcoin Developers
Copyright (c) 2011-2013 Litecoin Developers

What is Markka?
----------------

Markka is a slightly modified version of Litecoin
 - 5 minute block targets
 - subsidy halves in 210k blocks (~2 years)
 - ~500 million total coins
 - 200 coins per block
 - 2016 blocks to retarget difficulty

Markka was founded on the idea of creating a national (yet very unofficial)
virtual currency for the people of Finland. To attract the entire population
of Finland and reach stability within the next few years, roughly 84% of the
estimated total number of coins are to be shared evenly according to social
security ID's. 
 
License
-------

Markka is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

The `master` branch is not guaranteed to be
completely stable.

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

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./markka-qt_test

