# AVEX-MODE4
# MissionImpossible Token

## Overview
MissionImpossible is a simple ERC-20 token smart contract built on the Ethereum blockchain. The contract extends the OpenZeppelin ERC20 and Ownable contracts, providing basic functionality for a customizable token with additional features.

## Features
- **Token Name:** MissionImpossible
- **Symbol:** MI
- **Total Supply:** 10 MI tokens initially minted to the contract creator.
- **Ownership:** The contract owner has the ability to mint new tokens and has exclusive access to certain functions.

## Smart Contract Details
### Functions
1. **mintLoot**
   - **Visibility:** Public (onlyOwner)
   - **Description:** Mint additional MissionImpossible tokens and assign them to a specified address.

2. **redeemItem**
   - **Visibility:** Public
   - **Description:** Allows token holders to redeem a specific item by burning a predefined amount of MissionImpossible tokens.

3. **burnLoot**
   - **Visibility:** Public
   - **Description:** Allows token holders to burn a specified amount of MissionImpossible tokens.

### Constants
- **LootAmount:** 10 MI tokens are required to redeem an item.

### Storage
- **LootRedeemed:** A mapping to keep track of whether a token holder has already redeemed an item.

## Getting Started
1. Deploy the smart contract on the Ethereum blockchain.
2. The contract owner can mint additional tokens using the `mintLoot` function.
3. Token holders can redeem items using the `redeemItem` function.
4. Token holders can burn their tokens using the `burnLoot` function.

## License
This smart contract is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

