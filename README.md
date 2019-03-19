# Javascript interface for the Skycoin hardware wallet

[![Build Status](https://travis-ci.com/skycoin/hardware-wallet-js.svg?branch=master)](https://travis-ci.com/skycoin/hardware-wallet-js)

This library allows to communicate with the Skycoin hardware wallet.

## Protob dependencies

To communicate with the device, this library depends on [hardware-wallet-protob](https://github.com/skycoin/hardware-wallet-protob).
It is included as a submodule, so it is necessary to make some configurations before being able use the library.

### Get the files

To get the files from [hardware-wallet-protob](https://github.com/skycoin/hardware-wallet-protob), depending on the Git version
installed on the computer, run:

    git submodule update --init --recursive

or

    git submodule update --recursive --remote

### Build the protob files

Enter to the the `protob` folder and run:

    make build-js

## Documentation

The documentation of the library is in [DOCUMENTATION.md](DOCUMENTATION.md)