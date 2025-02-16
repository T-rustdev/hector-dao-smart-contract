# Hector DAO Contracts

This repository contains the smart contracts for Hector DAO, a decentralized autonomous organization operating on the Fantom blockchain. Hector DAO aims to provide a decentralized financial center through various use cases, including staking, bonding, and more.

## Overview

Hector DAO utilizes a set of smart contracts deployed on the Fantom network to facilitate financial transactions with crypto assets. Participants can acquire the native token, HEC, which carries voting rights within the DAO. HEC can be obtained by exchanging other crypto assets or purchasing from existing holders on the secondary market.

## Repository Structure

The repository is organized into the following directories:

- **bond**: Contracts related to the bonding mechanism.
- **staking**: Contracts for staking HEC tokens.
- **treasury**: Manages the DAO's treasury operations.
- **utils**: Utility contracts and libraries.
- **voting**: Contracts facilitating governance and voting within the DAO.

## Key Contracts

- `HectorBondDepository.sol`: Manages the bonding process, allowing users to acquire HEC tokens at a discount by providing liquidity or other assets.
- `HectorStaking.sol`: Handles the staking mechanism, enabling users to stake their HEC tokens in return for rewards.
- `HectorTreasury.sol`: Oversees the treasury, ensuring the DAO's assets are managed and utilized effectively.
- `DAO.sol`: The core governance contract, allowing HEC token holders to propose and vote on changes within the DAO.

## Getting Started

To interact with or develop on top of Hector DAO's contracts:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Myrmekes-a/hector-dao-contracts.git
   cd hector-dao-contracts
   ```
2. **Install Dependencies:** Ensure you have Node.js and npm installed. Then, install the necessary packages:
   ```bash
   npm install
   ```
3. **Compile Contracts:** Use a Solidity compiler to compile the contracts. For example, with Hardhat:
   ```bash
   npx hardhat compile
   ```
4. **Run Testss:** Execute the test suite to ensure all contracts function as expected:
   ```bash
   npx hardhat test
   ```

## Deployment
To deploy the contracts to the Fantom network:

1. **Configure Network Settings:** Update the hardhat.config.js file with the Fantom network configuration and your deployment account's private key.

2. **Deploy Contracts:** Run the deployment script:
    ```bash
   npx hardhat run scripts/deploy.js --network fantom
   ```