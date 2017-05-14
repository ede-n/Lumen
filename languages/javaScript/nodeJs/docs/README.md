# Learn NodeJs

## NodeJs

* uses an _event-driven_, _non-blocking I/O_ model

* is a javaScript runtime that uses V8 javascript engine

* utilizes _libuv_, a multiplatform support library with a focus on async I/O

* is single-threaded, but under the hood libuv handles threading, file system events, implements event loop, features thread pooling and so on

* the stable versions with long-term support (LTS) are the ones starting with even numbers (4, 6, 8 ...)

* the experimental version are the odd numbers (5, 7 ...)

## NVM

* is the node version manager and can be installed with `brew install nvm`

### NVM Cheat Sheet

* `nvm ls` - displays the versions of nodeJs installed

* `nvm current` - display currently activated version

* `nvm ls-remote` - check available node.js versions

* `nvm install 7.10.0` - installs specific nodeJs version

* `nvm use 7.10.0` - activates specific nodeJs version

## NodeJs Project

A node project is nothing but a node package, created using the node package manager.

```bash
mkdir learn-node
cd learn-node
npm init
 
```

## References

1. [Node Hero](https://blog.risingstack.com/node-hero-tutorial-getting-started-with-node-js/)
1. [NVM](https://www.liquidweb.com/kb/how-to-install-node-js-via-nvm-node-version-manager-on-ubuntu-14-04-lts/)