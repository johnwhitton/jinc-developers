# jinc-developers
Developers Guide for Jincubator Developers

# Environment Set up
## Terminal
-  [iterm2](https://code.visualstudio.com/docs?start=true)

## Source Control
- [git via XCODE](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [git manual for mac](https://git-scm.com/download/mac)

Download a [personal access token](https://github.com/settings/tokens) and use this the first time you clone a repository.

```
git --version
cd ~
mkdir projects
cd projects
git clone https://github.com/johnwhitton/jinc-developers.git
```

## Editors

- [Atom](https://atom.io/)
- [Visual Studio](https://code.visualstudio.com/docs?start=true)

## Communication
- [skype](https://www.skype.com/en/get-skype/skype-for-mac/) - Business Users
- [slack](https://slack.com/downloads/osx) - Internal teams and stellar, go, gcp
- [Rocketchat](https://rocket.chat/download) - Hyperledger
- [gitter](https://gitter.im/apps) - Ethereum
- [Keybase](https://keybase.io/download) - Stellar
- [Riot](https://about.riot.im/)
- [Telegram](https://telegram.org/)


## Other
- [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Amazon Reader](https://read.amazon.com/)

## Tools

### [Brew](https://brew.sh/)
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
## Note if you have multiple users you may need todo the following
sudo chown -R $(whoami) /usr/local/Cellar

brew upgrade

```

### Docker
- [Docker](https://docs.docker.com/docker-for-mac/install/)


- [npm and node](https://www.npmjs.com/get-npm)
- [mysql](https://gist.github.com/nrollr/3f57fc15ded7dddddcc4e82fe137b58e)

### Kubernetes
- [Kubernetes](https://kubernetes.io/docs/user-journeys/users/application-developer/foundational/)

### Helm
- [helm](https://github.com/kubernetes/helm)

### MySQL
This can be done via [brew](https://gist.github.com/nrollr/3f57fc15ded7dddddcc4e82fe137b58e) , 
[docker](https://docs.docker.com/samples/library/mysql/) or 
[natively](https://dev.mysql.com/doc/refman/5.7/en/osx-installation-pkg.html)

The following uses [brew](https://brew.sh/)

```
$ brew info mysql
$ brew install mysql
$ brew upgrade mysql

 $ brew tap homebrew/services
 $ brew services start mysql
 $ brew services list
 $ mysql -V
 $ mysql -u root
```

or the following to set a password

``` 
$ mysqladmin -u root password 'yourpassword' 
```

### Gitbook
Instructions for installing Gitbook can be found [here](https://toolchain.gitbook.com/setup.html)
or you can use [brew cask](http://macappstore.org/gitbook/) 

```
brew cask install gitbook
```

[Creating a gitbook](https://toolchain.gitbook.com/setup.html)

```
npm install gitbook-cli -g
cd ~/projects
mkdir gitbookSample
cd gitbookSample/
gitbook init
gitbook serve

```

## Programming Languages

### Go
- [brew install go](http://brewformulas.org/Go)
- Work through the exercises in [The Go Programming Language](https://www.amazon.com/Programming-Language-Addison-Wesley-Professional-Computing-ebook/dp/B0184N7WWS/ref=mt_kindle?_encoding=UTF8&me=) using [Kindle Reader](https://read.amazon.com/)

### Node
```
brew update
brew install node
node -v
npm -v
brew upgrade node
npm install -g npm
```

### React
- Read the [getting started guide](https://reactjs.org/docs/getting-started.html)




### Rust

Install using [rustup](https://www.rust-lang.org/en-US/install.html) or [other rust installers](https://www.rust-lang.org/en-US/other-installers.html)

Using rustup

```
curl https://sh.rustup.rs -sSf | sh
source $HOME/.cargo/env
rustup -V
rustup update stable
```

_Note: Still need to go through [getting started](https://doc.rust-lang.org/book/first-edition/getting-started.html_) to build first rust program_

### Solidity
The following gives an overview of how to [Install Solidity](http://solidity.readthedocs.io/en/v0.4.24/installing-solidity.html)

To install using npm

```
npm install -g solc
```


## Blockchains

### Ethereum - Go

https://geth.ethereum.org/downloads/

Instructions for installing via brew are [here](https://github.com/ethereum/go-ethereum/wiki/Installation-Instructions-for-Mac)

### Ethereum - Parity

https://github.com/paritytech/parity/releases

To install using brew use the [following link](
https://github.com/paritytech/homebrew-paritytech/blob/master/README.md) , note you may have to install xcode via the app store before installing the additional binaries

```
brew install ethabi
brew install ethkey
brew install ethstore
```

### Tendermint

To install use the [following link](https://tendermint.readthedocs.io/projects/tools/en/master/install.html)

### Bitcon
Please see the following for [bitcoin](https://bitcoin.org/en/download) and read over the notes for [light clients or pruning](https://bitcoin.stackexchange.com/questions/48882/is-there-a-light-spv-version-of-bitcoin-core-bitcoind)

Also see the [parity bitcoin client](https://github.com/paritytech/parity-bitcoin) for a light client.

### EOS
To install use the [following link](https://developers.eos.io/eosio-nodeos/docs/docker-quickstart)

### Stellar
To install use the [following link](https://github.com/stellar/stellar-core/blob/master/INSTALL.md) or the [docker version](https://github.com/stellar/docker-stellar-core-horizon)

### Maker DAO
To install use the [following link](https://makerdao.com/documentation/#installation)

## Repos

* ABCI - [tendermint](https://github.com/tendermint/tendermint/tree/master/abci)
  * [One Ledger Protocol](https://github.com/Oneledger/protocol)
* IBC - [specification in cosmos](https://github.com/cosmos/cosmos/blob/master/WHITEPAPER.md#ibc-packet-delivery-acknowledgement)
* [Peggy](https://github.com/cosmos/peggy)
* [Tendermint](https://github.com/tendermint/tendermint) - also see [amino](https://github.com/tendermint/go-amino)
* Parity - [ethereum](https://github.com/paritytech/parity-ethereum) and [bridge](https://github.com/paritytech/parity-bridge) and [parity bitcoin](https://github.com/paritytech/parity-bitcoin)
* [Polkadot](https://github.com/paritytech/polkadot)
* [Stellar](https://github.com/stellar)
* [Fabric](https://github.com/hyperledger/fabric) - [Jira board](https://jira.hyperledger.org/secure/RapidBoard.jspa?projectKey=FAB&rapidView=7&view=planning)
* Governance 
  * [tendermint consensus](https://github.com/tendermint/tendermint/blob/master/docs/spec/consensus/consensus.md) 
  * [Rocket Pool](https://github.com/rocket-pool/rocketpool)
* Stable Coins
  * [Maker DAO](https://github.com/makerdao) 
    * [documentation](https://github.com/makerdao/documentation)
    * [maker-otc](https://github.com/makerdao/maker-otc)
    * [maker-keeper](https://github.com/makerdao/market-maker-keeper)
  * [KowalaTech - KCOIN](https://github.com/kowala-tech/kcoin)
* OffChain Orchestration
  * [ChainLink](https://github.com/smartcontractkit/chainlink)
* WASM 
  * [Parity WASM tools](https://github.com/paritytech/wasm-utils)
  * [Ethereum WASM - eWASM](https://github.com/ewasm/design)
  * [WASM specification](https://github.com/WebAssembly/spec)
* Smart Contracts
  * [ERC-20](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-20.md) [issue](https://github.com/ethereum/EIPs/issues/20)
  * [ERC-223](https://github.com/ethereum/EIPs/issues/223)	- Like ERC-20 but with uniformity and  transfer handling  
  * [ERC-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md)	"Non-Fungible Tokens - Used for CryptoKitties - [write up](https://medium.com/crypto-currently/the-anatomy-of-erc721-e9db77abfc24) 
  * [ERC-827](https://github.com/ethereum/EIPs/issues/827)	- Extends ERC-20
  * [ERC-820](https://eips.ethereum.org/EIPS/eip-820) - Use of Registries
  * [EIP-777](https://eips.ethereum.org/EIPS/eip-777) - Extends ERC-20 and [ERC-820](https://eips.ethereum.org/EIPS/eip-820)
  * [MakerDAO](https://github.com/makerdao/sai/tree/master/src)	- Smart Contracts 
    * [Market Place](https://github.com/makerdao/maker-otc/tree/master/src)
  * TrueUSD	
    * [ERC-20](https://github.com/trusttoken)
    * [Staking](https://github.com/trusttoken/TrustToken-smart-contracts/blob/master/staking.sol)
  * [Bethereum](https://github.com/bethereumproject) - Bethereum's Smart Contracts
  * [AltEstate](https://github.com/AltEstate/altestate/tree/master/contracts) - Alt Estate - DPOS Smart Contracts
  * [OpenZeppelin](https://github.com/OpenZeppelin/openzeppelin-solidity/tree/master/contracts) - Open Zeppelin Smart Contracts
  * [Qurrex](https://github.com/Qurrex/smart_contracts) - Qurrex - ICO Smart Contracts
  * [Kowala](https://github.com/kowala-tech/edge-currency-kowala) - Kowala - Intergrate Bitcoin Send Recieve Functionality
  * [Solidified](https://github.com/solidified-platform) - Smart Contract Auditing - [website](https://solidified.io/)




