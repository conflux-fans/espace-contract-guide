# eSpace contract guide

This is a hardhat basic project. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

We use it to demonstrate how to deploy a contract to `Conflux eSpace testnet`.

## Setup

Create `.env` file in the root directory from `.env.example` and update the `PRIVATE_KEY` with your dev private key. Make sure it has some eSpace testnet CFX. 

Note: You can get some testnet CFX from [eSpace faucet](https://efaucet.confluxnetwork.org/)

## Common hardhat tasks

After installing the dependencies(`npm install` or `yarn`), try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.ts
```

## Deploy in eSpace

```shell
npx hardhat run scripts/deploy.ts --network espaceTestnet
```

## Verify in eSpace

```shell
npx hardhat verify --network espaceTestnet <contract address> <space separated constructor parameters>
```

## Resources

- [Conflux eSpace](https://doc.confluxnetwork.org/docs/espace/Overview)
- [Hardhat documentation](https://hardhat.org/docs)
- [Community Hardhat ignition viem example](https://github.com/SPCFXDA/conflux-devkit-hhv)
- [Community Hardhat ignition ethers.js example](https://github.com/SPCFXDA/conflux-devkit-hhe)