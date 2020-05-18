BlvWallet Fullnode is a z-Addr first, Sprout compatible wallet and full node for bitcoinloved that runs on Linux, Windows.


# Installation


### Linux

If you are on Debian/Ubuntu, please download the '.AppImage' package and just run it.

```
./Blvwallet.Fullnode-0.0.1.AppImage
```

If you prefer to install a `.deb` package, that is also available.

```
sudo dpkg -i blvwallet_0.0.1_amd64.deb
sudo apt install -f
```

### Windows

You can download the release binary, unzip it and double click on `BlvWallet FullNode.exe` to start.


## bitcoinloved

BlvWallet needs a Bitcoinlove node running bitcoinloved. If you already have a bitcoinloved node running, BlvWallet will connect to it.

If you don't have one, BlvWallet will start its embedded bitcoinloved node.

Additionally, if this is the first time you're running BlvWallet or a bitcoinloved daemon, BlvWallet will download the Bitcoinlove params (~1777 MB) and configure `bitcoinlove.conf` for you.

## Compiling from source

BlvWallet is written in Electron/Javascript and can be build from source. Note that if you are compiling from source, you won't get the embedded bitcoinloved by default. You can either run an external bitcoinloved, or compile bitcoinloved as well.

#### Pre-Requisits

You need to have the following software installed before you can build Blvwallet Fullnode

- Nodejs v12.16.1 or higher - https://nodejs.org
- Yarn - https://yarnpkg.com

```
git clone https://github.com/biggiddybust/blvwallet.git
cd blvwallet

yarn install
yarn build
```

To start in development mode, run

```
yarn dev
```

To start in production mode, run

```
yarn start
```

