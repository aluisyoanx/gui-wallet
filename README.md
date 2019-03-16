# Aluisyo Wallet (GUI)
Latest Release: v0.0.2
Maintained by Aluisyo.

## Warning: This is Highly Experimental for testing purposes Only, Use at own Risk!

## Information
### Aluisyo

The Future Of Blockchain Banking

Aluisyo is a decentralized cryptocurrency based on cryptonote with blockchain banking features and secure messaging.
Aluisyo is a fairly launched coin without any premine, ico or dev fee.

- Coin Name: Aluisyo
- Genesis Date: 25-02-19
- Ticker: ANX
- Address Prefix: aNX
- POW Algo: Cryptonight Fast
- Max Supply: 200milion
- Block Reward: smoothly increasing, starting from 5 all the way up-to 50
- Ports:
- P2P: 18001
- RPC: 19000


## Resources
- Web: [aluisyo.network](https://aluisyo.network/)
- GitHub: [https://github.com/aluisyonetwork/aluisyo-core](https://github.com/aluisyonetwork/aluisyo-core)
- Paperwallet: [https://paperwallet.aluisyo.network/](https://paperwallet.aluisyo.network/)
- Discord: [https://discord.gg/rbyNZRz](https://discord.gg/rbyNZRz)
- Our BitcoinTalk: https://bitcointalk.org/index.php?topic=5114934
- Our Telegram: https://t.me/joinchat/I5RElgnalLDhSHTQBjSluA

### [Block Explorers] 
- https://explorer.aluisyo.network/
- https://node.aluisyo.network/

### [Pools] 
- https://cnpool.cc/anx
- https://coinsforhash.com/aluisyo/

## Compiling Aluisyo from source

### Linux / Ubuntu

##### Prerequisites

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, Boost 1.55 or later, and Qt 5.9 or later.
You may download them from:

- http://gcc.gnu.org/
- http://www.cmake.org/
- http://www.boost.org/
- https://www.qt.io

Alternatively, it may be possible to install them using a package manager.

#### Building

To acquire the source via git and build the release version, run the following commands:

- `cd ~`
- `git clone https://github.com/aluisyonetwork/aluisyo-wallet`
- `cd aluisyo-wallet`
- `git clone https://github.com/aluisyonetwork/aluisyo-core.git cryptonote`
- `make build-release`
- `mkdir bin && mv build/release/Aluisyo-GUI bin/`
- `make clean`

If the build is successful the binaries will be in the bin folder.

### Windows 10

##### Prerequisites

- Install [Visual Studio 2017 Community Edition](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15&page=inlineinstall)
- When installing Visual Studio, you need to install **Desktop development with C++** and the **VC++ v140 toolchain** components. The option to install the v140 toolchain can be found by expanding the "Desktop development with C++" node on the right. You will need this for the project to build correctly.
- Install [CMake](https://cmake.org/download/)
- Install [Boost 1.67.0](https://boost.teeks99.com/bin/1.67.0/), ensuring you download the installer for MSVC 14.1.
- Install [Qt 5.11.0](https://www.qt.io/download)

##### Building

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017' or run "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\Tools\VsMSBuildCmd.bat" from any command prompt.
- Edit the CMakeLists.txt file and set the path to QT cmake folder. For example: set(CMAKE_PREFIX_PATH "C:\\Qt\\5.11.0\\msvc2017_64\\lib\\cmake\\").
- `git clone https://github.com/aluisyonetwork/aluisyo-core`
- `git clone https://github.com/aluisyonetwork/aluisyo-wallet`
- Copy the contents of the aluisyo-core folder into aluisyo-wallet\cryptonote
- `cd aluisyo-gui-wallet`
- `mkdir build`
- `cd build`
- `cmake -G "Visual Studio 15 2017 Win64" -DBOOST_LIBRARYDIR:PATH=c:/local/boost_1_67_0 ..` (Or your boost installed dir.)
- `msbuild ALUISYO-GUI.sln /p:Configuration=Release`

If the build is successful the binaries will be in the Release folder.

#### Special Thanks
Special thanks goes out to the developers from Cryptonote, Bytecoin, Monero, Forknote, TurtleCoin, Masari, The Circle Team
