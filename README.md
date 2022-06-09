# SVD-Annotate for Ghidra

This is a fork of Thomas Roth's [SVD-Loader](https://leveldown.de/blog/svd-loader/).

This version does not create structures, but instead defines data items, labels, and comments for each peripheral register.
This was needed since some devices (e.g., nRF5x) have overlapping peripherals.

## Installation

Simply add the checked-out Git repository to your Ghidra-Scripts search paths.

## Usage

The script can be found in the `ARM` folder in Ghidra's Script Manager.

## Getting SVDs

- [cmsis-svd contains over 650 SVDs](https://github.com/posborne/cmsis-svd/)
- [Keil Software Packs](https://www.keil.com/pack)

## Credits

The original SVD-Loader is by Thomas Roth / leveldown security [More info here](https://leveldown.de/blog/svd-loader/).

The cmsis-svd code is a fork from Posborne's [cmsis-svd](https://github.com/posborne/cmsis-svd/), ported to work on Ghidra's Jython. Without this library this script could not exist!

## Licensing

The code in `cmsis_svd/` is licensed under the Apache License v2.0, the same as the 'upstream' [cmsis-svd](https://github.com/posborne/cmsis-svd/). The SVD-Annotate and SVD-Loader are both licensed under GPLv3.
