# Skaina Docs

## Features

### Core Functionality
- **Permissionless Lending & Borrowing**: Create lending pools for any supported token pair
- **Cross-Chain Operations**: Seamless asset transfers across different blockchains via LayerZero
- **Dynamic Interest Rates**: Adaptive interest rate models based on utilization
- **Flexible Collateral Management**: Support for multiple collateral types
- **Automated Liquidation**: MEV-friendly liquidation mechanisms with incentives
- **Position Management**: Individual position contracts for each user

### Advanced Features
- **Token Swapping**: Built-in DEX integration with saucerswap for position management
- **Oracle Integration**: Real-time price feeds for accurate asset valuations
- **Protocol Fee Management**: Automated fee collection and revenue distribution
- **Upgradeable Architecture**: UUPS proxy pattern for seamless upgrades
- **Access Control**: Role-based permissions for protocol management
- **Ecosystem Growth**: Self-sustaining mechanism that strengthens ecosystem

##  Architecture

### Core Contracts

#### LendingPoolFactory
- **Purpose**: Main factory contract for creating and managing lending pools
- **Features**: Pool creation, operator management, token data stream configuration
- **Upgradeable**: Yes (UUPS pattern)

#### LendingPool
- **Purpose**: Individual lending pool for specific token pairs
- **Features**: Supply/withdraw liquidity, borrow/repay assets, cross-chain transfers
- **Integration**: LayerZero for cross-chain operations

#### Position
- **Purpose**: Individual user position management
- **Features**: Collateral management, token swapping, repayment flexibility
- **Security**: Reentrancy protection, access control


### Supporting Contracts

- **IsHealthy**: Health check system for position validation
- **Liquidator**: Automated liquidation mechanisms
- **Oracle**: Price feed integration
- **LendingPoolRouter**: Interest rate calculations and pool management
- **PositionDeployer**: Factory for creating user positions


## Security

### Audit Status
- **Internal Review**: Completed

### Security Features
- **Reentrancy Protection**: All critical functions protected
- **Access Control**: Role-based permissions
- **Slippage Protection**: Built-in slippage controls
- **Health Checks**: Automated position validation
- **Upgrade Safety**: UUPS pattern with proper authorization

## Protocol Economics

### Fee Structure
- **Protocol Fee**: 0.1% of borrow amount
- **Liquidation Incentive**: 5-10% (configurable)
- **Cross-Chain Fee**: LayerZero messaging fees

