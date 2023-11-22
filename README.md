## Packages

forge install openzeppelin/openzeppelin-contracts@v4.0.0 --no-commit
forge install smartcontractkit/chainlink-brownie-contracts@0.8.0 --no-commit

## Design Spec

1. (Relative Stability) Anchored or Pegged => $1.00
   1. Chainlink Price Feed
   2. Set a function to exchange ETH & BTC - $$$
2. Stability Mechanism (Minting): Algorithmic (Decentralized)
   1. People can only mint the stablecoin with enough collateral (coded logic)
3. Collateral: Exogenous (Crypto)
   1. wETC
   2. wBTC

## Scenarios

If under a threshold, 150% for example

Then someone pays back your minted DSC, they can have all your collateral for a discount as reward for safe-guarding the protocol.

This incentivizes people not to over leverage position on stablecoin, because the lose more than they borrow.

| $DSC     | Crypto | Amount |
| -------- | ------ | ------ |
| $100 DSC | ETH    |        |

Need data feed from .
https://data.chain.link/

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```

<!-- forge install smartcontractkit/foundry-chainlink-toolkit --no-commit -->

## Reminder

- [Full course](https://github.com/Cyfrin/foundry-full-course-f23)
- [Forta Bot](https://www.youtube.com/watch?v=42RcaQ8YTzQ)
