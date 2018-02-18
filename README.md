# Params
Block generation time: 2.5 mins
Blocks per hour: 24
Blocks per day: 576
MN collateral: 15000
Rewards at start: POW: 50% POW: 50%
Coins per block: 200 




NewCoin Core staging tree 0.12.2
===============================

`master:` [![Build Status](https://travis-ci.org/newcoinpay/newcoin.svg?branch=master)](https://travis-ci.org/newcoinpay/newcoin) `develop:` [![Build Status](https://travis-ci.org/newcoinpay/newcoin.svg?branch=develop)](https://travis-ci.org/newcoinpay/newcoin/branches)

https://www.newcoin.org


What is NewCoin?
----------------

NewCoin is an experimental new digital currency that enables anonymous, instant
payments to anyone, anywhere in the world. NewCoin uses peer-to-peer technology
to operate with no central authority: managing transactions and issuing money
are carried out collectively by the network. NewCoin Core is the name of the open
source software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the NewCoin Core software, see https://www.newcoin.org/get-newcoin/.


License
-------

NewCoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is meant to be stable. Development is normally done in separate branches.
[Tags](https://github.com/newcoinpay/newcoin/tags) are created to indicate new official,
stable release versions of NewCoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows
and Linux, OS X, and that unit and sanity tests are automatically run.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

Changes to translations as well as new translations can be submitted to
[NewCoin Core's Transifex page](https://www.transifex.com/projects/p/newcoin/).

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.

Translators should also follow the [forum](https://www.newcoin.org/forum/topic/newcoin-worldwide-collaboration.88/).
