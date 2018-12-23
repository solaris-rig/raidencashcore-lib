# RaidenCashcore Library

[![Build Status](https://img.shields.io/travis/solaris-rig/raidencashcore-lib.svg?branch=master)](https://travis-ci.org/solaris-rig/raidencashcore-lib)
[![NPM Package](https://img.shields.io/npm/v/raidencashcore-lib.svg)](https://www.npmjs.org/package/raidencashcore-lib)

> A pure and powerful JavaScript RaidenCash library.

RaidenCash is a powerful new peer-to-peer platform for the next generation of financial technology. The decentralized nature of the RaidenCash network allows for highly resilient RaidenCash infrastructure, and the developer community needs reliable, open-source tools to implement RaidenCash apps and services.

## Table of Contents
- [Install](#install)
- [Usage](#usage)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [License](#license)

## Install

### NodeJS

```
npm install raidencashcore-lib
```

### Browser

See the section below to generate your own bundle, or download the pre-generated [minified file](dist/raidencashcore-lib.min.js)

#### Building the Browser Bundle

To build a raidencashcore-lib full bundle for the browser:

```sh
npm run build
```

This will generate files named `raidencashcore-lib.js` and `raidencashcore-lib.min.js` in the `dist/` folder.

## Usage

### Browser

```
<script src='./dist/raidencashcore-lib.min.js' type="text/javascript"></script>
<script>
  const PrivateKey = raidencashcore.PrivateKey;
  const privateKey = new PrivateKey();
  const address = privateKey.toAddress().toString();
</script>
```

### Modules

Some functionality is implemented as a module that can be installed separately:

* [Payment Protocol Support](https://github.com/dashevo/raidencashcore-payment-protocol)
* [Peer to Peer Networking](https://github.com/dashevo/raidencashcore-p2p)
* [RaidenCash JSON-RPC](https://github.com/dashevo/dashd-rpc)
* [Payment Channels](https://github.com/solaris-rig/raidencashcore-channel)
* [Mnemonics](https://github.com/dashevo/raidencashcore-mnemonic)
* [Elliptical Curve Integrated Encryption Scheme](https://github.com/dashevo/bitcore-ecies-dash)
* [Signed Messages](https://github.com/dashevo/bitcore-message-dash)

### Development & Tests

```sh
git clone https://github.com/solaris-rig/raidencashcore-lib
cd raidencashcore-lib
npm install
```

Run all the tests:

```sh
npm test
```

You can also run just the Node.js tests with `npm run test:node`, just the browser tests with `npm run test:browser` or run a test coverage report with `npm run coverage`.

## Documentation

* [Addresses](docs/address.md)
* [Block](docs/block.md)
* [Crypto](docs/crypto.md)
* [Encoding](docs/encoding.md)
* [Hierarchically-derived Private and Public Keys](docs/hierarchical.md)
* [Networks](docs/networks.md)
* [PrivateKey](docs/privatekey.md)
* [PublicKey](docs/publickey.md)
* [Script](docs/script.md)
* [Transaction](docs/transaction.md)
* [Using Different Units](docs/unit.md)
* [Unspent Output](docs/unspentoutput.md)
* [URI](docs/uri.md)
* [Governance Object / Proposal](docs/govobject/govobject.md)

### Examples

Some examples can be found [here](docs/examples.md), below is a list of direct links for some of them.

* [Generate a random address](docs/examples.md#generate-a-random-address)
* [Generate an address from a SHA256 hash](docs/examples.md#generate-a-address-from-a-sha256-hash)
* [Import an address via WIF](docs/examples.md#import-an-address-via-wif)
* [Create a Transaction](docs/examples.md#create-a-transaction)
* [Sign a RaidenCash message](docs/examples.md#sign-a-bitcoin-message)
* [Verify a RaidenCash message](docs/examples.md#verify-a-bitcoin-message)
* [Create an OP RETURN transaction](docs/examples.md#create-an-op-return-transaction)
* [Create a 2-of-3 multisig P2SH address](docs/examples.md#create-a-2-of-3-multisig-p2sh-address)
* [Spend from a 2-of-2 multisig P2SH address](docs/examples.md#spend-from-a-2-of-2-multisig-p2sh-address)

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/solaris-rig/raidencashcore-lib/blob/master/CONTRIBUTING.md) file.

## License

Code released under [the MIT license](LICENSE).

Copyright 2013-2017 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.  
Copyright 2016-2017 The RaidenCash Foundation, Inc.  
Copyright 2017-2018 RaidenCash Group, Inc.  
