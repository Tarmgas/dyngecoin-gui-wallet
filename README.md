### Basic features:
* Generate/Backup/Restore wallet
* Encrypt wallet with password
* Built-in CPU miner with preferred pools
* Embedded/Local and remote blockchain
* Multiple location for remote blockchain
* Restore/display mnemonic phrases wallet from paper wallet (Thanks to https://github.com/seredat/karbowanecwallet/)
* Import/Export keys (not private spending and viewing key)
* Send and list transactions
* Block Explorer (for local blockchain)
* Contact list
* More...

### Recommendation
* Mnemonic phrases backup, we suggest to use English even though other languages are available.

### Build with Windows
#### Prerequisite
Install these:
* Microsoft Visual Studio 2017 Community Edition
* CMake 3.12 (Preferably GUI version)
* Boost 1.65  or later (32 or 63 bits depend on your build). You can get the compiled version from https://sourceforge.net/projects/boost/files/boost-binaries/
* Qt 5.10.x (32 or 63 bits depend on your build). If you can not find the binary for MSVC 2017, download 2015 version.
#### Generating project files and compilation
* Download or 
`git clone https://github.com/Tarmgas/dyngecoin-gui-wallet`
* Change working directory to  
`dyngecoin-gui-wallet`
 and 
`git clone https://github.com/Tarmgas/dyngecoin cryptonote`
* Launch CMake GUI and select source folder where you store 
`dyngecoin-gui-wallet`
. Build the binaries shall be 
`dyngecoin-gui-wallet/build/`
* Click Configure and select Visual Studio 2017 (64). Fix Qt lib paths and libboost path and re-configure again.
* Click Generate button. CMake will generate DyngeCoin-GUI.sln within 
`dyngecoin-gui-wallet/build/`
* Launch `x64 Native Tools Command Prompt for VS 2017` (64 bits) or `x86 Native Tools Command Prompt for VS 2017` (32 bits) and change working directory to 
`dyngecoin-gui-wallet/build/`
* In `build` directory, type 
`MSBuild DyngeCoin-GUI.sln /p:Configuration=Release`
* Wait a while. It will generate `DyngeCoin-GUI.exe` if everything goes fine.
* Qt library is required for `DyngeCoin-GUI.exe`. You shall change working directory to `build/Release` directory where there is the `DyngeCoin-GUI.exe` file, you shall run 
`c:\Qt\5.10.0\msvc2015\bin\windeployqt DyngeCoin-GUI.exe`
Change the path of where `windeployqt` you installed Qt. Qt necessary dll files will be copied to `Release` directory.
* Complete.

### Build with Linux
[Will write]

### Credit
Thanks to Cryptonote Developers, Bytecoin Developers, Monero Developers, Forknote Project, TurtleCoin Project Wrkzcoin Project and specifically to
* https://github.com/turtlecoin/ooze-wallet (based code)
* https://github.com/seredat/karbowanecwallet (Mnemonic features)

### Donation
[Doge]: DLu33DDpHzHHzCSVfGoLz77gcVFbWtGyd1

### Contact us
* Discord: https://discordapp.com/invite/Q4r2DdE
