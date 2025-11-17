# Skaina

Skaina is a permissionless cross-chain lending and borrowing protocol built on the Moonbeam parachain within the Polkadot ecosystem. It enables users to supply collateral, borrow assets across chains, and manage their positions through a unified on-chain interface.

Skaina uses LayerZero for secure cross-chain messaging and API3 as its oracle provider for decentralized, accurate, and first-party price feeds.

Users can swap collateral for managing positions directly within the protocol, allowing them to rebalance exposure or optimize collateral health without relying on external bridges or separate swapping platforms.

With permissionless pool creation, anyone can launch isolated lending markets with custom risk parameters. This modular architecture makes Skaina flexible, transparent, and highly composable within the Moonbeam and broader Polkadot ecosystem.

## Why Built on Moonbeam?

- Ethereum-Compatible Smart Contract Environment: Moonbeam offers full EVM compatibility inside the Polkadot ecosystem, enabling Ethereum-native tooling and contracts to operate seamlessly. Skaina leverages this environment to deliver low-latency lending, smooth UX, and familiar Solidity-based interactions.

- Native Cross-Chain Capabilities: As a Polkadot parachain, Moonbeam is deeply connected to the entire ecosystem. Through LayerZero messaging, Skaina can extend liquidity and lending markets across multiple parachains and external chains, powering permissionless cross-chain borrowing and collateral movement without centralized bridges.

- Robust Oracle Infrastructure via API3: API3’s first-party oracle architecture ensures secure and tamper-resistant price feeds directly from data providers. By using API3, Skaina reduces oracle attack vectors and guarantees reliable pricing for liquidations, borrow limits, and collateral management.

- Active and Composable DeFi Environment: Moonbeam provides a rapidly growing DeFi ecosystem with strong developer tooling and liquidity layers. Skaina utilizes this foundation to enable:
  - isolated and permissionless lending pool creation
  - efficient collateral flows
  - deep composability with Moonbeam-native applications

This ecosystem positioning accelerates Skaina’s reliability and extensibility.

## Why Moonbeam is Ideal for Skaina

- Polkadot Security + EVM Flexibility: Moonbeam benefits from Polkadot’s shared security model while offering full EVM compatibility, combining robust chain security with Ethereum’s familiar development experience.

- Cross-Chain Liquidity Without Centralized Bridges: Using LayerZero, Skaina offers real-time, transparent, and trust-minimized liquidity movement across chains. This enables cross-chain lending and settlement at scale.

- Powered by API3 Oracles: API3 ensures Skaina receives

- Seamless Composability

## Problem
1. Fragmented liquidity across chains
2. Complex onboarding for new users
3. Inefficient liquidation and risk management
4. Limited permissionless lending on Moonbeam
5. Lack of aligned incentive mechanism
6. Limited collateral flexibility

## Solution
1. Isolated Pool Architecture
2. Smooth user onboarding
3. Real-time risk management with API3 Oracles
4. First permissionless cross-chain lending protocol on Moonbeam
5. Transparent and sustainable fee model
6. In-protocol collateral management

## Products
- Borrow
  - Skaina is a permissionless cross-chain lending and borrowing protocol built on the Moonbeam ecosystem, powered by LayerZero interoperability.
- Collateral Swap
  - Skaina provides in-protocol collateral swap functionality, allowing users to seamlessly exchange one collateral asset for another without leaving the platform.
- Buyback (Coming Soon)

## How Skaina Works
Skaina is built on a set of core modules that work together to deliver permissionless cross-chain lending and borrowing on Moonbeam.

- Main Interface: Skaina is accessible through its unified interface on Moonbeam, where users can supply and borrow assets, swap collateral, and manage their portfolios in one place.
- Collateral Supply Module Users can deposit assets as collateral from multiple chains via LayerZero interoperability, allowing liquidity to flow seamlessly into Skaina without manual bridging.

- Borrowing and Repayment Module: Users can borrow supported assets and repay across chains.
- Interest rates adjust dynamically based on utilization and asset risk profiles, ensuring efficient capital markets across the Skaina ecosystem.

- Collateral Swap Module: Skaina provides native in-protocol collateral swap functionality, giving users the flexibility to manage risk, optimize collateral composition, and reduce liquidation probability all without leaving the platform.

- Liquidation Module: This module maintains protocol stability by liquidating undercollateralized positions. Liquidators are incentivized to keep all markets solvent and balanced, ensuring long-term security for lenders.

- Oracle and Risk Management: Skaina uses API3 decentralized oracles for real-time price data and dynamic risk modeling. These feeds ensure accurate collateral valuation, fair interest rate adjustments, and efficient liquidation processes across chains.

## Deployments
### Moonbeam

| Contract                                       | Address                                      |
|-----------------------------------------------:|:---------------------------------------------|
| GLMR_liquidator                                | 0x5EA729df247eC491F19d9Cf0A191B400E3c66612  |
| GLMR_isHealthy                                 | 0x22448674F7e1512b94CEd8E6525B2ffA3a200605  |
| GLMR_lendingPoolDeployer                       | 0xe8CbC5b1537cfc6965150E5740BfECCB2F060789  |
| GLMR_protocol                                  | 0x7ceDEfF32A1eAcaAD2d006f79744A6ac580B8Fd4  |
| GLMR_positionDeployer                          | 0xe56738c93eD629bAa9aEb5Dd233c7F71ccAc5CF8  |
| GLMR_lendingPoolFactoryImplementation          | 0x03e7669B2e85CB7C61Af39307D79390B79c3aB7B  |
| GLMR_lendingPoolFactoryProxy                   | 0xAb9b266f64dA601F7afb9582dE59DF9485d7e48a  |

### Oracle — API3 Price Feeds

| Feed                 | Address                                      |
|---------------------:|:---------------------------------------------|
| USDT / USD           | 0x4eadC6ee74b7Ceb09A4ad90a33eA2915fbefcf76  |
| USDC / USD           | 0xD3C586Eec1C6C3eC41D276a23944dea080eDCf7f  |
| Native USDT          | 0xB64e610082d3c5C34130b8229E13DaB96180a6DF  |
| ETH / USDT           | 0x5b0cf2b36a65a6BB085D501B971e4c102B9Cd473  |
| BTC / USD            | 0xCAc4d304032a46C8D0947396B7cBb07986826A36  |

## Others
Links:

[Skaina Docs](https://skaina.gitbook.io/skaina-docs)

[Website] 
