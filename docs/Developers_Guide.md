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

## Tools
- [brew](https://brew.sh/)
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
## Note if you have multiple users you may need todo the following
sudo chown -R $(whoami) /usr/local/Cellar

brew upgrade

```

- [Docker](https://docs.docker.com/docker-for-mac/install/)
- [Kubernetes](https://kubernetes.io/docs/user-journeys/users/application-developer/foundational/)
- [helm](https://github.com/kubernetes/helm)
- [npm and node](https://www.npmjs.com/get-npm)
- [mysql](https://gist.github.com/nrollr/3f57fc15ded7dddddcc4e82fe137b58e)

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

## Go
- [brew install go](http://brewformulas.org/Go)
- Work through the exercises in [The Go Programming Language](https://www.amazon.com/Programming-Language-Addison-Wesley-Professional-Computing-ebook/dp/B0184N7WWS/ref=mt_kindle?_encoding=UTF8&me=) using [Kindle Reader](https://read.amazon.com/)

## Node
```
brew update
brew install node
node -v
npm -v
brew upgrade node
npm install -g npm
```

## React
- Read the [getting started guide](https://reactjs.org/docs/getting-started.html)


## MySQL
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

## Gitbook
Instructions for installing Gitbook can be found [here](https://toolchain.gitbook.com/setup.html)
or you can use [brew cask](http://macappstore.org/gitbook/) 
```
brew cask install gitbook
```

## Rust

## Solidity

## Docker

## Kubernetes

## Helm

## Blockchains

### Ethereum - Go

### Ethereum - Parity

### Tendermint

### Bitcon

### EOS

### Stellar

## Repos

* ABCI
* IBC
* Peggy
* Tendermint
* Parity
* Governance
* Stable Coins
* OffChain Orchestration
* WASM




