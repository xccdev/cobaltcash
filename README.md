Cobalt Cash Core integration/staging repository
=================================================

Cobalt Cash (XCC) is a sustainable cryptocurrency modeled after Satoshi Nakamoto’s vision for Bitcoin. It is a decentralized, peer-to-peer transactional currency designed to offer a solution to the problem posed by the exponential increase in energy consumed by Bitcoin and other proof-of-work currencies. Proof-of-work mining is environmentally unsustainable due to the electricity used by high-powered mining hardware. Cobalt Cash utilizes an energy efficient proof-of-stake algorithm, can be mined on any computer, and will never require specialized mining equipment. The Green Protocol offers a simple solution to Bitcoin sustainability issues and provides a faster, more scalable blockchain that is better suited for daily transactional use.

- Fast transactions featuring guaranteed zero confirmation transactions, we call it _SwiftTX_.
- Decentralized blockchain voting providing for consensus based advancement of the current Masternode
  technology used to secure the network and provide the above features, each Masternode is secured
  with a collateral of 50,000 XCC.

More information at [savebitcoin.io](http://www.savebitcoin.io)

### Coin Specs
| Block Time                  | 60 Seconds      |
| Max Coin Supply (PoS Phase) | 210,000,000 XCC |
| Premine                     | 4,200,000 XCC   |

### Reward Distribution

| **Block Height** | **Masternodes**  | **PoS**         | **Budget**     |
|------------------|------------------|-----------------|----------------|
| 1680-1050000     | 50% (50 XCC)     | 50% (50 XCC)    | 5% (0.05 XCC)  |
| 1050000-2100000  | 50% (25 XCC)     | 50% (25 XCC)    | 5% (1.5 XCC)   |
| 2100000-3150000  | 50% (12.5 XCC)   | 50% (12.5 XCC)  | 5% (1 XCC)     |
| 3150000-4200000  | 50% (6.25 XCC)   | 50% (6.25 XCC)  | 5% (0.5 XCC)   |
| 4200000-5250000  | 50% (3.12 XCC)   | 50% (3.12 XCC)  | 5% (0.25 XCC)  |
| 5250000-6300000  | 50% (1.56 XCC)   | 50% (1.56 XCC)  | 5% (0.13 XCC)  |
| 6300000-Infinite | 50% (0.78 XCC)   | 50% (0.78 XCC)  | 5% (0.06 XCC)  |


### Compile 

```bash
$ cd depends
$ sudo make
$ cd ..
$ sudo ./autogen.sh
$ sudo ./configure --prefix=$PWD/depends/x86_64-w64-mingw32
```

A prefix will be generated that's suitable for plugging into Bitcoin's
configure. In the above example, a dir named x86_64-w64-mingw32 will be
created. To use it for Bitcoin:

Common `host-platform-triplets` for cross compilation are:

- `i686-w64-mingw32` for Win32
- `x86_64-w64-mingw32` for Win64
- `x86_64-apple-darwin11` for MacOSX
- `arm-linux-gnueabihf` for Linux ARM 32 bit
- `aarch64-linux-gnu` for Linux ARM 64 bit

Now Check for :

- /src/cobaltcash-cli
- /src/cobaltcashd
- /src/cobaltcash-tx
- /src/qt/cobaltcash-qt
