# UniswapV2 TWAP Oracle Factory

Deplopyable networks

- Ethereum
  - Mainnet
  - Goerli
- Polygon
  - Mainnet
- Binance
  - Mainnet
- Avalanche
  - Mainnet
- Arbitrum
  - Mainnet
- Optimism (TBD)
- Fantom
  - Mainnet

## TWAP Oracle Factory Contracts

Utilizing a beacon proxy pattern, the factory allows for setting an initial implementation of the TWAP Oracle to be deployed by the user and the ability to be upgraded when needed. The upgrade will then reflect all current deployed implementations allowing for smooth transitions between versioning.

## TWAP Oracle Contracts

Upgradable implementaion contract that allows for automated TWAP on liquidity pool pair in the respected network DEX.

## Setup

### Anvil (Local Node)

Open another terminal

```bash
make run-node
```

### UI

Open a new terminal

```bash
cd ui && yarn
yarn dev
```

### Contracts

```bash
make script-factory-local
```

Navigate to [http://localhost:3000](http://localhost:3000), click the connect wallet button, and choose Blacksmith.

### Docs

To generate and view contract documentation in your browser.

```bash
make run-doc-server
```
