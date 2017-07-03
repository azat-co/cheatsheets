# Node and npm Cheatsheet

> Node, Node... it's everywhere.

[FREE beautifully-designed print-ready PDF](https://node.university/p/library).


## Installation

npm comes with Node. Node 6, 8, 10, etc are long-term support versions. 

## brew (macOS only)

if no brew, then install it first:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

```
brew update && brew install node
```

## Installer (recommended for beginners)

Download installer from <https://nodejs.org>

## source (recommended for contributors) 

Unix / macOS Prerequisites:

* gcc and g++ 4.9.4 or newer
* clang and clang++ 3.4.2 or newer (macOS: latest Xcode Command Line Tools)
* Python 2.6 or 2.7
* GNU Make 3.81 or newer

Windows Prerequisites:

* Building Node: Visual Studio 2015 or Visual C++ Build Tools 2015 or newer
* Building native add-ons: Visual Studio 2013 or Visual C++ Build Tools 2015 or newer


```
git clone git@github.com:nodejs/node.git
cd node
./configure
make -j4
```

Test and make it a system Eode:

```
make test
./node -e "console.log('Hello from Node.js ' + process.version)"
make instal
```

## nvm (recommended for switching between multiple versions)

nvm does not support Windows

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash
```

## yum 

OSs: Amazon Linux, Red Hat® Enterprise Linux® / RHEL, CentOS, CloudLinux, Oracle Linux and Fedora


```
curl --silent --location https://rpm.nodesource.com/setup_8.x | bash -
yum -y install nodejs
```


##  apt-get

OSs: Debian, Ubuntu, Alpine, Linux Mint, Linux Mint Debian Edition (LMDE), elementaryOS

```
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y nodejs
```

## Usage

* REPL: `$ node`
* Eval: `$ node -e "{code}"`
* File: `$ node {filename.js}`

# Node Globals

* setTimeout()
* require
* __dirname
* __filename
* process.env
* process.argv
* process.exit()
* process.cwd()
* process.versions

# Node Core

* http
* utils
* os
* cluster
* stream
* event
* fs
* url
* path
* net


# package.json

Main package.json properties:

* version
* devDependencies
* dependencies
* name


# npm

* `npm init` and `npm init -y`
* `npm i {npm-package-name}` also with `-g`, `-S`, `-E` or `-D`
* `npm rm {npm-package-name}` also with `-g`, `-S`, or `-D`
* `npm version patch` also major and minor
* `npm i --production` or `NODE_ENV=production npm i`
* `npm config ls`
* `npm config set {config-key} {config-value}`
* `npm i git+http://github.com/{username}/{repo-name}.git`


# Node C++ Addons

# Popular Node Modules

* request, axios, superagent and fetch
* mocha, jasmine, jest and tape
* passport and oauth
* express, hapi and loopback
* mongodb, mongoose, sequilize, and shelf


## Resources

* [Node Foundation](https://nodejs.org)
* [Node School](http://nodeschool.io)
* [Node University](https://node.university)
