# eSpace contract guide

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.ts
```

## Setup

Create `.env` file in root directory from `.env.example` and update the `PRIVATE_KEY` with your private key. Make sure it has some eSpace testnet CFX.

## Deploy in eSpace

```shell
npx hardhat run scripts/deploy.ts --network espaceTestnet
```

## Verify in eSpace

```shell
npx hardhat verify --network espaceTestnet <contract address> <space separated constructor parameters>
```