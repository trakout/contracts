# Opus-foundation smart contracts
![opus-logo](img/opus_logo_big.png)
<br />
[Opus](http://opus-foundation.org/) - the worlds's first decentralised music platform, based on IPFS and Ethereum. <br />
Solidity smart contracts for Opus official token, crowdsale & testnet demo token. Also includes [advanced-demo website](http://opus-foundation.org/advanced-demo.html).
<br />
## Token Standards
Opus token is compliant to the [ERC23](https://github.com/ethereum/EIPs/issues/223) standards, as well as backward compatible with the [ERC20](https://github.com/ethereum/eips/issues/20) standards.
<br />
## Security Patterns
Uses [zeppelin-solidity ERC20 library](https://github.com/OpenZeppelin/zeppelin-solidity
) by OpenZeppelin.
<br />
## Prerequisites
To install demo you need:

- [npm](https://www.npmjs.com/)
- [Truffle v3.2.4](https://github.com/trufflesuite/truffle-core)
- [EthereumJS TestRPC v3.0.5](https://github.com/ethereumjs/testrpc)
- [Go IPFS](https://ipfs.io/docs/install/)

To install truffle, run the following command:
```sh
$ npm install -g truffle
```
To install testrpc, run:
```sh
npm install -g ethereumjs-testrpc
```

## Build
To build demo, clone this repo and run the following command:
```sh
$ cd contracts
$ npm install
```

## Running the demo
To run demo, first run testrpc by running:
```sh
$ testrpc
```
Then compile and deploy the solidity contracts:
```sh
$ truffle compile
$ truffle migrate
```
Run an instance of IPFS to enable uploads:
```sh
$ ipfs daemon
```
Finally to build website, run:
```sh
$ npm run dev
```

## License
All smart contracts are released under GPL v.3.
