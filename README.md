Dogecoin PoS Core integration/staging tree
=====================================

# Dogecoin Core [DOGE, Ð]

![Dogecoin](https://static.tumblr.com/ppdj5y9/Ae9mxmxtp/300coin.png)

Dogecoin is a cryptocurrency like Bitcoin, although it does not use SHA256 as
its proof of work (POW). Taking development cues from Tenebrix and Litecoin,
Dogecoin currently employs a simplified variant of scrypt.
- **Website:** [dogecoin.com.](https://dogecoin.com)

[Dogecoin Proof of Stake](https://blog.geekwisdom.org/)

What is Dogecoin PoS?
----------------

[Dogecoin PoS](https://dogecoin.com/) is a fork of Bitcoin POS as a proof of concept
staking mechanism for Dogecoin. Dogecoin PoS uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Dogecoin PoS Core is the name of open source
software which enables the use of this currency.

Dogecoin PoS Core is built on top of Dogecoin Core. The difference between the two
is the consensus algorithm: Dogecoin PoS Core uses Proof of Stake consensus, whilst
Dogecoin Core uses Proof of Work. Using Proof of Stake as a consensus algorithm is
allowing it not only to scale better and be orders of magnitude more efficient in
terms of power consumption, but it is also lowering the entry barrier for contributing
to the creation of new blocks.


## License – Much license ⚖️
Dogecoin PoS is released under the terms of the MIT license. See
[COPYING](COPYING) for more information or see
[opensource.org](https://opensource.org/licenses/MIT)

## Development and contributions – omg developers
Development is ongoing, and the development team, as well as other volunteers,
can freely work in their own trees and submit pull requests when features or
bug fixes are ready.

#### Version strategy
Version numbers are following ```major.minor.patch``` semantics.

#### Contributions ✍️

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

**testnet and regtest modes**

Run with the `-testnet` option to run with "play dogecoins" on the test network, if you
are testing multi-machine code that needs to operate across the internet.

If you are testing something that can run on one machine, run with the `-regtest` option.
In regression test mode, blocks can be created on-demand; see qa/rpc-tests/ for tests
that run in `-regtest` mode.

