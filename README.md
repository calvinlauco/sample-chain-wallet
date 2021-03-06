<p align="center">
  <img src="https://avatars0.githubusercontent.com/u/41934032?s=400&v=4" alt="Crypto.com Chain" width="400">
</p>

## Crypto.com Chain Sample Wallet

This repository contains a sample implementation of Crypto.com Chain wallet with integration of [client JSON-RPC server](https://github.com/crypto-com/chain/tree/master/client-rpc).

### Warning

Crypto.com Chain wallet is currently in the alpha development phase and subjects to changes. Before proceeding, please be aware of the following:

- This sample is for demonstration purposes only, do not use in production systems.

- Do not transfer any ERC20 tokens to addresses generated by this sample code as it can cause loss of funds.

Crypto.com is not liable for any potential damage, loss of data/files arising from the use of the sample wallet.

### Build

#### Build Prerequisites

- Node.js: https://nodejs.org/en/
- Crypto.com Chain: https://github.com/crypto-com/chain

#### Build instructions

- Start Crypto.com Chain by following instructions in the [Crypto.com Chain repository](https://github.com/crypto-com/chain)
- Start Crypto.com Chain Client RPC
```bash
$ ./target/debug/client-rpc --network-id 42 -i <main|test|dev>
```
- Run the following line to start serving the wallet
```bash
$ npm install
$ npm start
```
- Navigate to `http://localhost:4200/`.

### Configuration

#### ClientRPC Server URL

You can configure the ClientRPC server URL by changing the `clientRpcUrl` in `src/app/config.ts`

### How to create a new wallet

- A new wallet can be created using `Add wallet` button on UI and entering wallet name and passphrase.

### How to receive funds

- Share your wallet address and view key with with sender. Both, wallet address and view key, can be obtained by clicking `Receive funds` button

### How to send funds

- You can send funds by clicking `Send funds` button and entering recipient's wallet address, view key and other necessary details.

## Contribution

Please abide by the [Code of Conduct](CODE_OF_CONDUCT.md) in all interactions,
and the [contributing guidelines](CONTRIBUTING.md) when submitting code.

## License

[Apache 2.0](./LICENSE)
