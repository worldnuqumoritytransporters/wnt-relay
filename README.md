# Relay for Wnt network

This is a node for Wnt network that stores the entire database and forwards new storage units to peers.  The relay does not hold any private keys and cannot send payments itself.

## Install

Install node.js, clone the repository, then say
```sh
npm install
```
If you want to accept incoming connections (you probably want), set up a proxy, such as nginx, to forward all websocket connections on a specific path to your daemon running the relay code.  See example configuration for nginx in [wntcore](../../../wntcore) documentation.

## Run
```sh
node start.js > log &
```
## Customize

If you want to change any defaults, refer to the documentation of [wntcore](../../../wntcore), the core Wnt library `require()`'d from here.
