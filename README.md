# Gridix Core

Gridix Core is a smart contract framework for automated grid trading strategies on Uniswap V3 and other DEX protocols.

## Overview

Gridix Core provides a robust infrastructure for implementing grid trading strategies on decentralized exchanges. It enables users to create and manage automated grid trading positions with customizable parameters.

## Key Features

- Automated grid trading strategy implementation
- Support for Uniswap V3 and other DEX protocols
- Customizable grid parameters (price range, grid count, investment amount)
- Position management and rebalancing
- Factory pattern for easy deployment

## Architecture

The project is organized into several key components:

### Contracts Structure
```
contracts/
├── base/           # Base contract implementations
├── factory/        # Factory contracts for deployment
├── grid/          # Core grid strategy implementations
├── helper/        # Helper utilities and libraries
└── interfaces/    # Contract interfaces
```

### Key Components

- **Grid Contracts**: Implement the core grid trading logic
- **Factory Contracts**: Handle the deployment and initialization of grid strategies
- **Base Contracts**: Provide fundamental functionality and shared logic
- **Helper Contracts**: Offer utility functions and additional features
- **Interfaces**: Define the contract interfaces and types

## Grid Trading Strategy

The grid trading strategy implemented in this framework:
- Divides a price range into multiple grid levels
- Automatically places buy and sell orders at each grid level
- Manages position rebalancing when price moves between grids
- Supports customizable parameters including:
  - Upper and lower price bounds
  - Number of grid levels
  - Total investment amount
  - Extra token allocation

## Usage

To implement a grid trading strategy:

1. Deploy the appropriate factory contract
2. Call the factory to create a new grid strategy
3. Configure the grid parameters:
   - Set price range
   - Define grid count
   - Specify investment amount
4. Activate the strategy

## Development

### Prerequisites

- Solidity ^0.8.0
- Hardhat/Truffle development environment
- Node.js and npm

### Testing

Tests are included to verify the functionality of all components.

## Security

This project is under active development. While we strive to ensure the security of our contracts, please use them at your own risk.

## License

GPL-2.0-or-later

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
